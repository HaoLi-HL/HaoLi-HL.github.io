# HaoLi-HL.github.io

## How to apply website changes
1. Edit content in `index.html` (main landing page) or `index.md` (Jekyll markdown page).
2. The profile photo is embedded directly in `index.html` as a Base64 `data:image` URL to avoid binary-file limitations in some environments.
3. Preview locally:
   ```bash
   python3 -m http.server 8000
   ```
   Then open `http://127.0.0.1:8000`.
4. Commit and push:
   ```bash
   git add index.html index.md README.md
   git commit -m "Update website content and profile photo"
   git push
   ```
5. GitHub Pages will redeploy automatically after push.
