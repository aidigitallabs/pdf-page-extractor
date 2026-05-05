# PDF Page Extractor

Drop a PDF, get a contact sheet of every page as an image — and a ZIP of individual page PNGs. Runs entirely in your browser — no upload, no signup, nothing leaves your device.

- PDF in, PNG / JPEG / WEBP pages out.
- Render every page, or pick a range (`1-5`, `1,3,5-8`).
- Pick DPI (72 / 144 / 200 / 300) and an optional max-width clamp.
- Single-page download per tile, or full ZIP of the batch.

Sister tool to [Frame Generator](https://frames-generator.com/) — same spec-sheet aesthetic, same trust story, same in-browser pipeline.

## Run locally

```
node serve.mjs
```

Then open `http://localhost:4181/`.

## Stack

Single-file static HTML + inline JS. `pdf.js` and JSZip are loaded from CDN on demand. No build step — `serve.mjs` is just a tiny static server for local development. The deployed site is plain static hosting.
