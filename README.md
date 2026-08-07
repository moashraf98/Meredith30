# Replit export - local / GitHub Pages version

This package was created from the supplied single-file Replit export.

## What changed
- Extracted 13 Base64 JPEG images from the HTML into `assets/images/`.
- Replaced the embedded Base64 image constants with normal relative file paths.
- Removed the original `./favicon.svg` tag because `favicon.svg` was referenced by the export but was not included in the supplied file.
- Left the tiny inline SVG noise texture embedded in the HTML.
- Google Fonts are still loaded from `fonts.googleapis.com` / `fonts.gstatic.com`.

## Run locally
From this folder:

```bash
python -m http.server 8000
```

Then open:

http://localhost:8000

## GitHub Pages
1. Create a GitHub repository.
2. Upload everything in this folder, keeping the same folder structure.
3. Commit to your main branch.
4. Go to Settings -> Pages.
5. Under Build and deployment, choose "Deploy from a branch".
6. Select the `main` branch and `/ (root)`.
7. Save.

The entry page is `index.html`.
