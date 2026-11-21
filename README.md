# DiscTrace website

A static site: three pages, one stylesheet and a folder of graphics. No build step and no JavaScript.

## Files

| File | What it is |
| --- | --- |
| `index.html` | Homepage |
| `smart-tag.html` | Smart tag details |
| `simulator.html` | Simulator details |
| `styles.css` | Colours, type and layout for every page |
| `assets/` | Logo, favicon and illustrations (all SVG) |

## Before you publish

1. **Checkout link.** Search all three pages for `#CHECKOUT-LINK` and replace it with your real checkout address. It appears once per page, in the yellow buy section. Every other "Buy the tag" button scrolls to that section.
2. **Contact email.** In `index.html`, replace `hello@example.com` and the placeholder text beside it with your real address.
3. **Placeholders.** Search for `Placeholder:` to find every spot that needs a real fact (specs, shipping, returns, supported phones, net and space, your story). Each one shows on the page as a dashed yellow tag. Replace the whole `<span class="ph">…</span>` with your text.

## Swapping graphics for photos

Each illustration is an `<img>` tag pointing at a file in `assets/`. To use a photo, add it to `assets/` and change the `src` (and the `alt` description) on that tag.

The app screen graphic (`assets/app-stats.svg`) shows `00` for every number on purpose. Replace it with a real screenshot when you have one, then remove the placeholder tag under it.

## Logo

- `assets/logo-mark.svg`: the mark on its own (dark, for light backgrounds)
- `assets/logo-mark-light.svg`: the mark for dark backgrounds
- `assets/logo.svg`: mark plus wordmark. The wordmark uses the free Archivo font.
- `assets/favicon.svg`: browser tab icon

## Publishing

Upload the whole folder, keeping the structure, to any static host (Netlify, Cloudflare Pages, GitHub Pages or ordinary web hosting). `index.html` must sit at the top level. The `.claude` folder is only for local previewing and does not need to be uploaded.

The site loads the Archivo font from Google Fonts. If that is ever unavailable, the pages fall back to the visitor's system font.
