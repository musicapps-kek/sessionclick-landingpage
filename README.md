# sessionclick.com

Landing page for the SessionClick app. Built with Hugo, deployed via GitHub Pages.

## Local development

```bash
hugo server -D
```

Open http://localhost:1313.

## Build

```bash
hugo --minify
```

Output goes to `public/`.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds with Hugo and publishes to GitHub Pages.

## Custom domain

`static/CNAME` contains `sessionclick.com` — copied into the build output so GitHub Pages serves the custom domain.

## Structure

- `hugo.toml` — site config
- `content/` — Markdown content (home index, Impressum, Datenschutz)
- `layouts/` — HTML templates (`index.html` is the landing page)
- `assets/css/main.css` — stylesheet (processed by Hugo Pipes, fingerprinted)
- `static/` — files copied verbatim to the build (images, favicon, CNAME)

## To do before launch

- Fill in `content/impressum.md` (name, address, optional USt-IdNr.)
- Fill in `content/datenschutz.md` (name, address — same as Impressum)
- Set `playStoreUrl` in `hugo.toml` once the Play Store listing is live
- Add the official Google Play badge PNG to `static/images/google-play-badge.png`

--
