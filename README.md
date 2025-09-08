# ChetzGPT

ChetzGPT is a delightfully unhelpful, single‑file, snarky chatbot parody. It looks like a chat app, but only replies with random canned snark (and the occasional dad joke).

- Live (enable GitHub Pages): https://eranchetz.github.io/chetzgpt/
- Repo: https://github.com/eranchetz/chetzgpt

## Features
- Single file (`index.html`): no build, no dependencies
- Chat‑style UI with typing indicator
- Random snarky responses; keyword‑triggered dad jokes
- Enter to send; Shift+Enter for newline
- Chat history persisted to `localStorage`
- Clear button to wipe history

## Quick Start (Local)
1. Clone the repo
   ```bash
   git clone https://github.com/eranchetz/chetzgpt.git
   cd chetzgpt
   ```
2. Start a static server (any will do). Examples:
   ```bash
   # Python 3
   python3 -m http.server 8000 --bind 127.0.0.1
   # or Node.js (if installed)
   npx http-server -p 8000 -a 127.0.0.1
   ```
3. Open http://127.0.0.1:8000 in your browser.

## Deploy to GitHub Pages
1. Push to GitHub (already done if you’re reading this repo):
   ```bash
   git push origin main
   ```
2. In the repo, go to Settings → Pages.
3. Source: “Deploy from a branch”.
4. Branch: `main` and folder `/ (root)` → Save.
5. Wait a minute; your site will be at:
   - https://eranchetz.github.io/chetzgpt/

## Customize
- Responses: edit the arrays in `index.html`:
  - `SNARK` for snarky lines
  - `DAD_JOKES` for jokes
  - `TEMPLATES` for prompt‑referencing quips
- Storage key: change `STORE_KEY` to reset caches between versions.
- Branding: tweak the `<title>`, header text, and favicon data URL.

## Notes
- This is parody software. It intentionally provides unhelpful, fabricated answers.
- No tracking, analytics, or external requests; everything runs client‑side.

