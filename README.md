# P&L Tracker

Minimalist web app showing live mark-to-market P&L in CAD.

**Live demo:** https://lenibi.github.io/pl-tracker/

## What it does

- Fetches a live price + USD/CAD rate via Yahoo Finance (through a public CORS proxy)
- Computes a Black-Scholes mark with adjustable IV
- Displays one big number, color-coded green/red

## Hosting on GitHub Pages

1. Push to `main`
2. Settings → Pages → Source: `Deploy from a branch`, Branch: `main`, Folder: `/ (root)`
3. Wait ~30 sec
4. Live at `https://<username>.github.io/<repo-name>/`

Pure static HTML + vanilla JS. No build step.

## Customizing

Edit the constants at the top of the `<script>` block in `index.html`:
`QTY`, `AVG_FILL`, `STRIKE`, `EXPIRY_ISO`, `TICKER`.
