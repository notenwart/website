# notenwart – website

One static page for [notenwart](https://github.com/notenwart/notenwart) at [notenwart.app](https://notenwart.app): no
build step, no framework, no external resources (no fonts, scripts or embeds from other servers), no cookies, no
tracking. English. A [falkOSS](https://falkoss.org) project.

| Path | What |
|---|---|
| `index.html`, `style.css`, `404.html` | the page |
| `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest`, `social.png` | head icons – **generated** in [notenwart/brand](https://github.com/notenwart/brand) (`web/`), copied here |
| `assets/` | lockups and marks from `notenwart/brand` (`svg/`) |
| `.well-known/security.txt`, `robots.txt` | contact for security reports; crawlers welcome |

Imprint and privacy policy are falkoss.org's – same operator, one place to keep them current.

Preview locally:

```sh
python3 -m http.server 8020
```

## Publishing

GitHub Pages via `.github/workflows/pages.yml` on every push to `main` (Settings → Pages → Source: **GitHub
Actions**). The custom domain notenwart.app lives in the repository settings, not in a `CNAME` file. CI checks REUSE
and the DCO sign-off with the shared workflows of falkoss/starterpack, pinned by commit. `security.txt` expires
2027-10-29 – renew it before.

## Licence

The site's code is **AGPL-3.0-or-later** (`LICENSE`); the brand's artwork (favicons, icons, `social.png`, `assets/`)
is copied from `notenwart/brand` under CC BY-ND 4.0, and the brand itself (name, logo, marks) is not covered by any
licence.
