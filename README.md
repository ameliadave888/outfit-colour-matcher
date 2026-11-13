# The Outfit Edit — Colour Matcher

A free, offline-friendly, mobile-first wardrobe colour matching mini-app. No sign-in, APIs, subscriptions or third-party libraries.

## Try it locally

Open `index.html` in a modern browser. The preview works without a server; for home-screen installation and offline caching, publish the folder to an HTTPS website.

## Put it online with GitHub Pages

1. Create a **public** GitHub repository named `outfit-colour-matcher` (GitHub Pages is free for public repos).
2. Put all files from this folder into the root of that repository (not inside an additional nested folder). Commit and push to `main`.
3. In repository **Settings → Pages**, set **Source: Deploy from a branch**, choose `main` and `/(root)`, and save.
4. Open `https://YOUR-USERNAME.github.io/outfit-colour-matcher/` once GitHub Pages publishes it.
5. Android Chrome: menu (⋮) → **Add to Home screen** or **Install app**. iPhone Safari: Share → **Add to Home Screen** and enable **Open as Web App** if available.

## Features

- Preloaded example pieces: olive, black and grey trousers; black, cream and blue knit polos; grey, white and black shoes.
- Select combinations and see an illustration + an explanation.
- Shuffle top-scored combinations, browse office/weekend/dinner-ranked ideas, save favourites.
- Add or remove clothes, change individual shades, export/import a JSON wardrobe backup.
- Data is stored in browser local storage and **does not sync across devices**. Export a backup before changing browsers/devices or clearing storage.
- Offline functionality is enabled after the site has been loaded successfully under HTTPS and the service worker has installed.

## Updating it

Edit `index.html` in any editor, then commit and push. Future changes to the service worker's cache should bump `CACHE` in `sw.js` (e.g. `outfit-edit-v2`) so browsers refresh the offline app.

The initial blue and grey shades are illustrative. Adjust them in **Manage your wardrobe** to match your actual clothes.
