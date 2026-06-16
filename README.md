# sebneu.github.io

Personal website of Sebastian Neumaier — [sebneu.github.io](https://sebneu.github.io/).

A minimal **static** site (plain HTML + one stylesheet, no build step, no Jekyll).

## Structure

| File | Purpose |
| --- | --- |
| `index.html` | About, news, research, selected publications, projects, teaching, service |
| `publications.html` | Full publication list with per-entry *Cite* (Copy BibTeX) buttons |
| `publications.bib` | All publications as BibTeX — the single source of truth for citations |
| `documents.html` | Browsable overview of archived talk slides, posters and paper PDFs |
| `files/` | Uploaded documents migrated from WordPress, mirroring `wp-content/uploads/YYYY/MM/` |
| `archive/` | Raw archive of the old WordPress posts/pages (JSON + readable HTML), not linked from the site |
| `style.css` | Shared stylesheet (light + dark theme via `prefers-color-scheme`) |
| `favicon.svg` | Site icon |

## Adding a publication

1. Add the BibTeX entry to `publications.bib`.
2. Add a matching `<li data-bib="YOUR_KEY">…</li>` to `publications.html`.
   The *Cite* button is wired up automatically by matching `data-bib` to the BibTeX key.

## Notes

- `.nojekyll` disables Jekyll processing so the site is served as-is — **keep it**.
  It is also required for GitHub Pages to publish the `.well-known/` directory
  (which holds the Tesla third-party app public key).
