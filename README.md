# eportal-demo

Static demo of the **MAVIVO Tender ERP** cockpit — powered by EverTrust.

A single self-contained page (no build step, no framework) served on Vercel.

## Files

- **`index.html`** — the demo UI (dashboard, tender pipeline, contract awards, competitors, buyers, search).
- **`mavivo_mock_data.js`** — the data layer, loaded by the page:
  - `MEDICAL_TENDERS` — the MEDICAL niche from the live eCore catalog.
  - `BUYERS` — the real contracting authorities behind those tenders (from TED).
  - `AWARDS` — recent real German medical-supply contract awards (from TED).
  - `COMPETITORS` — market-research dossier (not from eCore).

## Deploy

Zero-config static deployment: Vercel serves `index.html` at the root and
`mavivo_mock_data.js` alongside it. No build command or output directory needed.
