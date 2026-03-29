# Scottish Hill Runners Content Repository

This repository stores editorial content for Scottish Hill Runners.

The admin app at https://admin.scottishhillrunners.uk creates pull requests against this repository for:

- News posts
- Race index files
- Race results CSV files

## Repository Layout

- news/
  - One markdown file per news post
  - File name pattern: YYYY-MM-DD[-suffix].md
- races/
  - One folder per race
  - Each race folder contains:
    - index.md (race metadata and markdown description)
    - YEAR.csv files (results data)
- clubs/
- info/
- long-distance/

## News Content

Path pattern:

- news/2026-03-29.md
- news/2026-03-29-2.md

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
- Use -suffix only when multiple posts share the same date
- Keep excerpt concise for listing pages

## Race Index Content

Path pattern:

- races/Carnethy5/index.md

Race index format:

```md
---
title: Carnethy 5
venue: Pentland Hills
distance: 6 miles
climb: 2500 ft
maleRecord: 39:00
femaleRecord: 45:30
nonBinaryRecord:
web: https://example.org/carnethy-5
organiser: Carnethy Club
---

Markdown race description and event notes go here.
```

## Race Results Content

Path pattern:

- races/Carnethy5/2026.csv

CSV rules:

- File must be valid CSV
- Header names and required columns must match SHR validation rules used by the admin app
- Keep values clean and consistently formatted

## Editorial Workflow

1. Open or create content in the admin app
2. Submit draft changes
3. Admin app opens a pull request against this repository
4. Review, discuss, and merge in GitHub

## Pull Request Guidance

Please include:

- What changed
- Why it changed
- Any source links or notes for reviewers

## Branch and Merge Policy

- Default branch: main
- Changes should be merged via pull request
- Avoid direct commits to main

## Ownership

Maintained by Scottish Hill Runners editors and maintainers.
