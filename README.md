# Verko — Portfolio

Static site, no build step, no framework. Upload every file in this folder to the root of a GitHub repository.

## Publish with GitHub Pages
1. Create a public repository on github.com and upload all files (Add file > Upload files > Commit changes).
2. Settings > Pages > Build and deployment: Deploy from a branch, branch `main`, folder `/ (root)`, Save.

## Custom domain
1. Settings > Pages > Custom domain: enter your domain, Save (GitHub creates a `CNAME` file), then tick Enforce HTTPS.
2. At your domain registrar add DNS records: four `A` records for the root domain pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`, and a `CNAME` for `www` pointing to `YOUR-USERNAME.github.io`.

The custom 404 page (`404.html`) links to `/`, so it works correctly on a custom domain at the root.

## Files
- `index.html` — the site (title, description, structured data, one `<h1>`).
- `404.html`, `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest`, `og-image.png`.
- `fonts/` — Awesome Serif (Light, Medium, Bold) for headlines. Body text uses SF Pro on Apple devices and falls back to Inter Tight elsewhere.
- `robots.txt`, `llms.txt`, `poster1-8.jpg` and `clip1-8.mp4` (work previews).

Titles, captions and links are plain text in `index.html`.
