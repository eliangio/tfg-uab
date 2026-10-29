# TFG 2026/27: first meeting / primera reunión

Quarto (reveal.js) slides for the first meeting with TFG students (Facultat d'Economia i Empresa, UAB).

| Language | Source |
|---|---|
| Español | `index.qmd` |
| English | `index-en.qmd` |

Each title slide links to the other version.

## Files

- `index.qmd`, `index-en.qmd`: the slides. One `##` heading is one slide. Speaker notes are in `::: notes` blocks (press `S` in the browser). Keep both files in sync when you edit.
- `theme.scss`: the look. Based on the *clean* theme by Grant McDermott (MIT licence, notice kept in the file header), plus the extra components of these slides and Roboto embedded as base64.
- `_quarto.yml`: three lines that make Quarto treat both decks as one website project (needed for `quarto publish`).

The rendered HTML is not stored on `main`; it lives on the `gh-pages` branch, which Quarto creates.

## Preview and build

```bash
quarto preview index.qmd      # live preview (use index-en.qmd for English)
quarto render                 # writes _site/index.html and _site/index-en.html (git-ignored)
```

Add `?print-pdf` to the URL and print to PDF from Chrome for a handout.

## Publish

```bash
quarto publish gh-pages --no-prompt
```

This renders both decks and updates the `gh-pages` branch. In the repo settings use *Pages → Build and deploy → Deploy from a branch → `gh-pages` / `(root)`*. The slides are then at `https://<user>.github.io/<repo>/` (Spanish) and `https://<user>.github.io/<repo>/index-en.html` (English).
