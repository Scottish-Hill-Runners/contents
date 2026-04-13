# Pictures

This folder now has a first-pass curation layer for website use.

The source archive remains in place. The approved subsets for website work live in `collections.yaml` as named collections that a frontend or build step can consume later.
The collections manifest now lives at the repository root in `../collections.yaml` so build pipelines can fetch it without cloning the full `Pictures` folder.

## Current collections

- `homepage-decorative-draft`
  - Use for: background mosaic, image wall, section background band
  - Do not use for: full-width hero, text-heavy overlay, automatic race-page imagery
- `committee-portraits-draft`
  - Use for: committee, office-holder, and governance/profile pages
  - Do not use for: decorative backgrounds or homepage mosaics

## Curation rules

- Prefer scenic landscapes and runners-in-landscape action shots.
- Keep older low-resolution images only when they still work as atmosphere in a mosaic.
- Keep committee portraits separate from decorative imagery.
- Avoid `-sidebar` variants.
- Avoid batch exports, UUID-style names, merchandise graphics, calendars, maps, scans, and crowd-heavy start or finish photos in the first pass.
- Treat anything not in `../collections.yaml` as unreviewed.

## Notes for implementation

- This repository is content-only. The frontend app will need to decide how to render these collections.
- The first pass is intentionally small and conservative.
- If the homepage treatment works well, expand from these approved files rather than pulling from the full archive.
- If the frontend needs stronger hero imagery later, create a separate hero collection instead of reusing the mosaic set.

## Files intentionally left out of the first pass

- Older portraits that are too small for profile use
- Archive images that are scenic but visibly weak enough to distract at large sizes
- Generic race coverage where the subject is documentary rather than atmospheric
