# Eventora — Smart Event & Vendor Management

Static website (a single `index.html`). Host: Shlok Gupta, 7318168802.

## Put it live with GitHub Pages
1. Create a new repository on GitHub (for example `eventora`). Public is simplest.
2. Upload these files to the repository root (GitHub web: Add file > Upload files), or from a terminal in this folder:
   ```
   git init
   git add .
   git commit -m "Eventora website"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/eventora.git
   git push -u origin main
   ```
3. In the repository open Settings > Pages. Under "Build and deployment" choose Source: **Deploy from a branch**, Branch: **main**, folder **/ (root)**, then Save.
4. Wait 1 to 2 minutes. Your site is at `https://YOUR-USERNAME.github.io/eventora/`.

## What works on GitHub Pages
- The whole design, pages, vendor search, planner, event-day demo, and theme switching.
- Quote requests are sent to the host by WhatsApp (the visitor taps Send).

## What does not work on GitHub Pages
GitHub Pages only hosts static files, so there is no backend. Sign in, saved quotes, dashboards and saved plans need the FastAPI backend (separate project) running somewhere else. Until then the site says "Backend not connected" for those actions. Vendors, ratings and prices are sample data.

## Updating the site
Replace `index.html` (and `404.html`, keep it identical), commit, push. Pages redeploys on its own.
