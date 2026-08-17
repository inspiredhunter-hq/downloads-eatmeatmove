# downloads-eatmeatmove

Download landing page for `Downloads.EatMeatMove.com`.

## Deployment

- GitHub target: `inspiredhunter-hq/downloads-eatmeatmove`
- Netlify team: Shared HQ team (`69bfab4d538bd5f02952f64f`)
- Custom domain: `Downloads.EatMeatMove.com`
- Publish directory: repository root

## Required files

Place the approved PDFs in `/downloads/` using these public filenames (matches the live files and the links in `index.html`):

- `Train for Real Life Training Log - Full Colour.pdf`
- `Train for Real Life Training Log - Black and White.pdf`

Do not change these public filenames when replacing a PDF with a later approved version. This keeps published links stable. `index.html` links to these filenames using percent-encoding (e.g. `Train%20for%20Real%20Life%20Training%20Log%20-%20Full%20Colour.pdf`) — if a filename changes, update the corresponding href in `index.html` too.

## Structure

```text
downloads-eatmeatmove/
├── index.html
├── netlify.toml
├── README.md
├── assets/
└── downloads/
    ├── Train for Real Life Training Log - Full Colour.pdf
    └── Train for Real Life Training Log - Black and White.pdf
```

## Local downloads

Both training log PDFs are stored in `/downloads/` and served directly by Netlify. This avoids Google Drive permission errors.
