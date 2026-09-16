# Dao Anh Tu - Personal Website

Personal portfolio for Dao Anh Tu (`oktutay`) - Computer Science student at SoICT, Hanoi
University of Science and Technology, working on AI in Security.

Static HTML/CSS/JS. No build step, no dependencies, no framework.

## Structure

| File | Contents |
| --- | --- |
| `index.html` | Hero, research interests, CV download, contact, recent updates |
| `skills.html` | Technical skills, experience, education |
| `publications.html` | Papers and work in preparation |
| `projects.html` | Research and engineering projects |
| `awards.html` | Competition results, certifications, earlier achievements |
| `colleagues.html` | Hibiscus Company, teams and labs, communities |
| `blog.html` | Blog index and photo gallery |
| `blogs/` | Individual blog posts |
| `style.css` | All styling. Theme variables live in `:root` at the top |
| `script.js` | Mobile nav toggle and the image lightbox |

The header and footer are **duplicated in every HTML file** - there is no templating.
If you change the nav or footer, change it in all 8 pages.

## Assets

```
assets/avatar.jpg        Hero portrait (4:5, 900x1125)
assets/DaoAnhTu_CV.pdf   Linked from the "Download CV" button on index.html
assets/BaiStudio/        SCIC 2026 Q1 award photos + demo screenshot
assets/MalEvo/           SCIC 2026 Q2 award photos + product screenshots
assets/VAR/              Viettel AI Race 2026 photo
assets/HibiscusCo/       Hibiscus Company members photo
assets/Gallery/          Event photos shown on blog.html
navicon.png              Favicon
```

To swap the CV, overwrite `assets/DaoAnhTu_CV.pdf` - the link in `index.html` does not
need to change.

## Run locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000

## Deploy

GitHub Pages serves this from the repository root via `.github/workflows/jekyll-gh-pages.yml`
on every push to `main`. Settings → Pages → Deploy from a branch → `main` → `/ (root)`.

## Open TODOs

Search the project for `TODO:` - currently:

- Full author list for the LLMal paper on `publications.html`
- A Viettel AI Race photo that you are in, on `awards.html`
