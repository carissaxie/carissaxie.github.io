# Personal Academic Website — Yi Xie · Build Plan & Tracker

This file is the **source-of-truth tracker** for building the website. It lives at the
repo root so progress is reviewable in git. Each step below is completed in a focused
commit that also ticks its checkbox, so `git log` reads as a step-by-step build log.

- **Repo:** `carissaxie.github.io` → GitHub Pages
- **Framework:** [Quarto](https://quarto.org)
- **Custom domain:** TBD (e.g. `yixie.bio`)
- **Tracker issue:** "Website build — plan tracker" (mirror this checklist once the repo is on GitHub)

## Scope guardrails
- **Show only published work.** The Projects page features **scPanel only** for now.
- **Unpublished work is held off the site** (ATOMIC, state_weighted, drug/MoA harmonization,
  and anything else in progress). Research pages stay at a **general thematic level** and
  never name unpublished projects.
- Site structure scales: add a new card under `_projects/` once a project is published.

## Featured publication — scPanel
Yi Xie, Jianfei Yang, John F. Ouyang, Enrico Petretto.
*scPanel: a tool for automatic identification of sparse gene panels for generalizable
patient classification using scRNA-seq datasets.*
**Briefings in Bioinformatics** 25(6), 2024, bbae482.
DOI: [10.1093/bib/bbae482](https://doi.org/10.1093/bib/bbae482) ·
bioRxiv: [10.1101/2024.04.09.588647](https://doi.org/10.1101/2024.04.09.588647) ·
Code: [github.com/carissaxie/scPanel](https://github.com/carissaxie/scPanel)

## Step checklist

- [x] **Step 0 — Repo + tracker bootstrap.** `~/site` working dir, git on `main`, this `PLAN.md`.
- [x] **Step 1 — Install Quarto & scaffold.** Quarto CLI installed (user-space tarball) + site skeleton.
- [x] **Step 2 — Configure `_quarto.yml`.** Navbar, theme, SEO metadata, sitemap.
- [x] **Step 3 — Write content pages.** `index`, `research`, `projects`, `_projects/scpanel`, `cv`.
- [x] **Step 4 — references.bib + publications page.** scPanel entry rendered.
- [x] **Step 5 — Add assets.** Placeholder `profile.jpg`, `assets/favicon.png`, `projects/scpanel.png`, `assets/cv.pdf` in place — **swap in your real photo + CV**.
- [ ] **Step 6 — Deploy via GitHub Actions.** `publish.yml`; create GitHub repo + set Pages source. *(needs your GitHub auth)*
- [ ] **Step 7 — Custom domain.** Buy domain, add `CNAME`, set DNS, enforce HTTPS. *(your action)*
- [ ] **Step 8 — SEO / discoverability.** Sitemap, robots.txt, Google Search Console, meta tags.

## Items needed from you
- Headshot image + CV PDF.
- Final bio wording + exact job title/affiliation.
- ORCID, Google Scholar, LinkedIn, X/BlueSky URLs.
- Domain name to purchase.

## How to work on this site
```bash
# from repo root
export PATH="$HOME/.local/bin:$PATH"   # quarto lives here
quarto preview      # live local preview
quarto render       # full build into _site/
```
