# Singapore Environment Map

Static web app (GitHub Pages) showing PM2.5, rainfall, temperature, lightning and dengue clusters.

## Setup
1. Create a public GitHub repository and upload these files, keeping the folder structure:
   - `index.html` (rename `sg-air-temperature.html` to `index.html`)
   - `dengue.geojson` (created automatically by the workflow; you can also add an initial copy now)
   - `.github/workflows/update-dengue.yml`
2. Repository **Settings → Pages**: source "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Repository **Actions** tab: enable workflows if prompted, then open "Update dengue clusters" and click **Run workflow** once to create the first `dengue.geojson`.
4. Open `https://<your-username>.github.io/<repo-name>/` on your phone and allow location access.

The dengue file refreshes automatically every 6 hours. Real-time weather and air-quality feeds load directly in the browser.
