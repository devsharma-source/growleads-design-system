# Layout System

## Page Structure

```
┌──────────────────────────────────────────────────┐
│  Sidebar (240px, fixed)  │  Main Content          │
│                          │                        │
│  ┌─ Brand ─────────────┐ │  ┌─ Page Header ──────┐│
│  │ Logo + "Growleads"  │ │  │ Title + Subtitle   ││
│  └─────────────────────┘ │  │ + Status badge     ││
│                          │  │ (gradient bg)      ││
│  ┌─ Nav Section ───────┐ │  └────────────────────┘│
│  │ OVERVIEW            │ │                        │
│  │  Dashboard          │ │  ┌─ Filter Bar ───────┐│
│  │  Reactions          │ │  │ Buttons / filters  ││
│  │  Sessions           │ │  │ (gradient bg)      ││
│  │                     │ │  └────────────────────┘│
│  │ CONFIGURATION       │ │                        │
│  │  Keywords           │ │  ┌─ Page Body ────────┐│
│  │  Settings           │ │  │ Content here       ││
│  └─────────────────────┘ │  │ padding: 24px 32px ││
│                          │  │                    ││
│  ┌─ Footer ────────────┐ │  │                    ││
│  │ Login to LinkedIn   │ │  │                    ││
│  └─────────────────────┘ │  └────────────────────┘│
└──────────────────────────────────────────────────┘
```

## Sidebar

```css
width: 240px;
background: #111426;             /* bg-secondary */
border-right: 1px solid #1e2235;
position: fixed;
top: 0; left: 0; bottom: 0;

/* Brand area */
padding: 20px 20px 24px;
border-bottom: 1px solid #1e2235;

/* Logo */
width: 32px; height: 32px;
background: #2563eb;
border-radius: 0.5rem;
font-weight: 700; font-size: 14px; color: white;

/* Nav section */
padding: 12px 8px;

/* Section label */
padding: 16px 12px 6px;
font-size: 11px; text-transform: uppercase;
color: #5c6080; letter-spacing: 0.5px;

/* Nav item */
padding: 8px 12px;
border-radius: 0.5rem;
font-size: 13px; font-weight: 500;
color: #5c6080;
/* hover */ background: #1a1e2e; color: #e2e4f0;
/* active */ background: rgba(59, 130, 246, 0.12); color: #60a5fa;

/* Icon in nav item */
width: 18px; height: 18px;
stroke: currentColor; stroke-width: 2;
opacity: 0.7; /* active: 1 */

/* Footer */
padding: 12px 8px;
border-top: 1px solid #1e2235;
```

## Main Content

```css
margin-left: 240px;              /* sidebar width */
min-height: 100vh;
```

## Page Header

```css
background: linear-gradient(180deg, #161929 0%, #111426 100%);
border-bottom: 1px solid #1e2235;
padding: 24px 32px 20px;
```

## Filter Bar

```css
background: linear-gradient(180deg, #111426 0%, #0c0e1a 100%);
border-bottom: 1px solid #1e2235;
padding: 12px 32px;
display: flex; align-items: center; gap: 8px;
```

## Page Body

```css
padding: 24px 32px;
```

## Stat Grid

```css
display: grid;
grid-template-columns: repeat(4, 1fr);  /* 2 on mobile */
gap: 16px;
margin-bottom: 24px;
```

## Two-Column Grid

```css
display: grid;
grid-template-columns: 1fr 1fr;  /* 1fr on mobile */
gap: 16px;
```

## Spacing Scale

```
4px    Tight gap (icon to text in badge)
6px    Tag gap, chart bar gap
8px    Small gap (button group, nav items, tags)
10px   Medium gap (sidebar item icon-to-text, hbar row gap)
12px   Card internal section gap, sidebar nav padding
16px   Grid gap, card padding (tight), form group spacing
20px   Card padding (standard), card header padding
24px   Page body padding (top/bottom), section spacing
32px   Page body padding (left/right)
```

## Responsive Breakpoints

```
≤ 900px:
  - Sidebar hidden (off-canvas, toggleable)
  - Main content: margin-left: 0
  - Page padding: 20px
  - Stat grid: 2 columns

≤ 500px:
  - Stat values: 22px
  - Button groups: vertical stack
  - Page padding: 16px
```

## Mobile Sidebar

```css
/* Hidden by default on mobile */
.sidebar { transform: translateX(-100%); transition: transform 0.2s ease; }
.sidebar.open { transform: translateX(0); }
```
