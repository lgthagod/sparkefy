# Sparkefy Support Site

Official support site for the Sparkefy iOS app.

**Live URL:** https://lgthagod.github.io/sparkefy/

## Stripe Connect redirect pages

- Return: https://lgthagod.github.io/sparkefy/payout-return.html
- Refresh: https://lgthagod.github.io/sparkefy/payout-refresh.html

## GitHub Pages setup

The `Deploy GitHub Pages` workflow publishes static files to the **`gh-pages`** branch.

If payout pages return 404, set **Settings → Pages → Build and deployment → Source** to **Deploy from a branch**, branch **`gh-pages`**, folder **`/ (root)`**.

Alternatively, allow the `main` branch in **Settings → Environments → github-pages → Deployment branches** and switch source to **GitHub Actions**.
