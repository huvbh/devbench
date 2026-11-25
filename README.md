# DevBench

Thirty browser instruments in one HTML file. Hashers, formatters, converters, generators — every one of them runs inside the tab, with no account, no upload and no build step.

Open `index.html` from your disk, or serve it from Pages once the workflow has run.

---

## What is actually inside

Five zones, thirty tools, all wired to real implementations:

| Zone | Tools |
| --- | --- |
| Converters | Base64, URL encode, JSON/YAML, CSV to JSON, timestamp |
| Formatters | JSON, SQL, HTML, CSS, Markdown preview |
| Crypto | SHA-1/256/512, HMAC, UUID v4, JWT decode, bcrypt check |
| Generators | QR code, password, lorem ipsum, slug, colour palette, meta tags |
| Dev utils | Regex tester, text diff, word count, cron builder, fake data, case converter |

Nothing is a placeholder card. Open a tile and the tool works offline in the same tab.

## Why it is a single file

- No `package.json`, no node_modules, no build step. The CSS, the scripts and the tool code are inline.
- Works from `file://`, a USB stick, a static host, or an air-gapped laptop.
- No network requests at runtime — no fonts, no CDNs, no analytics. Open the network tab and it stays empty.
- About 250 KB, and most of it is the thirty tool implementations rather than assets.

## Recolour it

The palette is one block of CSS custom properties at the top of the `<style>` section:

```css
:root{
  --bg:#0A0A0B; --ink:#F1ECE3;
  --accent:#E8A020;        /* buttons, tiles, matrix, scanlines */
  --accent-dim:rgba(232,160,32,.13);
  --hairline:rgba(242,237,228,.085);
}
```

Change `--accent` and every amber element follows. Nothing is hard-coded twice.

## The square matrix

`#bwGrid` holds thirty cells, one per tool, generated from the rendered tool cards at runtime:

- hover a cell, the matching tool card lights up;
- click a cell, the tool opens;
- the legend under the grid explains idle / hover / open.

Renumber or regroup the tools and the wall follows — it reads `data-tool`, not a hard-coded list.

## Deploy

The included workflow publishes the repository root to GitHub Pages:

1. Push to `main`.
2. Repository settings, Pages, Source: **GitHub Actions**.
3. The first run publishes `index.html`.

Any static host works the same way — it is one file.

## Browser support

Chromium, Firefox and Safari, current versions. The stroked headline falls back to solid text where `-webkit-text-stroke` is missing. Motion is reduced automatically under `prefers-reduced-motion`.

## Licence

MIT. Take it, fork it, ship it, sell a version of it — the licence text is in [LICENSE](LICENSE).

If this saved you a build, a star is the cheapest way to say thanks.
