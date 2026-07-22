# Terry Liu — Quant Portfolio

A dependency-free, responsive, dark-mode portfolio built for quantitative research and trading-system applications.

## Run locally

```bash
python3 -m http.server 4173
```

Then visit `http://localhost:4173`.

## Publish with GitHub Pages

This portfolio is prepared for a GitHub user site at
`https://kiwicabbage.github.io/`.

1. On GitHub, create a **public** repository named exactly
   `kiwicabbage.github.io`. Do not add a README, `.gitignore`, or license there.
2. In this folder, connect and upload the prepared `main` branch:

   ```bash
   git remote add origin https://github.com/kiwicabbage/kiwicabbage.github.io.git
   git push -u origin main
   ```

3. Open the repository's **Settings → Pages**. Under **Build and deployment**,
   select **Deploy from a branch**, choose `main` and `/(root)`, then save.
4. Wait a few minutes, then open `https://kiwicabbage.github.io/`.

### Update the live site later

After editing the files, publish the update with:

```bash
git add .
git commit -m "Update portfolio"
git push
```

GitHub Pages will redeploy automatically. The academic record PDFs listed in
`.gitignore` remain local and are intentionally excluded from the public site.

## Structure

- `index.html` — portfolio content and semantic structure
- `styles.css` — responsive visual system and motion
- the site is fully static: no JavaScript and no runtime dependencies
- source PDFs remain in the project root; the résumé and private project summary are linked directly
- `.nojekyll` — tells GitHub Pages to serve the static files without Jekyll processing
