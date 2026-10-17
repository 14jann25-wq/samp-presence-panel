# SA:MP Presence — Web Control Panel

Static front-end prototype for configuring a SA:MP / Discord Rich Presence setup.

## Run locally
Open `index.html` in a browser, or use the VS Code Live Server extension. No build step is required.

## Deploy online with GitHub Pages
1. Create a new repository on GitHub (for example `samp-presence-panel`).
2. Upload `index.html`, `style.css`, `app.js`, and `README.md` to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then Save.
6. Wait for the published URL shown on the Pages settings screen.

## What works
- Edit activity, server name, details, address and a preview player count.
- Live preview card.
- Save the settings in the current browser using localStorage.
- Export/copy `presence-config.json`.

## Important limitation
This website is only a configuration UI. A static website cannot directly inspect the local SA:MP process or publish Discord Rich Presence by itself. A separate Windows companion/plugin must read the configuration, safely detect game state, and use Discord's supported Rich Presence integration. The player count and server data here are user-entered preview values, not live game data.

Do not put Discord client secrets, tokens, or other credentials in this static website. The preview is not an official Discord UI and this project is not affiliated with Discord or SA:MP.
