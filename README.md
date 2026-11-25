# roblotracker GitHub Pages

This repository only contains the public website. It uses plain HTML and CSS, with the production pages rooted in `docs/`. The bot service and its configuration are maintained separately.

## Preview

Run `python -m http.server 8000 --directory docs` from this folder and open `http://localhost:8000/`.

## Publish

In the website repository’s **Settings → Pages**, select **Deploy from a branch**, **main**, and **/docs**. Each push to `main` updates the site. The untouched `docs/.nojekyll` file enables static file serving.

Use `/privacy.html` and `/terms.html` under the deployed Pages base URL for the app’s Privacy Policy and Terms of Service fields in the Discord Developer Portal. Contact and install links are ordinary Discord URLs. When configuration or data handling changes, update each affected page and its revision date.

The site also serves short links at `/privacy/` and `/terms/`. The alternate `/pysics/` spelling opens the Privacy Policy.

## Move the site to roblotracker.github.io

GitHub reserves each `github.io` address for the matching user or organization. To use `roblotracker.github.io`, sign in to an account that can create repositories as `roblotracker`. Create a public repository named `roblotracker.github.io` owned by `roblotracker`, upload this website's `docs/` folder to the `main` branch, and publish from `main` and `/docs` in **Settings → Pages**. Once the new site and both policy pages load, update the links in the Discord Developer Portal.

If someone else controls that GitHub name, keep the current project address or connect a domain you control under **Settings → Pages → Custom domain**. Renaming the website repository under a different account changes the URL path. The owner name still determines the `github.io` address.
