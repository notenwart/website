# notenwart website

Static one-page site for [notenwart](https://github.com/notenwart/notenwart), deployed to GitHub Pages by
`.github/workflows/pages.yml` on every push to `main`, under the custom domain in `CNAME`.

No build step, no framework, no external resources (no fonts, scripts or embeds from other servers), no cookies, no
tracking. English; imprint and privacy policy are falkOSS's (linked in the footer).

| Path | What |
|---|---|
| `index.html`, `style.css` | the page |
| favicons, `icon-*.png`, `site.webmanifest`, `assets/` | copied from `notenwart/brand/` (edit `brand/generate.py` there, regenerate, copy here) |

Preview locally:

```sh
python3 -m http.server 8020
```

All paths are relative, so the site also works at `https://notenwart.github.io/website/`.

Licence: the site's code is AGPL-3.0-or-later (`LICENSE`); the brand (name, logo) is not covered by it – see
`notenwart/brand/README.md`.
