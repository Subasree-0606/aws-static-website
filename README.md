# aws-static-website

Personal portfolio static website (HTML/CSS/JS) — Subasree Rajaram

This repository contains a simple, responsive static website showcasing AWS DevOps projects and skills.

## What’s included

- `index.html` — main site markup
- `style.css` — styling for the site
- `script.js` — small client-side JS (mobile nav toggle, year auto-update)
- `assets/` — images and favicon

## Run locally (two easy ways)

1) Using VS Code Live Server (recommended for development)
- Install the Live Server extension in VS Code.
- Open the project folder in VS Code.
- Open `index.html` and click **Go Live** (bottom-right) — the site will open in your default browser.

2) Using a lightweight Node static server (if you have Node.js installed)
- Open PowerShell in the project folder (or VS Code integrated terminal):

```powershell
# install/run without installing globally
npx http-server -p 8080
# open this URL in your browser:
# http://127.0.0.1:8080
```

## Project structure

```
index.html
style.css
script.js
assets/
  images/
  favicon.ico
README.md
```

## Common troubleshooting

- Portrait image not showing:
  - Confirm the image exists under `assets/images/` (for example `assets/images/Profile.jpeg` or `profile.jpg`).
  - Use forward slashes in HTML `src` attributes: `<img src="assets/images/profile.jpg" alt="...">` (avoid backslashes `\`).
  - If the image still 404s, open DevTools (F12) → Network and reload; the Console/Network tab shows the exact path and error.

- "Go Live" button missing in VS Code:
  - Ensure the Live Server extension is installed.
  - Confirm your workspace is opened at the project root and `index.html` is part of the workspace.

## Notes & small fixes to consider

- The hero image `img` should use a relative path with forward slashes and the correct filename/case. Example:

```html
<div class="hero-image">
  <img src="assets/images/Profile.jpeg" alt="Portrait of Subasree">
</div>
```

- If you prefer a different filename or extension (jpg/png), update the `src` accordingly.

## Contact

If you want further edits or a different layout for the projects section (cards, grid, or the exact screenshot style), tell me which design to target and I’ll update `style.css` and `index.html`.

---

© Subasree Rajaram
