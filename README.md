# Uyen Mai — personal website (431 Lab 5)

Quarto website. Due to Dr. Love by email (subject **My Website**) on Wed 2026-11-04 at noon.

## Files

| File | What it is |
|---|---|
| `_quarto.yml` | Site settings, navbar, footer |
| `index.qmd` | Front page: photo, links, Welcome, current work, education, honors |
| `research.qmd` | Research & Experience |
| `publications.qmd` | Articles and presentations |
| `cv.pdf` | Public CV (no phone number, no references) |
| `_cv-source/cv.qmd` | Source for `cv.pdf`; folders starting with `_` are not published |
| `profile.jpg` | **Placeholder. Replace with your photo** (square works best) |
| `styles.css` | Small style tweaks |
| `docs/` | Rendered site that GitHub Pages serves |

## Five key elements checklist

- [ ] 1. Photo on front page (`profile.jpg` replaced)
- [x] 2. Email and LinkedIn links (front page and navbar)
- [x] 3. Welcome section on front page
- [x] 4. Education, experience, and projects
- [x] 5. Downloadable CV (navbar and front-page button)

## Before you publish

1. Replace `profile.jpg` with your photo (same file name).
2. Read every page for accuracy, especially "What I'm Working on Now" and "Current Research", which were drafted from your project descriptions rather than your CV.
3. In RStudio: open the folder as a project and run `quarto render` in the Terminal (or click **Render Website** in the Build pane).
4. If you edit `_cv-source/cv.qmd`, re-make the PDF from the Terminal:
   ```
   quarto render _cv-source/cv.qmd
   mv _cv-source/cv.pdf cv.pdf
   quarto render
   ```

## Publish on GitHub Pages

1. Create a free GitHub account if you don't have one.
2. Create a **public** repository named exactly `YOURUSERNAME.github.io`.
3. Upload this whole folder to it (GitHub Desktop is the easiest way: *File → Add Local Repository*, then *Publish*). Make sure `docs/` is included.
4. In the repo: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/docs` → Save**.
5. After a minute or two the site is live at `https://YOURUSERNAME.github.io`.
6. To update later: edit, `quarto render`, commit, push.

Alternative with no GitHub: `quarto publish quarto-pub` in the Terminal gives a free permanent `*.quarto.pub` URL.

## Email to Dr. Love

- **Subject:** My Website
- **Body:** the URL; that the site was built with Quarto and published on GitHub Pages; and the AI tools and prompts used (see `AI-disclosure.md`).
