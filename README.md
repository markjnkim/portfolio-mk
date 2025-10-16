# Mark Kim — Static Portfolio Site

This is a static, production-ready portfolio site (HTML/CSS/JS). It includes resume & cover letter PDFs, portfolio links, SEO metadata, and accessible, responsive design.

## Quick Start (Local)
Python 3.x is already enough to serve this site locally:
```bash
cd mark_kim_site
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy Options

### GitHub Pages
1. Create a new repo, e.g., `mark-kim-portfolio`.
2. Upload the contents of this folder.
3. In **Settings → Pages**, set Source to **main** branch, root (`/`).
4. Your site will be live at `https://<username>.github.io/mark-kim-portfolio/`.

### Netlify
- Drag & drop this folder in the Netlify UI, or run:
```bash
netlify deploy --prod --dir .
```

### Vercel
```bash
vercel . --prod
```

### CloudFront / S3 (AWS)
- Upload files to an S3 bucket, enable static hosting, and set index to `index.html`.
- Put CloudFront in front for HTTPS and global caching.

## Where to update
- **index.html** — content, sections, links.
- **assets/css/styles.css** — theme & layout.
- **assets/js/main.js** — basic scripts.
- **assets/docs** — resume/cover letter PDFs.

## SEO
- The `<head>` includes Open Graph tags and JSON-LD for rich search results.
- Update the `"url"` property in `index.html` JSON-LD after deployment.

## Notes
- PDFs included: `Mark_Kim_Resume.pdf`, `Mark_Kim_Cover_Letter.pdf` (in `assets/docs/`).
- Replace placeholder images under `assets/img/` as needed.
