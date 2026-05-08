# Cloudinary Integration Plan

## Decision Summary

- Decision: adopt Cloudinary for image binaries, keep GitHub for metadata and editorial workflow.
- Why: avoids repository bloat, improves delivery performance via CDN, and enables responsive image transformations.
- Rollout: phased migration with mixed-mode support so legacy blob references keep working during transition.
- Operational model: `shr-admin` uploads to Cloudinary and opens PRs that update YAML references in `shr-contents`.
- Fallback: if Cloudinary is unavailable, continue serving legacy GitHub/blob-backed images while pausing new Cloudinary uploads.

## Goal

Move image binary storage out of GitHub (`shr-contents`) and into Cloudinary, while keeping editorial workflow and site generation driven by pull requests and content metadata.

## Scope

- `shr-contents`: keep image metadata and references only
- `shr-admin`: upload and optimize images, then store Cloudinary references in YAML via PRs
- `shr-web`: consume Cloudinary URLs and generate responsive/transformed URLs for rendering

## Current Architecture

1. `shr-admin` uploads files and opens PRs against `shr-contents`.
2. `shr-contents` stores image binaries in `blobs/` and metadata in YAML collections.
3. `shr-web` syncs content and emits `public/image-collections.json.gz` with image links.

## Target Architecture

1. Editors upload images in `shr-admin`.
2. `shr-admin` sends files to Cloudinary and receives `secure_url` + `public_id`.
3. `shr-admin` opens PRs to `shr-contents` updating only metadata YAML (no binary blobs).
4. `shr-web` reads Cloudinary-backed metadata and outputs responsive image variants.
5. Frontend serves optimized images via Cloudinary CDN.

## Data Model Changes

### Existing

Collections currently reference local blob paths (for example `sourcePath` under `blobs/...`).

### Proposed

Add Cloudinary fields per image item:

- `imageUrl`: canonical Cloudinary HTTPS URL
- `publicId`: Cloudinary asset identifier for transformations
- `metadata` (optional): width, height, format, bytes
- Keep existing descriptive fields (title, credit, caption, etc.)

## Repository-by-Repository Plan

### 1) `shr-admin`

#### Environment configuration

Add:

- `CLOUDINARY_CLOUD_NAME`
- `CLOUDINARY_API_KEY`
- `CLOUDINARY_API_SECRET`
- Optional: `CLOUDINARY_UPLOAD_PRESET`

#### Upload pipeline changes

- Keep current validation and optimization (`sharp`) in `src/lib/image-upload.ts`.
- After optimization, upload bytes to Cloudinary using signed server-side upload.
- Capture `secure_url`, `public_id`, and derived metadata.
- For race assets and collections flows, create PR file changes that update YAML metadata only.

#### UX behavior

- Continue showing previews and validation errors as now.
- On success, show uploaded asset summary (URL, dimensions, format).
- PR description should list modified YAML files and linked asset IDs.

### 2) `shr-contents`

#### Content storage policy

- Keep YAML collections in git.
- Stop committing new images to `blobs/` for Cloudinary-managed paths.
- Optionally retain legacy `blobs/` during migration and support mixed-mode references temporarily.

#### YAML schema evolution

Update collection schemas to accept either:

- Legacy local path (`sourcePath`), or
- Cloudinary-backed references (`imageUrl`, `publicId`)

This allows phased migration with no hard cutover.

### 3) `shr-web`

#### Build pipeline changes

- While generating `public/image-collections.json.gz`, detect Cloudinary-backed items.
- For Cloudinary entries, emit transformation URLs for key breakpoints (thumbnail/card/hero/mobile).
- Preserve backward compatibility for legacy GitHub raw URL entries until migration completes.

#### Frontend rendering

- Prefer `picture`/`srcset` (or equivalent component strategy) with Cloudinary variants.
- Keep lazy-loading and explicit dimensions for CLS stability.
- Use transformation presets consistently across homepage, race galleries, portraits, and documents.

## Migration Strategy

1. Implement Cloudinary upload path in `shr-admin` behind a feature flag.
2. Extend YAML schema and parsing in both admin and web build tooling.
3. Enable mixed-mode rendering in `shr-web` (local/GitHub + Cloudinary).
4. Batch migrate existing `blobs/` images to Cloudinary and update YAML references.
5. Freeze new binary uploads to `blobs/`.
6. Optionally archive or prune legacy blobs once confidence is high.

## Operational Considerations

- Folder naming convention in Cloudinary:
  - `homepage/...`
  - `races/<raceId>/...`
  - `portraits/...`
  - `documents/...`
- Apply tags at upload (`shr`, section, race ID) for asset management.
- Store `public_id` in YAML to avoid URL-coupling and enable safe URL regeneration.
- Define deletion/replace policy (retain old versions vs overwrite semantics).
- Add simple audit logging in admin PR bodies and commit messages.

## Cost and Limits

- Cloudinary free tier should cover current scale for early adoption.
- Main free-tier watchpoints:
  - Monthly transformation volume
  - Bandwidth/CDN egress
  - Storage growth as galleries expand

## Risks and Mitigations

- Vendor lock-in risk: keep `publicId` + metadata in open YAML and avoid opaque-only references.
- URL churn risk: derive delivery URLs from `publicId` in build/runtime.
- Partial migration complexity: support both legacy and Cloudinary records during transition.
- Editorial disruption: keep admin forms unchanged where possible; swap backend storage only.

## Acceptance Criteria

- Editors can upload race/homepage/portrait images without committing binaries to git.
- PRs in `shr-contents` include only metadata changes for new Cloudinary assets.
- `shr-web` renders responsive Cloudinary images with no regression for legacy entries.
- Existing content remains valid during migration.
- Build output remains deterministic and deployment-safe.

## Suggested Rollout

1. Pilot on one collection (for example homepage images).
2. Extend to race galleries.
3. Extend to portraits/documents where appropriate.
4. Migrate historical blobs in batches.
5. Enforce policy to block new large image binaries in `shr-contents`.
