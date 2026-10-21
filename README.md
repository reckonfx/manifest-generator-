# Direct USA Manifest Generator

Single-page form that builds Direct USA courier manifests from HAWB / commodity entries.

- **Download CSV** — 54-column Direct USA manifest CSV (UTF-8 BOM, CRLF).
- **Download Manifest Excel** — `.xlsx` in the same layout as the carrier's sample manifest
  (filter on column A showing only `hawb` rows; commodity rows kept but hidden).
- Declared value: split a manifest total across HAWBs, or enter value per HAWB.
  Item values are split randomly (or by quantity) and always add up exactly to the HAWB value.
- HTS code suggestions from previously used codes, plus live search on hts.usitc.gov.
- Import an existing manifest CSV; fixes Excel-damaged ZIP codes.

Runs entirely in the browser — no server, no install. Open `index.html`, or enable
GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

Data is saved in the browser's local storage only.
