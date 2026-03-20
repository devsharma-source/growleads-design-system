# AI Assistant Instructions

This is the Growleads design system. When asked to build UI for any Growleads project:

1. Read `tokens.css` — import these CSS variables into the project
2. Read `components.md` — use exact CSS specs for buttons, inputs, cards, tables, badges, toggles
3. Read `layout.md` — use the sidebar + main content structure with gradients
4. Read `typography.md` — use Inter font with the exact size/weight scale
5. Read `colors.md` — follow the 12% opacity badge rule, gradient patterns, focus ring spec

The `reference.css` file is a complete production CSS that can be copied directly as a starting point.

Key rules:
- Dark theme only (bg: #0c0e1a)
- Inter font, 13px base
- Buttons: 32px height, 0.5rem radius
- Badges: 9999px radius, 12% opacity backgrounds
- Cards: #111426 bg, 1px #1e2235 border, 0.75rem radius
- All borders: #1e2235
- Focus: blue ring with 12% opacity shadow

Branding:
- `favicon.png` is the official logo — use it for favicons and app icons
- Sidebar logo: use the SVG recreation from `README.md` (blue-to-indigo gradient rect + white "G" + green-to-cyan arrow)
- Logo gradient: #0A84FF → #5E5CE6 (background), #30D158 → #64D2FF (arrow)
- Corner radius on logo: 9px at 40x40
