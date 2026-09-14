# Simple POS for iPad

Free, offline-first browser POS. Upload these files to a GitHub repository and enable GitHub Pages.

## Files
- `index.html` — complete app
- `sw.js` — offline cache/service worker
- `manifest.json` — iPad web-app metadata

## Features
- Touch-friendly sales screen
- Orders and saved unpaid/open orders
- Payment recording: EFTPOS, Cash, Bank transfer, Other
- Daily transaction log with purchased items, payment method and totals
- Print/share-ready daily report via iPad print sheet
- Editable menu items and categories
- Reports: sales, order count, average order, items sold, top-selling items, payment breakdown and daily performance
- Local storage on the iPad
- JSON backup/export and restore/import

## Important
This is a record-keeping POS. It does **not** process card/EFTPOS transactions. The EFTPOS transaction is completed on the separate EFTPOS terminal, then recorded in the app.

Data is stored locally in the browser on the device. Export backups regularly.

## Updating
If a future version appears stuck on the old version, change the `CACHE` value in `sw.js`, e.g. `simple-pos-v2`, then upload the updated files. This forces a new service-worker cache.
