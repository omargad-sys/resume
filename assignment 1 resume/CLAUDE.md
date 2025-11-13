# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML resume website for Omar Gad. The project is a simple, single-page personal resume with no build process or dependencies.

## Architecture

The codebase consists of:
- `index.html` - Main resume page with semantic HTML sections (contact, summary, education, work experience, skills, certifications)
- `styles.css` - Basic styling with wheat background and teal headings (#098a9e)
- `favicon.png` - Site favicon
- `Omar Gad.JPG` - Profile picture displayed in the header

## Development

This is a static website with no build process. To work on it:

1. **Preview changes**: Open `index.html` directly in a browser or use a local server:
   ```bash
   python3 -m http.server 8000
   ```
   Then navigate to `http://localhost:8000`

2. **Edit HTML**: Modify `index.html` directly
3. **Edit styles**: Modify `styles.css` directly

## Git Workflow

- Main branch: `main`
- Remote: https://github.com/omargad-sys/resume.git
- All changes are committed and synced with remote

## Code Style Notes

- HTML5 semantic elements: `<header>`, `<main>`, `<section>`, `<footer>`
- Accessibility: ARIA labels, proper heading hierarchy, Schema.org structured data
- Responsive design with mobile-first approach
- External links use `target="_blank"` with `rel="noopener noreferrer"` for security
- Profile picture styled with circular border and shadow
- Color scheme: wheat background with teal (#098a9e) accents
- Print-optimized CSS for PDF exports

## Recent Enhancements (Completed)

All technical debt has been resolved:
- ✅ Added proper `<html lang="en">` tag and document structure
- ✅ Added viewport meta tag for mobile responsiveness
- ✅ Implemented consistent indentation and formatting
- ✅ Created .gitignore file to exclude system artifacts
- ✅ Moved footer outside section tags for semantic correctness
- ✅ Enhanced CSS with responsive design and modern styling
- ✅ Added accessibility features (ARIA labels, semantic HTML)
- ✅ Implemented SEO improvements (meta description, structured data)
- ✅ Repository reorganized with clean structure

## Implementation Plans

Detailed implementation plans are located in `.claude/tasks/`:
- `project-setup-and-improvements.md` - Comprehensive plan for git cleanup, code improvements, and documentation

## Testing Checklist

Before committing changes:
- [ ] Open index.html in multiple browsers (Chrome, Firefox, Safari)
- [ ] Test on mobile device or use browser dev tools responsive mode
- [ ] Verify all links work (GitHub profile, AWS certification)
- [ ] Verify images load correctly (favicon.png, Omar Gad.JPG)
- [ ] Check for console errors in browser developer tools
- [ ] Validate HTML at https://validator.w3.org/ (optional)

## Deployment

This is a static site suitable for deployment on:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service
- University web server (if applicable)

No build process required - just upload the files.
