# Blobs live here

This `blobs/` folder is home to large files - images and documents -
used in the SHR web site. During site build, the contents of `blobs/`
is not copied or even looked at by the site builder. Instead, the site
builder works with references to their location in GitHub and
downloads the files from there when viewing. It's much faster to build
that way (and the static site is way smaller and faster to load), but
does miss out on the fancy screen-aware image pre-processing that
would otherwise be available. Them's the breaks.

The folder organisation should be fairly obvious - `races` for race
images, `documents` for PDFs of committee meetings etc. and
`portraits` for individuals looking their best exhausted, muddy
selves.

Having a file uploaded to here _is not sufficient_ for it to appear in
the web site. To be seen by the site builder it must appear in a
"collection" in the main body of the repository. Collections are YAML
files with paths to the blob along with various metadata. The format
varies by collection, and is expected to evolve as we get a better
handle on what meta-data is useful. Currently the following
collections exist:

- `homepage/images.yaml` - images for decorating the landing page
- `committee/portraits.yaml` - dashing pictures of committee members
- `documents/manifest.yaml` - boring stuff
- `races/<raceId>/images.yaml` - race gallery and hero images

A large number of images imported from the legacy SHR web site have
not yet been classified. They all live in `blobs/unclassified`. Many
of these are race images, some have meaningful names, but many do
not. Help in classifying them is welcome! This will involve:

1. Renaming the image into the appropriate `blobs/races/<raceId>/`,
   `blobs/documents/` or `blobs/portraits/` folder
2. Updating the corresponding collection YAML.

It might be worth checking the admin app before you get stuck in as we
have been planning to add a management page to make this a bit easier.

- John Hamer, 2 May 2026.
