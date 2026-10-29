# TFG 2026/27: first meeting / primera reunión

Quarto (reveal.js) slides for the first meeting with TFG students (Facultat d'Economia i Empresa, UAB).

| Language | Source | Rendered |
|---|---|---|
| Español | `index.qmd` | `docs/index.html` |
| English | `index-en.qmd` | `docs/index-en.html` |

The title slide of each version links to the other one.

## Files

- `index.qmd`, `index-en.qmd`: the slides. One `##` heading is one slide. Speaker notes are in `::: notes` blocks (press `S` in the browser). Keep both files in sync when you edit.
- `custom.scss`: small additions on top of the theme (tables, four-phase layout, evaluation bar, callouts).
- `fonts.scss`: Roboto embedded as base64, so the deck looks the same on every machine (SIL Open Font License, from Google Fonts).
- `_extensions/grantmcdermott/clean/`: the *clean* reveal.js theme by Grant McDermott, MIT licence (see the `LICENSE` file there).
- `docs/`: rendered output, one self-contained HTML file per language, ready for GitHub Pages.

## Editing notes

- Anything marked *(propuesta)* / *(proposal)* in red is the tutor's own suggestion, not a faculty rule: the internal deadlines and the "My rules" column.
- Official dates and rules come from the faculty calendar, the Normativa and the course guide, all linked from the slides.

## Preview and build

```bash
quarto preview index.qmd      # live preview (use index-en.qmd for English)
quarto render                 # writes docs/index.html and docs/index-en.html
```

Add `?print-pdf` to the URL (for example `docs/index.html?print-pdf`) and print to PDF from Chrome for a handout.

## GitHub Pages

*Settings → Pages → Build and deploy → Deploy from a branch → `main` / `/docs`*. The slides are then served at `https://<user>.github.io/<repo>/` (Spanish) and `https://<user>.github.io/<repo>/index-en.html` (English).
