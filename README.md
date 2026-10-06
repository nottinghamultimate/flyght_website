# flyght_website

Website for Flyght Ultimate (Nottingham), built with [Astro](https://astro.build) and deployed to GitHub Pages.

## Development

```
npm install
npm run dev      # local dev server
npm run build    # static build into dist/
```

## Structure

- `src/pages/` – one file per page (`/`, `/what-is-ultimate/`, `/news/`, `/documents/`, `/contact/`, 404)
- `src/layouts/BaseLayout.astro` – shared `<head>` (SEO, Open Graph, JSON-LD), header and footer
- `src/data.ts` – club details and document links, used by the header, footer and pages
- `src/assets/` – images; processed to optimised WebP at build time
- `public/` – `CNAME`, `robots.txt`, favicon

## Deployment

Pushing to `main` runs `.github/workflows/deploy.yml`. In the repo settings, **Pages → Source** must be set to **GitHub Actions**.
