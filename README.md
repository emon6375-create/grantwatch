# GrantWatch 2.0 PC

Desktop/web version of GrantWatch 2.0. It is a zero-cost, install-free web app that can run locally on Windows/macOS/Linux or be hosted free with GitHub Pages.

## Run on your PC
1. Extract the ZIP.
2. Open the `app` folder.
3. Double-click `index.html`.
4. If your browser blocks local JSON loading, run a tiny local server:
   - Windows: `python -m http.server 8080`
   - macOS/Linux: `python3 -m http.server 8080`
   from the project root, then open `http://localhost:8080/app/`.

## Live data
Set `DATA_URL` in `app/config.js` to your GitHub raw `data/grants.json` URL.

## Automatic monitoring
The collector in `collector/collect.py` runs through GitHub Actions every 6 hours and updates `data/grants.json`.

## Important
This is designed for free infrastructure. No paid server is required. Worldwide coverage cannot honestly be guaranteed because funding bodies publish through many different systems and may block automated access. Expand `config/sources.json` to increase coverage.
