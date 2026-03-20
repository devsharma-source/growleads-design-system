# Growleads Design System

The official design system for all Growleads products. Extracted from [dashboard.growleads.io](https://dashboard.growleads.io) — contains every color, font, spacing value, and component spec needed to build consistent UIs across projects.

## Quick Start

### Option 1: Copy the CSS tokens

Drop `tokens.css` into your project and import it:

```html
<link rel="stylesheet" href="tokens.css">
```

Or import in your CSS:

```css
@import url('./tokens.css');
```

This gives you all CSS custom properties (`--bg-primary`, `--blue-500`, etc.) ready to use.

### Option 2: Use the full reference CSS

Copy `reference.css` for a complete, production-ready stylesheet that includes the sidebar layout, all components, responsive breakpoints, and the custom scrollbar.

### Option 3: Use with AI coding tools (Claude Code, Cursor, etc.)

Clone this repo, then tell your AI assistant:

```
Read the design system from /path/to/growleads-design-system/ and apply it to this project
```

The AI will read the spec files and build UI matching the Growleads style automatically.

## Files

| File | What | When to use |
|------|------|-------------|
| **`tokens.css`** | CSS custom properties (colors, radius, shadows, spacing) | Every project — import this first |
| **`colors.md`** | Full color palette, badge opacity rules, gradients, focus rings | Reference when picking colors |
| **`typography.md`** | Inter font, size/weight scale for every element type | Reference when styling text |
| **`components.md`** | Exact CSS for buttons, inputs, cards, tables, badges, toggles, charts | Reference when building components |
| **`layout.md`** | Sidebar + main content structure, spacing scale, breakpoints | Reference when structuring pages |
| **`reference.css`** | Complete production CSS (everything above, ready to use) | Starting point for new projects |

## Color Palette

### Surfaces (dark theme)

| Token | Hex | Usage |
|-------|-----|-------|
| `--bg-primary` | `#0c0e1a` | Page background |
| `--bg-secondary` | `#111426` | Sidebar, cards, inputs |
| `--bg-card` | `#161929` | Elevated cards, header gradients |
| `--bg-hover` | `#1a1e2e` | Hover states |
| `--border-color` | `#1e2235` | All borders and dividers |

### Text

| Token | Hex | Usage |
|-------|-----|-------|
| `--text-primary` | `#e2e4f0` | Headings, body text, values |
| `--text-muted` | `#5c6080` | Labels, placeholders, secondary |

### Brand & Semantic

| Token | Hex | Usage |
|-------|-----|-------|
| `--blue-600` | `#2563eb` | Primary button |
| `--blue-500` | `#3b82f6` | Primary hover, focus ring, active |
| `--green-500` | `#22c55e` | Success, running |
| `--red-500` | `#ef4444` | Error, danger |
| `--amber-500` | `#f59e0b` | Warning |
| `--violet-500` | `#8b5cf6` | Accent |

## Typography

```
Font:    Inter (Google Fonts)
Base:    13px / 1.5
Mono:    SF Mono, ui-monospace, Menlo, Monaco, Consolas
```

| Element | Size | Weight |
|---------|------|--------|
| Page title | 20px | 600 |
| Card title | 14px | 600 |
| Body / cells | 13px | 400 |
| Buttons | 13px | 500 |
| Badges | 12px | 500 |
| Table headers | 11px | 500 (uppercase) |
| Stat values | 28px | 700 |

## Key Design Rules

### Badge Pattern
All badges use **12% opacity** of the semantic color as background, with the lighter color variant as text, and `border-radius: 9999px`:
```css
background: rgba(59, 130, 246, 0.12);  /* 12% of blue */
color: #60a5fa;                         /* blue-400 (lighter) */
border-radius: 9999px;
```

### Focus Ring
```css
border-color: #3b82f6;
box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.12);
```

### Gradients
```css
/* Page header */
background: linear-gradient(180deg, #161929 0%, #111426 100%);

/* Filter bar */
background: linear-gradient(180deg, #111426 0%, #0c0e1a 100%);
```

### Buttons
Height `32px`, padding `0 16px`, border-radius `0.5rem`, font `13px/500`. Primary is `blue-600` with `blue-500` hover.

## Using with AI Assistants

This repo is specifically structured so AI coding tools can read it and produce pixel-accurate UI. The key files for AI consumption are:

1. **`tokens.css`** — Machine-readable CSS variables
2. **`components.md`** — Copy-paste-ready CSS blocks for every component
3. **`layout.md`** — ASCII diagram + exact CSS for page structure

### Recommended prompt

```
Read all files in the growleads-design-system folder.
Use tokens.css for variables, components.md for component specs,
and layout.md for page structure. Build [describe what you need].
```

## Font Setup

Add to your HTML `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

## License

Internal use only — Growleads team.
