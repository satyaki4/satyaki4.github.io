# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Site Overview

Plain HTML/CSS static site hosted on GitHub Pages. No build system — files are served as-is. `.nojekyll` disables Jekyll. Push to `main` to deploy.

## Structure

- `index.html` — About/home page (bio, contact)
- `research.html` — Working papers and policy papers
- `teaching.html` — Teaching history with course evaluations
- `style.css` — Single stylesheet for all pages
- `files/` — PDFs (CV, papers, course evaluations); synced from `C:\Users\satya\Dropbox\satyaki4.github.io_files\files_synced_on_website`
- `images/` — Profile photos and favicons

## Workflow

Files (CV, evals, paper drafts) are generated in Dropbox, staged to `files_synced_on_website`, then copied here before committing. When the user says "update the CV" or "add eval PDFs", the source files come from that Dropbox staging folder.

## Conventions

- All three HTML pages share the same nav bar structure — keep them in sync when editing navigation.
- No JavaScript anywhere; keep it that way.
- Mobile breakpoint is 540px in `style.css`.
- PDF links in `research.html` point to `/files/filename.pdf`; confirm the file exists in `files/` before adding a link.
