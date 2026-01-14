# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A simple TODO application built as a single-page HTML file with no external dependencies. Uses vanilla JavaScript and localStorage for data persistence.

## Development

Open `index.html` directly in a browser:
```bash
open index.html
```

No build process, package manager, or server required.

## Architecture

Single file (`index.html`) containing:
- **CSS** (lines 7-254): Embedded styles with responsive design, gradient theme, and transitions
- **HTML** (lines 256-276): Semantic structure with input, filters, todo list, and stats sections
- **JavaScript** (lines 279-423): State management and rendering

### Data Model

Todos are stored in localStorage as JSON array with structure:
```javascript
{ id: string, text: string, completed: boolean, createdAt: number }
```

### Key Functions

- `render()` - Main render function, re-renders entire todo list based on current state and filter
- `saveTodos()` - Persists state to localStorage
- `escapeHtml()` - XSS prevention for user input
