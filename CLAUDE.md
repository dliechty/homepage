# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static personal homepage for David Liechty. Single-page site with no build step, no dependencies, and no tests.

## Architecture

- **`index.html`** — The entire site: HTML, CSS (inlined in `<style>`), and inline SVG icons. No JavaScript.
- Deployed via **GitHub Pages** directly from the `main` branch.
- Uses **CSS custom properties** (`--color-*`) for theming with automatic light/dark mode via `prefers-color-scheme`.
- Typography from Google Fonts (Inter).

## Development

Open `index.html` in a browser. No build or serve commands needed.

## Deployment

Push to `main` — GitHub Pages serves the site automatically.
