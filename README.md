# 🔥 Higher or Lower

A simple, addictive guessing game. You see one item and its number, then guess whether the next one is **higher or lower**. Keep your streak alive as long as you can, then share your result.

**Categories (550+ items):** 🌍 Countries · 🗼 Landmarks · ⏳ History · 🏎️ Cars · 🍔 Food Calories · ⚽ Football · 🏏 Cricket

## Play
Once GitHub Pages is on, the game is live at:
`https://<your-username>.github.io/<repo-name>/`

## Publish on GitHub Pages
1. Create a new **public** repository on GitHub (for example `higher-or-lower`).
2. Upload `index.html`, `README.md` and `.nojekyll` to the root of the repo.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set *Source* to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
5. Wait a minute or two, then open the link GitHub shows at the top of the Pages settings.

## How it works
- Everything is in one file (`index.html`): no build step, no server, no dependencies.
- Best scores are saved in the player's browser.
- "Copy result to share" copies an emoji result grid plus the game link.

## Editing the data
All items live in the `CATS` object near the top of the `<script>` in `index.html`.
- Simple categories use `['Name', '🙂', value]`.
- Multi-stat categories (Cars, Football, Cricket) use `{n:'Name', e:'🙂', s:{stat: value}}`. Each round picks a stat both items have.

Numbers are approximate. Football and cricket title counts are current as of November 2026.
