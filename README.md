# tvt-site

The website for [tvt (Telemetry Value Tracker)](https://github.com/Opsmastery-Summit/tvt),
served by GitHub Pages at https://opsmastery-summit.github.io/tvt-site/.

Plain HTML and CSS: no build step, no external fonts or trackers. One small inline script remembers the Dark, Light or Auto theme.

| Path | What |
| --- | --- |
| `index.html` | The home page |
| `404.html` | Not-found page (paths are absolute to `/tvt-site/`) |
| `assets/style.css` | Styles; the palette is at the top |
| `assets/logo.svg` | Logo and favicon |
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

## Custom domain later

Add a `CNAME` file with the domain, copy it into `_site` in the workflow, set the
domain in Settings > Pages, and update the URLs in `index.html`, `robots.txt` and
`sitemap.xml`. Paths in `404.html` assume the `/tvt-site/` prefix and change to `/`.

## License

Apache 2.0, the same as tvt.
