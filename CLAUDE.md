# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal website for Leon S. Freyermuth, an attorney at Gibson Dunn. Static single-page site with a retro CLI aesthetic.

## Development

No build system. Open `index.html` directly in a browser to preview.

## Deployment

Push to `main` branch to auto-deploy via GitHub Pages to https://leonf.me

## Architecture

- `index.html` - Single page with semantic HTML structure (header, about section, footer)
- `style.css` - All styles including responsive (mobile) and dark mode via `@media (prefers-color-scheme: dark)`
- `favicon.svg` - SVG favicon with "LSF" initials
- `assets/headshot.jpg` - Profile photo (displayed grayscale via CSS filter)
- `CNAME` - Custom domain configuration for GitHub Pages

## Design Notes

- Monospace font (IBM Plex Mono)
- Minimal black/white color scheme with CSS borders
- Dark mode styles must be placed at the END of style.css to properly override base styles (CSS specificity)
- Headshot uses `object-position: center 20%` to frame face properly
