# IOARTS

IOARTS is a static gallery of digital illustrations and gaming fan art. The site is built from HTML and CSS, with artwork and page assets stored in the repository.

## Features

- Featured artwork and an image gallery linking to the artist's portfolio
- About, contact, terms of sale, privacy, and copyright pages
- Responsive page styles, favicons, and a web app manifest
- Search metadata, structured data, `robots.txt`, and a sitemap
- Vercel configuration for clean URLs, redirects, and response headers

## Technology

- HTML and CSS
- WebP and PNG image assets
- Vercel static hosting

There is no package manifest, dependency installation, or build step.

## Run locally

Use Python 3 (or another static HTTP server) from the repository root:

```bash
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). For pages that use clean URLs on Vercel, use the corresponding `.html` filename locally (for example, `/about-me.html`).

## Project structure

| Path | Purpose |
| --- | --- |
| `index.html` | Home page and artwork gallery |
| `about-me.html`, `contact.html` | About and contact pages |
| `terms-of-sale.html`, `privacy-policy.html`, `copyright-attribution.html` | Legal and policy pages |
| `shared.css`, `home.css`, `pages.css` | Shared, home-page, and content-page styles |
| `*.webp`, `*.png` | Artwork, favicon, and touch-icon assets |
| `manifest.json` | Web app metadata and icons |
| `robots.txt`, `sitemap.xml` | Search crawler configuration |
| `vercel.json` | Hosting, URL, redirect, and response-header configuration |
| `CNAME` | Custom-domain record |

## Deployment

Deploy the repository as a static site on Vercel. No build command or environment variables are required; serve the repository root as the output directory and keep `vercel.json` with the deployment so its URL and header configuration is applied.
