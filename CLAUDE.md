# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Spendly is a Flask-based expense tracking web application. The project is currently in early development with UI scaffolding in place and backend functionality partially implemented.

## Development Commands

**Run the development server:**
```bash
python app.py
```
The server starts on port 5001 with debug mode enabled.

**Install dependencies:**
```bash
pip install -r requirements.txt
```

**Run tests:**
```bash
pytest
```

## Architecture

**Tech Stack:**
- Backend: Flask 3.1.3 with Jinja2 templating
- Styling: Custom CSS (no framework)
- Fonts: DM Serif Display and DM Sans from Google Fonts
- Testing: pytest with pytest-flask

**Project Structure:**

- `app.py` — Main Flask application with route definitions. Currently contains placeholder routes for features not yet implemented (logout, profile, expense CRUD operations).
- `database/` — Contains `__init__.py` (currently empty). Database initialization code is planned but not yet implemented.
- `templates/` — Jinja2 templates using template inheritance:
  - `base.html` — Base layout with navigation and footer
  - `landing.html` — Marketing homepage with YouTube modal demo
  - `login.html` / `register.html` — Authentication forms (UI only, not wired up)
  - `terms.html` / `privacy.html` — Static legal pages
- `static/css/` — Stylesheets: `style.css` (global styles), `landing.css` (landing page specific)
- `static/js/` — `main.js` (minimal, global scripts)

**Routing Convention:**
Routes are defined in `app.py` using Flask's `@app.route()` decorator. URL names use lowercase with hyphens for multi-word paths. Routes are organized by feature area (auth, expenses, etc.).

**Styling Approach:**
- CSS uses CSS custom properties for theming (defined in `style.css`)
- Component-based CSS classes (e.g., `.btn-primary`, `.auth-card`)
- Mobile-first responsive design
- Currency displayed in Indian Rupees (₹)

**Development Notes:**
- Port 5001 is hardcoded in `app.py`
- Virtual environment (`venv/`) should be activated before running
- Several routes return placeholder strings indicating future implementation steps
