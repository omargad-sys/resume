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

- Main branch: `master`
- Remote: https://github.com/omargad-sys/javascript-assignment-2.git

## Code Style Notes

- The HTML uses semantic `<section>` tags for content organization
- External links use anchor tags (GitHub profile, AWS certification)
- Profile picture is sized at 75x75 pixels
- Color scheme: wheat background with teal (#098a9e) headings

## Current State and Known Issues

### Git Repository Status
- Branch: `main` (local) diverged from `origin/main`
  - Local has 13 commits, remote has 2 commits ahead
  - Files were reorganized from parent directory to current subdirectory
  - Untracked files need to be staged and committed
- Note: Repository URL references "javascript-assignment-2" but contains resume project

### Technical Debt
- Missing `<html>` opening tag in index.html
- Missing viewport meta tag (affects mobile responsiveness)
- Inconsistent indentation in HTML file
- No .gitignore file (tracks .DS_Store and other artifacts)
- Footer is inside a section tag (should be outside for semantic correctness)

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
