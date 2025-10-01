# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal academic website template for graduate students in social sciences at Université Laval, used as a course assignment in the digital tools course (POL-6078). The site is built with static HTML/CSS/JavaScript and hosted on GitHub Pages with a custom domain (adriencloutier.com).

## Architecture

**Template**: Based on the "Read Only" template by HTML5 UP (html5up.net), licensed under CCA 3.0

**Structure**:
- `index.html` - Main landing page with sections: About, Work, CV, Projects, Contact
- `assets/` - Static resources (CSS, JS, webfonts)
  - `css/main.css` - Primary stylesheet
  - `js/` - jQuery and template scripts (scrolling, breakpoints, browser detection)
- `images/` - Site images including portrait and background
- `cv/` - CV directory containing PDF, source (LaTeX/markdown/Quarto), and preview image (cv.jpg)
- `projet_session/` - Projects directory containing R Markdown projects exported to HTML
- `CNAME` - Custom domain configuration for GitHub Pages

**Navigation**: Single-page site with smooth scrolling between sections using jQuery scrolly/scrollex

## Development Commands

This is a static site with no build process. To work on it:

1. **Local preview**: Open `index.html` directly in a browser, or use a simple HTTP server:
   ```bash
   python -m http.server 8000
   ```

2. **Deploy to GitHub Pages**:
   ```bash
   git add .
   git commit -m "Update site"
   git push origin main
   ```
   Site automatically publishes to GitHub Pages after push.

## Key Implementation Details

**Projects section**: The `projet_session/` directory contains R Markdown files (`.Rmd`) that are "knitted" into HTML using RStudio. Each project needs:
- `projet.Rmd` - R Markdown source
- `projet.html` - Exported HTML output (generated from .Rmd)
- `projet.png` - Preview thumbnail

**CV section**: Follows same pattern - needs PDF, source file, and preview image (`cv.jpg`)

**Social links**: Located in the sidebar footer, configured with `href` attributes in index.html:19-68

**FontAwesome icons**: Template includes fontawesome-all.min.css for icon support throughout the site

## Important Notes

- The index.html file MUST remain named `index.html` - this is the default entry point for web browsers
- The site uses French language for content (target audience: Quebec graduate students)
- Template includes extensive commented-out example code (lines 204-532) showing available UI components
- When adding new projects, update both the navigation menu and create a new `<article>` in the projects section
- Git remote currently points to a different repository (clessn/article_syrie-ukraine) - may need updating

## Domain Configuration

Custom domain `adriencloutier.com` is configured via:
- `CNAME` file in repository root
- DNS settings at domain registrar (Namecheap) pointing to GitHub Pages IPs
- GitHub Pages settings with "Enforce HTTPS" enabled
