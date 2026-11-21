# MAGNA — Shift Work Table

Mobile-first production-plan table for the MAGNA shift workflow.

## Features
- Upload a photo of the production planning screen.
- In-browser OCR using Tesseract.js (the photo is processed in the browser, not uploaded to an application server).
- Editable table with the source columns: Lis, Status, Číslo dielu, MSW, Názov dielu, ID, Poznámky, Vymena, IDPlanovac, MSW_Plan, DielArtikel.
- Separate chronological list of mould changes (Vymena).
- Search, status filtering, manual row entry and deletion.
- CSV import/export, JSON backup, browser-local persistence and print view.

## Run locally
Serve the repository root with a static server, then open `/simulator/` or `/`.

```bash
python -m http.server 8080
```

## OCR limitations
OCR is an assisted first pass, not an authoritative data source. All recognized rows are flagged for manual review. Recognition quality depends on image sharpness, perspective, screen glare and column alignment. Verify every part number, mould/MSW identifier, change time and planner/project value against the original production screen before using the list.

## Privacy and storage
The photo is processed in the browser. The recognized table is saved in localStorage on the current device. Export CSV or download a JSON backup before clearing browser data or changing devices.
