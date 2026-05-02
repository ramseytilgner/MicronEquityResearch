# Perplexity Signal — Micron NLP Stock Pitch

A single-page case study applying NLP perplexity signals to Micron Technology earnings call transcripts. April 2026.

The site is fully static — plain HTML, two CSS files, three chart images, and the two source PDFs. No build step required.

## Project Structure

```
.
├── index.html                                      # Main case study page
├── base.css                                        # CSS reset + base styles
├── style.css                                       # Theme tokens + components
├── assets/
│   ├── chart1.png                                  # Cumulative L/S returns
│   ├── chart2.png                                  # Quintile distributions
│   └── chart3.png                                  # Perplexity vs. return scatter
├── Micron Technology Equity Research Memo.pdf      # Full equity memo (linked)
├── Mircon Technology NLP Analysis.pdf              # NLP methodology (linked)
├── .nojekyll                                       # Tells GitHub Pages not to run Jekyll
└── README.md                                       # This file
```

## Deploy to GitHub Pages

### Option 1 — GitHub web UI (easiest, no terminal)

1. Go to https://github.com/new and create a new **public** repository (e.g. `perplexity-signal-micron`). Leave it empty (no README, no .gitignore).
2. On the new repo page, click **uploading an existing file**.
3. Drag every file in this folder — `index.html`, `base.css`, `style.css`, the `assets/` folder, both `.pdf` files, `.nojekyll`, and this README — into the upload area.
4. Click **Commit changes**.
5. Go to **Settings → Pages** in the repo.
6. Under **Source**, choose **Deploy from a branch**. Set branch to `main` and folder to `/ (root)`. Click **Save**.
7. Wait ~30 seconds. Your site will be live at:

   ```
   https://YOUR_USERNAME.github.io/perplexity-signal-micron/
   ```

### Option 2 — git CLI

```bash
cd "Perplexity Signal — Micron NLP Stock Pitch (2)"
git init
git add .
git commit -m "Initial publish"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/perplexity-signal-micron.git
git push -u origin main
```

Then enable Pages from **Settings → Pages → Deploy from a branch → main / (root)**.

### Custom domain (optional)

1. Create a file named `CNAME` (no extension) at the repo root containing only your domain, e.g.:
   ```
   signal.example.com
   ```
2. In your DNS provider, add a CNAME record pointing `signal` to `YOUR_USERNAME.github.io`.
3. In **Settings → Pages**, set the custom domain and tick **Enforce HTTPS** once the cert provisions.

## Local Preview

No build step. Either:

- Double-click `index.html` to open in a browser, **or**
- Run a tiny local server (better for relative asset paths):
  ```bash
  python3 -m http.server 8000
  # then open http://localhost:8000
  ```

## Notes

- Theme toggle (sun/moon icon, top right) flips between dark and light modes.
- Both source PDFs are downloadable from the **Source Documents** section.
- This is educational content. Not investment advice.
