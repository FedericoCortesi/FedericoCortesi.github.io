# Federico Cortesi — academic website

Built with [al-folio](https://github.com/alshedivat/al-folio) and published at https://federicocortesi.github.io.

## Where to put your content

Search the repo for `PLACEHOLDER` to find everything that still needs filling in.

| What | File |
| --- | --- |
| Name, site description, contact note | `_config.yml` (top section) |
| Bio, research interests, contact, position | `_pages/about.md` |
| Profile photo | replace `assets/img/prof_pic.jpg` |
| Publications | `_bibliography/papers.bib` (BibTeX; add `selected={true}` to feature a paper on the home page) |
| CV page | `_data/cv.yml` |
| CV PDF download | upload as `assets/pdf/cv.pdf` |
| Email, GitHub, Scholar, LinkedIn, ORCID icons | `_data/socials.yml` |
| News items (optional) | add files to `_news/`, then set `announcements.enabled: true` in `_pages/about.md` |

## Publishing

Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site and pushes it to the `gh-pages` branch.
One-time setup: in the repo's **Settings → Pages**, set **Source** to "Deploy from a branch", branch `gh-pages`, folder `/ (root)`.

## Preview locally

```bash
bundle install
LANG=C.UTF-8 bundle exec jekyll serve   # http://localhost:4000
```

The full al-folio documentation is at https://github.com/alshedivat/al-folio.
