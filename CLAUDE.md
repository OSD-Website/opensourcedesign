# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll static site theme for Open Source Design community. Built with Ruby/Jekyll, SCSS for styling, and GitHub Pages compatible.

## Build Commands

```bash
# Install dependencies
bundle install

# Build the site (outputs to _site/)
bundle exec jekyll build

# Run development server (http://localhost:4000)
bundle exec jekyll serve
```

## Architecture

### Layout System
- `_layouts/default.html` - Main wrapper template
- `_layouts/home.html` - Homepage with hero section
- `_includes/` - Reusable components (header, footer, sidebar, hero-motif)

### SCSS Architecture
Modular styles in `_sass/`:
- `_variables.scss` - CSS custom properties for colors, spacing, typography
- `_base.scss` - Typography and element defaults
- `_layout.scss` - Grid system (2-column: `2fr 1fr`, collapses at 900px)
- `_components.scss` - Component styles (RHC cards, pills, sponsor grids)

Entry point: `assets/css/main.scss` imports all partials.

### Design Tokens
Color palette uses CSS variables with naming convention:
- `--brand-*` (navy tones)
- `--mint-*` (accent colors)
- `--neutral-*` (grayscale)

### Content
- `index.md` - Homepage content (uses `home` layout)
- `about.md` - About page with sponsor/contributor grids
- Content written in Markdown with YAML frontmatter

### Configuration
`_config.yml` controls Jekyll settings including:
- kramdown markdown processor
- Compressed SCSS output
- Excluded files from build
