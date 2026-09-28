# AM Trades — Journal & Dashboard

A single-page trading journal, pre-trade checklist, and analytics dashboard built around the **AM Trades 3-Step** framework (Framework → Confirmation → Entry).

## Features

- **Pre-Trade Checklist (hard gate)** — 19 checks across Steps 1/2/3 plus setup classification. The trade log stays locked until the setup is fully aligned. Large-wick reversal days are auto-flagged as skips.
- **Journal** — Full-template trade entries with auto-calculated R multiple, plus dedicated "skipped day" logging (discipline is tracked as a positive outcome).
- **Analytics** — Win rate, profit factor, expectancy, avg winner/loser, current streak, max drawdown, equity curve, and win-rate breakdowns by profile, scenario, daily-candle type, divergence, and day of week. Toggle between R multiples and $ P&L.
- **Discipline metrics** — Rule adherence rate and correctly-skipped days, weighted equally.
- **Export / Import** — CSV track record (investor-ready) and JSON backup/restore.

## Data storage

All data is stored in the browser's `localStorage`, scoped to the deployment origin. It persists across sessions on the same browser. Use **Backup (JSON)** regularly and **Export CSV** to hand a clean track record to a third party. No data leaves the browser.

## Tech

- Single self-contained `index.html` (inline CSS + JS)
- [Chart.js](https://www.chartjs.org/) via CDN for visualizations
- No build step — static hosting

## Local use

Open `index.html` in any modern browser, or serve the folder with any static server.

## Deployment

Deployed as a static site on Vercel.
