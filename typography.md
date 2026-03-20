# Typography

## Font Stack

```css
font-family: 'Inter', system-ui, -apple-system, sans-serif;
```

Load via Google Fonts:
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

## Monospace (code, logs)

```css
font-family: 'SF Mono', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
```

## Base

```
Font size:    13px
Line height:  1.5
Smoothing:    -webkit-font-smoothing: antialiased
```

## Scale

| Element | Size | Weight | Color | Extra |
|---------|------|--------|-------|-------|
| Page title | 20px | 600 | text-primary | — |
| Page subtitle | 13px | 400 | text-muted | — |
| Card title | 14px | 600 | text-primary | — |
| Section header | 12px | 500 | text-muted | uppercase, letter-spacing: 0.5px |
| Sidebar section label | 11px | 500 | text-muted | uppercase, letter-spacing: 0.5px |
| Sidebar item | 13px | 500 | text-muted (active: blue-400) | — |
| Body / table cell | 13px | 400 | text-primary | — |
| Table header | 11px | 500 | text-muted | uppercase, letter-spacing: 0.5px |
| Button | 13px | 500 | white / contextual | — |
| Badge | 12px | 500 | contextual | — |
| Input | 13px | 400 | text-primary | placeholder: text-muted |
| Stat value | 28px | 700 | text-primary | font-variant-numeric: tabular-nums |
| Stat label | 12px | 500 | text-muted | uppercase, letter-spacing: 0.3px |
| Stat detail | 12px | 400 | text-muted | — |
| Chart value | 11px | 600 | text-primary | tabular-nums |
| Chart label | 11px | 500 | text-muted | — |
| Toast | 13px | 500 | white | — |
| Footer/description | 12px | 400 | text-muted | line-height: 1.4 |
| Log text | 12px | 400 | text-muted | monospace, line-height: 1.6 |

## Weight Map

```
400  Regular    Body text, descriptions, input values
500  Medium     Labels, buttons, sidebar items, badges, table headers
600  Semibold   Titles, card headers, section headers, stat labels
700  Bold       Stat values, brand name
```
