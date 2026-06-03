# AI CSV Viewer Online

**Free, private, browser-based CSV file viewer.**

Live at → **[ai-csv-viewer-online.github.io](https://ai-csv-viewer-online.github.io)**

No uploads. No server. Your files never leave your browser.

---

## Features

- **Drag & drop or browse** — drop a file anywhere on the page or use the file picker
- **Auto-detects delimiter** — comma, semicolon, tab, and pipe-delimited files all work
- **Header row toggle** — enable or disable the first-row-as-header setting per file
- **Column sorting** — click any column header to sort ascending / descending
- **Global search** — filters across all columns instantly
- **Per-column filters** — dropdown filter for each individual column
- **Pagination** — configurable rows per page (25 / 50 / 100 / 500)
- **Row selection** — select individual rows or use select-all; copy only selected rows
- **Export to CSV** — downloads filtered + sorted data as a CSV file
- **Export to JSON** — downloads filtered + sorted data as JSON
- **Copy to clipboard** — copies selected rows (or current page) as TSV
- **Column visibility toggle** — show/hide individual columns
- **Column resizing** — drag column borders to resize
- **Dark / light mode** — toggle in the header, preference is saved
- **File metadata** — shows file name, size, row count, column count, and detected delimiter
- **Handles large files** — tested with 50,000+ row files via PapaParse streaming

## Supported File Formats

| Format | Extension | Delimiter |
|---|---|---|
| CSV | `.csv` | Comma `,` |
| TSV | `.tsv` | Tab |
| Semicolon-separated | `.csv` | Semicolon `;` |
| Pipe-separated | `.txt` / `.csv` | Pipe `\|` |

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | Tailwind CSS (CDN) |
| Logic | Vanilla JavaScript (ES2020) |
| CSV Parsing | [PapaParse 5.4](https://www.papaparse.com/) (CDN) |
| Hosting | GitHub Pages |

Single-file app (`index.html`) — no build step, no Node.js, no dependencies to install.

## Local Development

```bash
# Clone the repo
git clone https://github.com/ai-csv-viewer-online/ai-csv-viewer-online.github.io.git
cd ai-csv-viewer-online.github.io

# Open in browser (any static server works)
npx serve .
# or just open index.html directly in Chrome/Firefox
```

No build step required. Edit `index.html` and refresh.

## Deployment

Pushes to `main` are automatically deployed by GitHub Pages.
The `.nojekyll` file prevents GitHub Pages from running a Jekyll build.

## Contributing

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Make your changes in `index.html`
4. Test in Chrome, Firefox, and Safari
5. Open a pull request

Please keep the app as a single `index.html` file with CDN-only dependencies.

## Roadmap

- [ ] AI CSV Q&A via Claude API (Phase 2)
- [ ] Companion tools: JSON Viewer, TSV Viewer
- [ ] Freeze/pin columns (not just header row)
- [ ] Excel (.xlsx) support
- [ ] Chart / visualization panel

## License

MIT © [Babar Aslam](https://github.com/BabarAslamm)
