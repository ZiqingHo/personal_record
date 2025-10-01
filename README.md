# Literature Review Manager

A single-file, local & private web app to collect, search, and export your literature notes. Supports LaTeX via MathJax.

## Features

- Add/Edit entries with **Year, Venue, Title, Authors, Keywords, Method, Contribution, Summary**
- Search, sort (by year/title), and filter by **year range**
- LaTeX rendering with MathJax (`$inline$`, `$$display$$`)
- Local-first: data stored in `localStorage` (no backend)
- Import from JSON, Export to **JSON** or **CSV** (Excel-friendly)

## Usage

1. Open `index.html` in your browser (double-click is fine).
2. Fill the form and click **Save Entry**.
3. Use the **Library** toolbar to search, sort, filter by year, and export/import.

> Tip: Keywords are comma-separated and render as tags.

## Data format

JSON entries are shaped like:

```json
{
  "id": "id_abc123",
  "createdAt": 1710000000000,
  "updatedAt": 1710000001000,
  "year": 2024,
  "venue": "Journal/Conference",
  "title": "Paper title",
  "authors": "First A., Second B.",
  "keywords": ["gp", "variational"],
  "method": "Sparse GP",
  "contrib": "Bullet or paragraph text",
  "summary": "Free text; LaTeX allowed"
}
```

