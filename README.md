# Scottish Hill Runners Content Repository

This repository stores editorial content for Scottish Hill Runners.

A companion repository, `site-builder` constructs a static web site
for the contents, and should be re-deployed after any content changes.

The admin app at <https://admin.scottishhillrunners.uk> creates pull requests against this repository for:

- News posts
- Uploading and correcting race results
- Race information
- Calendar updates
- Image uploads
- Club information
- Long distance challenge information

## Repository layout

- news/
  - One markdown file per news post
  - Each post is filed by year
  - File name pattern: YEAR/YYYY-MM-DD[-suffix].md
- races/
  - One folder per race
  - Each race folder contains:
    - index.md (race metadata in markdown format)
    - YEAR.csv files (results data)
- clubs/
- info/
- long-distance/

## News

Path pattern:

- news/2026/2026-03-29.md
- news/2026/2026-03-29-2.md

News file format:

```md
---
title: Spring Championships Announced
date: 2026-03-29
excerpt: Key dates and race details for this season.
---

Markdown body content goes here.
```

Rules:

- date should use YYYY-MM-DD
- Use -suffix only when multiple posts share the same date.
  This will usually be inserted automatically, based on existing content.
- Keep excerpt concise for listing pages

## Race descriptions

Path pattern:

- races/Carnethy5/index.md

Race index format:

```md
---
title: Carnethy 5
venue: Pentland Hills
distance: 10
climb: 760
maleRecord: 39:00
femaleRecord: 45:30
nonBinaryRecord:
web: https://example.org/carnethy-5
organiser: Carnethy Club
---

Markdown race description and event notes go here.
```

Distance and climb must be in metric units; the UI will convert to imperial when requested.

## Race results

Path pattern:

- races/Carnethy5/2026.csv

CSV rules:

- File must be valid CSV
- Header names and required columns must match SHR validation rules used by the admin app
- Keep values clean and consistently formatted; e.g. times should be hh:mm:ss, without omitting leading 0s.

## Editorial workflow

1. Open or create content in the admin app
2. Submit draft changes
3. Admin app opens a pull request against this repository
4. Review, discuss, and merge in GitHub

## Pull request guidance

Please include:

- What changed
- Why it changed
- Any source links or notes for reviewers

## Branch and merge policy

- Default branch: main
- Changes should be merged via pull request
- Avoid direct commits to main

## Ownership

Maintained by the Scottish Hill Runners association and hill running community.
