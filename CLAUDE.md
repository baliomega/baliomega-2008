# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the "Baliomega 2008" portfolio website - a static HTML/CSS/JavaScript site showcasing the design and web development work of Nurul Izwan Dahlan. The site is a legacy portfolio from 2008 featuring graphic design works and web design mockups.

## Architecture

**Static Website Structure:**
- `index.html` - Main portfolio page with complete site content
- `style.css` - Primary stylesheet with dark theme and blue accent colors (#0099ff)
- `lightview.css` - Stylesheet for the Lightview image gallery plugin
- `js/` - JavaScript dependencies (Prototype.js, Script.aculo.us, Lightview)
- `designworks/` - Portfolio images organized as thumbnails (s-*.jpg) and full-size images (b-*.jpg)
- `img/` - Site assets and header images
- `works/` - Additional work samples directory

**Key Technologies:**
- XHTML 1.0 Strict
- CSS for layout and styling (fixed 870px width, dark theme)
- Prototype.js framework for JavaScript functionality
- Script.aculo.us for visual effects
- Lightview for image gallery/lightbox functionality

**Content Organization:**
The portfolio is divided into two main sections:
1. **Graphic works** - Print design, magazine layouts, wallpapers, flyers, brochures, t-shirt designs
2. **Web Design works** - Website mockups, live sites, and web banners

## Development Notes

**No Build Process:** This is a static site with no build system, package manager, or compilation steps. All files are served directly.

**Image Gallery System:** Uses Lightview plugin with gallery grouping via `rel="gallery[name]"` attributes. Thumbnails follow naming convention `s-*.jpg` for small images and `b-*.jpg` for full-size images.

**Analytics:** Site includes Reinvigorate analytics tracking (legacy service).

## File Patterns

- Thumbnail images: `designworks/s-[project].jpg` (250x200px)
- Full-size images: `designworks/b-[project]-[number].jpg`
- Multiple images in galleries use sequential numbering (01, 02, 03, etc.)

## Legacy Considerations

This is a 2008-era website using legacy JavaScript libraries and XHTML. When making modifications:
- Maintain compatibility with Prototype.js and Script.aculo.us
- Preserve the fixed-width layout and dark theme design
- Keep the lightbox gallery functionality intact
- Maintain XHTML 1.0 Strict compliance if editing HTML