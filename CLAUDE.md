# AI Agent Instructions for Vite React Template

This file provides guidance for AI coding agents customizing this Vite + React template.

## Quick Start

1. **App Entry**: Edit `src/App.tsx` for main application
2. **Styling**: Edit `src/App.css` and `src/index.css` for styles
3. **Assets**: Add images to `src/assets/`

---

## Files to MODIFY (Customize These)

### Core Application
| File | Purpose |
|------|---------|
| `src/App.tsx` | Main application component |
| `src/App.css` | Application styles |
| `src/index.css` | Global styles |
| `index.html` | HTML template, page title, meta tags |

### Assets
| Location | Purpose |
|----------|---------|
| `src/assets/` | Images, fonts, static files |
| `public/` | Public static files (favicon, etc.) |

### Configuration
| File | Purpose |
|------|---------|
| `vite.config.ts` | Vite build configuration |
| `tailwind.config.js` | Tailwind CSS theme (if using) |

---

## Project Structure

```
src/
├── App.tsx          # Main app component
├── App.css          # App-specific styles
├── main.tsx         # Entry point
├── index.css        # Global styles
└── assets/          # Static assets
```

---

## Adding New Components

Create components in `src/components/`:

```tsx
// src/components/Button.tsx
export function Button({ children, onClick }) {
  return (
    <button onClick={onClick} className="btn">
      {children}
    </button>
  );
}
```

Import in App.tsx:
```tsx
import { Button } from './components/Button';
```

---

## Build and Test

```bash
# Install dependencies
npm install

# Start dev server (hot reload)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Lint code
npm run lint
```

---

## Deployment Notes

This template is configured for Netlify deployment.

**Build output**: `dist/` folder

**netlify.toml** is already configured:
- Build command: `npm run build`
- Publish directory: `dist`

For other platforms, use the same build command and publish the `dist/` folder.
