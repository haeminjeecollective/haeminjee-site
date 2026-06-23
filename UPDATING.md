# How to Update Your Website

## Adding a Publication

1. Create a new folder: `content/publication/your-paper-slug/`
2. Inside it, create `index.md` with this template:

```yaml
---
title: "Your Paper Title"
date: 2026-01-01
authors: ["First Last", "First Last"]
publication_types: ["journal_article"]
publication: "*Journal Name* Vol(Issue): Pages"
abstract: "Full abstract text."
links:
  - name: "Publisher's Version"
    url: "https://doi.org/..."
  - name: "Article"
    url: "files/your-paper.pdf"
tags: ["keyword1", "keyword2"]
---
```

**Publication types:** `journal_article`, `book`, `book_chapter`, `report` (for working papers, commentary, etc.)

3. To include a downloadable PDF, place it in `static/files/` and reference it as `files/your-paper.pdf` in the links.

## Updating the Bio

Edit `content/bio/index.md` directly.

## Updating Teaching

Edit `content/teaching/index.md` directly.

## Updating Contact Information

Edit `content/contact/index.md` directly.

## Updating Research Areas on the Homepage

Edit `layouts/index.html` — each research area is an accordion block. Add or remove `<li>` entries linking to publications.

## Updating the CV PDF

Replace `static/files/Jee_CV.pdf` with the new version (keep the same filename).

## Previewing Locally

1. Install Hugo: `brew install hugo`
2. Run: `hugo server`
3. Open: `http://localhost:1313/`

## Publishing

Push to the `main` branch. GitHub Actions will automatically build and deploy your site to `https://haeminjeecollective.github.io/haeminjee-site/`.
