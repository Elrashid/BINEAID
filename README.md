# BINEAID — Paper Library

Static reading site for a higher-education research corpus (211 papers,
5 with Arabic translations).

- **paper_reader.html** — ADHD-friendly reader (bionic text, dyslexia font, focus
  mode, read-aloud, EN↔AR toggle). Reads `papers_md/`, `papers_md_ar/`, `figures/`.
- **csv_viewer.html** — sort/filter the bibliographic index in `data/`.

## Run locally
The reader fetches files, so serve over http (not file://):

```
python -m http.server 8000
# open http://localhost:8000/
```

## Deploy
Pushed to GitHub Pages by `.github/workflows/deploy.yml` on every push to `main`.

> Source PDFs and conversion notebooks are intentionally NOT included.
