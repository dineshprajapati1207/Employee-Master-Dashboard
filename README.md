# Employee Master Data Dashboard

Static web app (single `index.html`, no build step).

- Upload many employee info files (.xls or .xlsx) at once (filename = Emp Code, e.g. `0001.xlsx`, `1001.xls`)
- New code = added; existing code = replaced; no duplicates; per-file delete
- Master Sheet template is built in (`template/Master_Sheet.xlsx` is a reference copy)
- Export all data to Excel in the Master Sheet format

## Deploy on Vercel
1. Push this folder to a **private** GitHub repo.
2. vercel.com > Add New > Project > import the repo.
3. Framework preset: **Other**. Build command: none. Output directory: leave empty (root).
4. Deploy.

## Important
Employee records are stored in the browser (IndexedDB) of the device you use. They are not sent to any server,
and are not shared between browsers or devices. Export to Excel regularly as your backup.
Protect the site (Vercel project > Settings > Deployment Protection) because it handles personal data.
