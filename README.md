# tvt-site

The website for [tvt (Telemetry Value Tracker)](https://github.com/opsmastery/tvt),
served by GitHub Pages at https://tvt.opsmastery.dev/.

Plain HTML and CSS: no build step, no external fonts or trackers. One small inline script remembers the Dark, Light or Auto theme.

| Path | What |
| --- | --- |
| `index.html` | The home page |
| `404.html` | Not-found page (absolute paths from the domain root) |
| `assets/style.css` | Styles; the palette is at the top |
| `assets/brand/` | Logo, mark and favicon in every variant |
| `assets/report-*.png` | Screenshots of the report on the tvt test lab |
| `assets/social-card.png` | 1200x630 preview image for links shared on LinkedIn and elsewhere |
| `.github/workflows/pages.yml` | Deploys on every push to `main` |

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Publish

Push to `main`. The `pages` workflow checks the pages and deploys them. In the
repo settings, Pages > Build and deployment > Source must be **GitHub Actions**.

## Domain

The site is served at `tvt.opsmastery.dev`. The domain is set in Settings > Pages
(Actions deployments ignore a `CNAME` file), with **Enforce HTTPS** on. DNS at
GoDaddy has a CNAME record `tvt` pointing to `opsmastery.github.io`. The `.dev` TLD
is HTTPS-only in every browser, so the site will not load until the certificate
is issued.

## License

Apache 2.0, the same as tvt.
