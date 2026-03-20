# Color Palette

## Surface Hierarchy (darkest → lightest)

```
#0c0e1a  bg-primary      Page background, deepest layer
#111426  bg-secondary     Sidebar bg, card bg, input bg
#161929  bg-card          Elevated cards, header gradient start
#1a1e2e  bg-hover         Row hover, interactive hover state
#1e2235  border-color     All borders, dividers, table lines
#2e3248  scrollbar-hover  Scrollbar thumb hover
```

## Text

```
#e2e4f0  text-primary     All readable content, headings, values
#5c6080  text-muted       Labels, placeholders, secondary info, timestamps
```

## Brand Blue (primary actions)

```
#2563eb  blue-600    Primary button bg
#3b82f6  blue-500    Primary button hover, focus rings, active elements
#60a5fa  blue-400    Active sidebar text, links, tag text
#93c5fd  blue-300    Light blue accent (rare)
```

## Semantic Colors

| Purpose | Main | Light (badges) |
|---------|------|----------------|
| Success / Running | `#22c55e` | `#4ade80` |
| Error / Danger | `#ef4444` | `#f87171` |
| Warning / Amber | `#f59e0b` | `#fbbf24` |
| Orange | `#f97316` | `#fb923c` |

## Reaction Colors

| Reaction | Color | Badge bg |
|----------|-------|----------|
| Like | `#3b82f6` | `rgba(59, 130, 246, 0.12)` |
| Celebrate | `#f59e0b` | `rgba(245, 158, 11, 0.12)` |
| Insightful | `#8b5cf6` | `rgba(139, 92, 246, 0.12)` |
| Love | `#f43f5e` | `rgba(244, 63, 94, 0.12)` |
| Support | `#22c55e` | `rgba(34, 197, 94, 0.12)` |
| Funny | `#22d3ee` | `rgba(34, 211, 238, 0.12)` |

## Badge Pattern

All badges use the **12% opacity** rule:
- Background: `rgba([color], 0.12)`
- Text: the lighter variant of the color (e.g., `green-400` not `green-500`)
- Border-radius: `9999px` (full pill)

## Gradient Patterns

```css
/* Page header */
background: linear-gradient(180deg, #161929 0%, #111426 100%);

/* Filter bar */
background: linear-gradient(180deg, #111426 0%, #0c0e1a 100%);
```

## Focus Ring

```css
border-color: #3b82f6;
box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.12);
```
