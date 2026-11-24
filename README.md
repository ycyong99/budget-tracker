# Budget Tracker

A daily expense and income tracker that runs as an installable web app (PWA). One HTML file holds the whole app.

## Privacy

- Entries are stored only in the browser on your device (localStorage). Nothing is sent to a server.
- This repository holds no personal figures. Budgets, categories and auto-post items load from a private setup file that you import in **Settings › Restore / import setup**. Do not commit that file: `.gitignore` excludes all `.json` files.

## Features (v1)

- Today: day-to-day spend left against a pace line, pending auto-posts (confirm, edit, skip), today's entries, repeat buttons.
- Add entry: expense, income or transfer; category and sub-category; frequency (One-time, Monthly, Quarterly, Half-yearly, Yearly); payment method; trip name for holidays; note.
- Month: budget vs actual by category with near-limit and over-budget labels, lump-sum bills with due months, income and net cash flow.
- Records: search and filter, edit, delete with undo.
- Export: Excel (.xlsx: Transactions, Monthly summary, Income) and CSV. Backup and restore as JSON.
- Works offline after the first visit. Two-column layout on wide screens (foldable inner screen, tablet, PC).

## Files

| File | Purpose |
|---|---|
| `index.html` | The app |
| `manifest.webmanifest` | Install details (name, icons, colours) |
| `sw.js` | Offline cache. Change `VERSION` on each release so phones pick up the update |
| `icons/` | App icons |

## Hosting

GitHub Pages: Settings › Pages › Source: Deploy from a branch › `main` / root.
