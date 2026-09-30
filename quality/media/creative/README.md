# MAOS P05 — Creative Media

This folder is the controlled media layer for the **AI Creative & Multimedia Applications** section of the Quality portfolio.

## Safe structure

- `media-manifest.json` is the single source of truth for project-to-media mapping.
- `project-viewer.html` reads a project id from the URL and resolves it through the manifest.
- Published media files use stable semantic names rather than upload names.
- Reserve/original files are not linked publicly until selected and QA-approved.
- CV files (`cv-ar.pdf`, `cv-en.pdf`) are outside this media layer and must not be modified by P05 media work.

## Future maintenance

To add a project: upload the approved media asset, add one project object to `media-manifest.json`, and add/link its portfolio card.

To replace media without changing the public project identity: keep the project `id`, update `publishedFile`, then run link/media/mobile QA.

To remove a project: remove or archive its card first, then remove its manifest entry after confirming no remaining links depend on it.

This design intentionally supports future addition, deletion, replacement, and expansion without restructuring the portfolio.
