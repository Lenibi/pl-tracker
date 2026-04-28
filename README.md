# SOXL P&L Tracker

Quick web app showing live mark-to-market P&L for a SOXL option position, in CAD.

**Live demo:** https://lenibi.github.io/soxl-pnl-tracker/

## What it does

- Fetches live SOXL price and USD/CAD rate via Yahoo Finance (through a public CORS proxy)
- Computes option mark using Black-Scholes with adjustable IV
- Shows P&L in both USD and CAD
- Auto-refreshes on load; manual refresh button

## Position (hardcoded for fun)

- 6 contracts SOXL May01 $110C
- Avg fill: $6.26 USD
- Total cost: $3,754 USD

To change the position, edit the constants at the top of the `<script>` block in `index.html`.

## Hosting on GitHub Pages

1. Push to `main` branch
2. Settings → Pages → Source: `Deploy from a branch`, Branch: `main`, Folder: `/ (root)`
3. Wait ~30 seconds, site goes live at `https://<username>.github.io/<repo-name>/`

No build step. Pure static HTML + vanilla JS.
