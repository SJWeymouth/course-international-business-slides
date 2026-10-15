# International Business Slides

Public lecture slides for Georgetown University’s **STRT 3260: Introduction to International Business** (Fall 2026):

https://sjweymouth.github.io/course-international-business-slides/

The deployed website is a single-page lecture launcher. Each class deck is available in two formats:

- **Slides** — a Quarto/Reveal.js presentation that opens in the browser
- **PDF** — a matching downloadable version for students and Canvas

## Slide workflow

Slide source is maintained in the private course-production repository and authored with Quarto in RStudio.

1. Pull the latest `main` branch of the private course repository.
2. Copy the shared slide template and name the new deck `YYYY-MM-DD-short-topic.qmd`.
3. Add the class date to the deck’s YAML metadata.
4. Put reusable figures in the shared `assets/` folder.
5. Render or preview the deck locally.
6. Commit and push the source deck and any assets to `main`.

The publishing workflow automatically renders the browser presentation, exports the PDF, updates the lecture launcher, and publishes the generated files to this repository.

## Shared slide design

All International Business decks use one shared Georgetown theme. The design is optimized for 1600 × 900 Reveal slides, large readable type, sparse layouts, and figures that use as much of the available slide area as possible.

Deck-specific CSS should not be added unless a design requirement cannot be handled through the shared theme.

## GitHub Pages deployment

This repository is a generated deployment target. Its `gh-pages` branch is force-published by the private course repository’s **Build and publish Quarto slides** workflow.

Do not edit generated slide, PDF, or website files directly in this repository: the next publication will replace them.

After a slide-related push:

1. Open the private repository’s **Actions** tab.
2. Watch **Build and publish Quarto slides**.
3. Allow several minutes for rendering, PDF export, and publication.
4. If the workflow is green but the browser still shows the old page, force-refresh with **Ctrl+F5**.

## Canvas

Canvas remains the student-facing course site. Class pages can link directly to the stable browser presentation and PDF URLs published here. Readings, assessments, instructor materials, and other restricted course content are not published in this repository.
