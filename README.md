# Fab-Form Rental Calculator

A single-page rental quote calculator for Fab-Form used equipment.

- Pick **2 weeks** or **1 month**, then **+2 weeks / +1 month** to extend
- Enter quantities (Shift-click + / − to step by 10)
- Override any price on its card; edit quantity-discount tiers, billing rule and tax under **Pricing settings**
- **Copy quote** (plain text) or **Print / PDF**
- Quantities, prices and settings are remembered in your browser

## Put it live with GitHub Pages

1. Create a new repo on GitHub (e.g. `rental-calculator`), public.
2. Upload `index.html` and the `images/` folder to the repo root (Add file → Upload files, drag both in).
3. Repo **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
4. After a minute your link is `https://<your-username>.github.io/rental-calculator/`

## Changing list prices / products

Edit the `PRODUCTS` list near the bottom of `index.html`. Each line has the name, price,
`unit` (`"month"` or `"week"`), image path, and `hot: true` for the "Most rented" section.
To add a photo for MID Zote, ONEJIG or the kits, drop a PNG in `images/` and set its `img:` path.

## Billing assumptions

- 1 month = 4 weeks.
- Weekly items (Chainsaw Kit, Hot Wire Gun Kit) bill per week.
- Monthly items bill in half-month steps per 2 weeks by default (2 weeks = ½ month price);
  switch to "Round up to full months" in settings if you charge a 1-month minimum.
