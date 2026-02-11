# HaoLi-HL.github.io

## How to apply website changes
1. Edit content in `index.html` (main landing page) or `index.md` (Jekyll markdown page).
2. Update your profile image via `photo.svg` (text-based image wrapper), which avoids binary-file limitations in some review/deploy tools.
3. Preview locally:
   ```bash
   python3 -m http.server 8000
   ```
   Then open `http://127.0.0.1:8000`.
4. Commit and push:
   ```bash
   git add index.html index.md photo.svg README.md
   git commit -m "Update website content and photo"
   git push
   ```
5. GitHub Pages will redeploy automatically after push.

## If you encounter "Binary files are not supported"
- Do not commit a raw `.jpg`/`.png` to this repo for the profile image.
- Use `photo.svg` as done here, which embeds the photo as text content and is accepted by text-only tooling.
