# Byunghoon (David) Kang — Personal Website

Source for my academic homepage, hosted with GitHub Pages.

🔗 **Live site:** https://david-bkang.github.io/

Byunghoon (David) Kang — Associate Professor of Economics, Department of Economics, Lancaster University.
Research in econometric theory and applied econometrics.

## What's here

| File | Purpose |
|------|---------|
| `index.html` | The entire site — a single, self-contained one-page layout (HTML + CSS + a little JavaScript, no build step). |
| `profile.jpg` | Profile photo shown in the header. |
| `README.md` | This file. |

The page is one scrolling layout with sticky navigation: **About → Working Papers & Work in Progress → Publications → Teaching → Contact**, plus Google Scholar / LinkedIn / CV links and expandable "Abstract" and "Stata command" panels.

## How to edit

Everything lives in `index.html`:

- **Text, papers, links** — edit the relevant section directly in the HTML.
- **Add a publication / working paper** — copy an existing `<div class="item">…</div>` block and update the title, authors, date, abstract, and links.
- **Abstracts** — the text sits in `<div class="abstract" hidden>…</div>`; a few say "Abstract coming soon" and are marked with a `<!-- TODO -->` comment.
- **Colors & fonts** — change the CSS variables in `:root` at the top of the `<style>` block (e.g. `--accent`, `--bg`, `--serif`, `--sans`).
- **Photo** — replace `profile.jpg` (a roughly square or portrait headshot works best).

## How to publish

The site auto-deploys on every push to the `main` branch.

```bash
git add -A
git commit -m "Update site"
git push
```

Changes go live at https://david-bkang.github.io/ within about a minute.

GitHub Pages is configured under **Settings ▸ Pages** (Source: *Deploy from a branch*, Branch: `main` / `root`).

## Design notes

- Warm, minimal "classic academic" style: cream background with a rust accent.
- Fonts: **Newsreader** (serif) + **Inter** (sans) via Google Fonts. The font stack requests Anthropic's Tiempos / Styrene first, so self-hosted licensed copies would be picked up automatically if ever added.
- No frameworks or dependencies — just open `index.html` in a browser to preview locally.
