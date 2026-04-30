# Proteo-R1

Official project page for **Proteo-R1: Reasoning Foundation Models for *De Novo* Protein Design** (ICML 2026).

**Live site:** [https://smiles724.github.io/r1/](https://smiles724.github.io/r1/)  
**Repository:** [https://github.com/smiles724/r1](https://github.com/smiles724/r1)

## Repository layout

| File | Purpose |
|------|---------|
| `index.html` | Single-page site: abstract, method figure, results tables, BibTeX, sticky nav |
| `styles.css` | Layout, hero styling, tables, responsive tweaks |
| `logo.svg` | Site and favicon mark (antibody + helix motif) |
| `figure.pdf` | Main schematic embedded in the Method section |
| `main.tex` | Camera-ready LaTeX source (optional; not required for Pages) |

## GitHub Pages

1. Open **Settings → Pages** on the repo.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose branch **`main`** and folder **`/ (root)`**, then save.

The site URL is `https://smiles724.github.io/r1/` (unless you use a custom domain).

## Updating the site

1. **Paper links:** In `index.html`, replace placeholder `href="#"` on the top **GitHub** button and on **Paper PDF / ArXiv / OpenReview / Code** when those URLs are ready.
2. **Content:** Title, authors, affiliations, abstract, tables, and corresponding-author emails are already synced from the paper; adjust in `index.html` if the camera-ready version changes.
3. **Figure:** Replace `figure.pdf` and keep the same filename, or update the `<object>` / link in `index.html`.

## Local preview

Open `index.html` in a browser, or from this directory:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Push to GitHub

```bash
git add .
git commit -m "Update project page"
git push origin main
```

If `git push` asks for credentials, use [GitHub CLI](https://cli.github.com/) (`gh auth login`) or a [personal access token](https://github.com/settings/tokens) with `repo` scope for HTTPS.
