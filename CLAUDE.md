# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static CV/Resume website for Isidro Torregrosa Torralba. It consists of a single HTML page styled with modern CSS, presenting a professional curriculum vitae.

## Project Structure

- `index.html` - Main HTML file containing the CV content and structure
- `index.css` - Stylesheet with CSS Grid layout, custom properties, and responsive design
- No build process or dependencies (except Font Awesome CDN for icons)

## Development Commands

Since this is a static site with no build process:
- **View locally**: Open `index.html` directly in a web browser
- **Deploy**: Upload both files to any static hosting service (GitHub Pages, Netlify, Vercel, etc.)

## Architecture & Code Style

### HTML Structure
- Semantic HTML5 elements
- BEM-like class naming convention (e.g., `cv__header`, `section__title`)
- Sections: Header (name, title, contact), Aside (skills, languages), Main (about, experience, education)

### CSS Architecture
- CSS custom properties for theming in `:root`
- Grid layout for responsive design
- Color scheme: Blue accent colors (#1a237e primary, #3949ab secondary)
- Typography scale using rem units
- Spacing scale based on 4px unit
- Print styles included for PDF generation
- Mobile-responsive breakpoints at 768px and 480px

### Key CSS Variables
- Colors: `--cv-primary`, `--cv-secondary`, `--cv-accent`
- Typography: `--cv-font-size-*` (xs through xl)
- Spacing: `--space-*` (1 through 8)

## Important Considerations

- No JavaScript - purely static HTML/CSS
- Font Awesome 6.5.1 loaded from CDN for icons
- All external links open in new tabs with `rel="noopener"`
- Contact information is clickable (mailto, tel, links)
- Optimized for both screen viewing and printing