# Simple POS — GitHub Pages / iPad

This is a small offline-first POS web app designed for iPad use.

## Features
- Current sales and cart
- Open/unpaid orders
- Record payment method: EFTPOS, Cash, Bank transfer, Other
- Daily Transactions Log with selectable previous dates
- End-of-day report with purchases, payment methods and totals
- Print / Share daily reports using the iPad print/share interface
- Reports covering average order value, sales, orders, items sold, top-selling items, payment breakdown and daily performance
- Add, edit, hide and show menu items
- Local JSON backup and restore
- No external libraries or internet connection required after initial caching

## Important
This app RECORDS EFTPOS payments. It does not process card payments or control an EFTPOS terminal.

Sales are stored locally in the browser on the iPad. Export backups regularly.

## GitHub Pages
Upload `index.html`, `manifest.json`, and `sw.js` to the root of a GitHub repository.
Then go to Settings -> Pages -> Deploy from branch -> `main` -> `/ (root)`.

Open the resulting GitHub Pages URL in Safari on the iPad. Once loaded, use Safari Share -> Add to Home Screen and enable Open as Web App.

For a later code update, keep the files together. The service-worker cache version is `simple-pos-v2`; increment it for future releases (v3, v4, etc.) so old cached files are replaced.
