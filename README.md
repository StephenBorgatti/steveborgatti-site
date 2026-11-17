# steveborgatti.com

Personal academic site, built with [Quarto](https://quarto.org) and published to GitHub Pages at <https://steveborgatti.com>.

## Everyday edits

| To change… | Edit |
|---|---|
| Home page / bio | `index.qmd` |
| Research statement | `research.qmd` |
| A publication | `data/publications.toml` (never `publications.qmd`, which is generated) |
| A paper's PDF | put it in `papers/` and set `pdf = "file-name.pdf"` on its entry |
| The CV | export from Word to `cv/Borgatti-CV.pdf` |
| Teaching, software, tools | `teaching.qmd`, `software.qmd`, `tools.qmd` |
| Menu, theme, footer | `_quarto.yml`, `assets/styles.scss` |

## Preview locally

```
quarto preview
```

This regenerates the publications page, builds the site, and opens it in a browser. It reloads as you save.

## Publish

Commit and push to `main`. The GitHub Action in `.github/workflows/publish.yml` builds the site and deploys it to GitHub Pages; it is live a minute or two later.

## Notes

- PDF file names in `papers/` are permanent URLs (`steveborgatti.com/papers/<name>`), so don't rename them once published.
- `papers/dissertation.pdf` keeps the address that old links already use.
