# AGENTS.md

This is the static website for the [Kopf](https://github.com/nolar/kopf) project, hosted at [kopf.dev](https://kopf.dev).

## Tech Stack

Plain HTML + Tailwind CSS (CDN) + highlight.js for syntax highlighting. No build step, no framework.

## Style Guide

See [STYLEGUIDE.md](STYLEGUIDE.md) for colors, typography, components, layout patterns, and page templates. All pages must follow this guide for visual consistency.

## Structure

- `index.html` — landing page
- `CNAME` — GitHub Pages custom domain config
- `.github/workflows/pages.yaml` — deployment workflow

## Deployment

GitHub Pages via GitHub Actions. Deploys on push to `main`. Custom domain: `kopf.dev`.

## Guidelines

- Every new page must reuse the same `<head>` block (CDN deps, Tailwind config, custom CSS), `<nav>`, and `<footer>` from `index.html`.
- Alternate section backgrounds between `bg-white` and `bg-slate-50`.
- Use the `code-window` component for all code examples.
- All external links must use `target="_blank" rel="noopener"`.
