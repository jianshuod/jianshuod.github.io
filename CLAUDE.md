# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML academic portfolio website for Jianshuo Dong (PhD student at Tsinghua University). The site showcases research publications, education, and professional activities in machine learning security and trustworthy AI.

## Development

**No build process** - This is a pure static site with no build tools, package manager, or dependencies.

To preview locally, open `index.html` directly in a browser or use any static file server:
```bash
python3 -m http.server 8000
```

## Architecture

- `index.html` - Single-page site with all content (inline CSS, table-based layout)
- `css/custom.css` - Custom tag styling for publication metadata (oral/poster badges)
- `css/academicons.min.css` - Academic icon library for Google Scholar badge
- `fonts/` - Academicons font files
- `images/` - Profile photo and images
- `data/` - PDF files for research papers

## Making Changes

- **Content updates**: Edit `index.html` directly (publications, news, education sections)
- **Styling**: Add custom styles to `css/custom.css`, avoid modifying inline styles in HTML when possible
- **New papers**: Add PDF to `data/`, update publications section in `index.html`

## External Dependencies (CDN)

The site loads these from external CDNs:
- Google Fonts (Lato)
- Font Awesome icons
- Google Analytics (currently commented out)
