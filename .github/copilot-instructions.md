# Copilot Instructions for webapp

## Project Overview

A static website built with vanilla HTML, CSS, and JavaScript. No build tools or frameworks required.

**Tech Stack:**
- HTML5 for structure
- CSS3 with modern features (Grid, Flexbox, CSS Variables)
- Vanilla JavaScript (ES6+)
- No dependencies or build process

**Deployment:** Can be served from any static hosting (GitHub Pages, Netlify, Vercel, etc.)

## Architecture

Simple static site structure with separation of concerns:
- `index.html` - Main entry point with semantic HTML structure
- `styles.css` - All styling with mobile-first responsive design
- `script.js` - Client-side interactivity and animations

**Design Patterns:**
- CSS Grid for layout (features section)
- Intersection Observer API for scroll animations
- CSS transitions for smooth interactions

## Development Workflow

### Getting Started

```powershell
# Clone and navigate
git clone <repository-url>
cd webapp
```

### Running the Application

Open `index.html` directly in a browser, or use a local server:

```powershell
# Using Python
python -m http.server 8000

# Using Node.js (if http-server is installed)
npx http-server -p 8000

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000`

### Testing

Manual testing in browser. Check responsive design with DevTools device emulation.

## Code Conventions

### CSS Conventions
- Use semantic class names (`.hero`, `.features`, `.feature`)
- Mobile-first responsive design with `@media` queries
- CSS Grid for layouts, Flexbox for component alignment
- Smooth transitions on hover states (300ms ease)

### JavaScript Conventions
- Use `const`/`let` (no `var`)
- Modern ES6+ features (arrow functions, template literals)
- Event delegation where appropriate
- Intersection Observer for scroll animations

### HTML Structure
- Semantic HTML5 elements (`header`, `main`, `section`, `footer`)
- Accessibility: proper heading hierarchy, alt text, ARIA labels
- External CSS and JS files linked in `<head>` and before `</body>`

## Key Files

- `index.html` - Main page structure
- `styles.css` - All styling (includes responsive design)
- `script.js` - Interactive features and animations

## Common Tasks

**Add a new section:**
1. Add semantic HTML in `index.html` within `<main>`
2. Style in `styles.css` with appropriate class names
3. Add interactivity in `script.js` if needed

**Update colors:**
- Primary gradient: `#667eea` to `#764ba2` (header)
- Accent color: `#667eea` (headings)
- Adjust in `styles.css`

**Add animations:**
- Use Intersection Observer pattern (see existing `.feature` animation)
- Combine with CSS transitions for smooth effects

---

**Note:** This is a template. Update each section as the codebase develops to help AI assistants understand project-specific patterns and conventions.
