# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio/blog site for Vincent Chen (mao3267), built with Hugo and deployed to GitHub Pages at https://mao3267.github.io/.

## Commands

- **Dev server**: `hugo server` (runs at localhost:1313 with live reload)
- **Build**: `hugo` (outputs to `public/`)
- **New content**: `hugo new content/<section>/<slug>.md`

## Architecture

This is a Hugo static site using the **Adritian** theme (`themes/adritian-free-hugo-theme/`).

### Configuration (dual config)

- `hugo.toml` — Primary config: theme settings, menu structure, plugins, analytics, color theme, i18n. Sections enabled via `params.sections`.
- `hugo.yaml` — Minimal override: baseURL, languageCode, title.

Both are loaded by Hugo (YAML overrides TOML for overlapping keys).

### Content Structure

- `content/experience/` — Work/research experience entries (Markdown with front matter)
- `content/projects/` — Project portfolio entries
- `content/blog/` — Blog posts
- `data/homepage.yml` — Homepage section toggles (showcase, about, education, experience, contact, etc.) and social links
- `i18n/en.yaml` — All user-facing text strings (name, bio, descriptions, section titles, contact info). **Edit this file to change any displayed text on the site.**

### Key Conventions

- The theme supports i18n (en/es/fr) but only English is enabled; Spanish and French are disabled in `hugo.toml`.
- Homepage sections are controlled by `params.sections` in `hugo.toml` and the `enable` flags in `data/homepage.yml`.
- Images go in `assets/images/` (processed by Hugo) or `static/` (served as-is). Currently showcase/about images are referenced from `assets/images/`.
- The `layouts/` directory is empty — all templates come from the theme. To customize a template, copy it from `themes/adritian-free-hugo-theme/layouts/` into `layouts/`.
- The `public/` directory is the build output and should not be edited directly.
