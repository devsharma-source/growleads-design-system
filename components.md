# Component Specifications

## Buttons

### Primary
```css
height: 32px;
padding: 0 16px;
background: #2563eb;              /* blue-600 */
color: white;
border: none;
border-radius: 0.5rem;            /* 8px */
font-size: 13px;
font-weight: 500;
transition: all 0.15s ease;
/* hover */ background: #3b82f6;   /* blue-500 */
/* disabled */ opacity: 0.4;
```

### Secondary
```css
background: #161929;              /* bg-card */
color: #e2e4f0;                   /* text-primary */
border: 1px solid #1e2235;        /* border-color */
/* hover */ background: #1a1e2e;   /* bg-hover */
```

### Success
```css
background: #22c55e;
/* hover */ background: #4ade80;
```

### Danger
```css
background: #ef4444;
/* hover */ background: #f87171;
```

### Ghost
```css
background: transparent;
color: #5c6080;                   /* text-muted */
height: auto;
padding: 4px 8px;
/* hover */ color: #e2e4f0;
```

## Inputs

```css
padding: 7px 12px;
background: #111426;              /* bg-secondary */
border: 1px solid #1e2235;        /* border-color */
border-radius: 0.5rem;
color: #e2e4f0;
font-size: 13px;
/* placeholder */ color: #5c6080;
/* focus */
  border-color: #3b82f6;
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.12);
```

### Settings-style inline input
```css
/* Row container */
display: flex;
align-items: center;
justify-content: space-between;
padding: 10px 16px;
border-bottom: 1px solid #1e2235;

/* Input within row */
width: 160px;
text-align: right;
background: #0c0e1a;             /* bg-primary — one step darker than card */
```

## Textarea

```css
min-height: 80px;
resize: vertical;
line-height: 1.5;
/* Same border/focus/color as input */
```

## Cards

```css
background: #111426;              /* bg-secondary */
border: 1px solid #1e2235;
border-radius: 0.75rem;           /* 12px */
overflow: hidden;
```

### Card with header
```css
/* Header */
display: flex;
justify-content: space-between;
align-items: center;
padding: 16px 20px;
border-bottom: 1px solid #1e2235;

/* Body (when padded) */
padding: 20px;
```

## Tables

```css
/* Header row */
background: rgba(22, 25, 41, 0.5);
font-size: 11px;
font-weight: 500;
color: #5c6080;
text-transform: uppercase;
letter-spacing: 0.5px;
padding: 10px 16px;

/* Body cell */
font-size: 13px;
color: #e2e4f0;
padding: 10px 16px;
border-bottom: 1px solid #1e2235;

/* Row hover */
background: #1a1e2e;

/* Last row */
border-bottom: none;
```

## Badges / Status Pills

```css
display: inline-flex;
align-items: center;
gap: 5px;
padding: 2px 10px;
border-radius: 9999px;
font-size: 12px;
font-weight: 500;
```

| State | Background | Text |
|-------|-----------|------|
| Running / Completed | `rgba(34, 197, 94, 0.12)` | `#4ade80` |
| Idle | `rgba(92, 96, 128, 0.15)` | `#a1a1aa` |
| Error | `rgba(239, 68, 68, 0.12)` | `#f87171` |
| Warning | `rgba(245, 158, 11, 0.12)` | `#fbbf24` |

### Dot indicator inside badge
```css
width: 6px;
height: 6px;
border-radius: 50%;
background: currentColor;
/* Running state animates with pulse */
```

## Tags (keyword chips)

```css
padding: 3px 10px;
background: rgba(59, 130, 246, 0.12);
color: #60a5fa;                   /* blue-400 */
border-radius: 9999px;
font-size: 12px;
font-weight: 500;
```

## Toggle Switch

```css
/* Container */
width: 40px;
height: 22px;

/* Track (off) */
background: #1e2235;              /* border-color */
border-radius: 11px;

/* Track (on) */
background: #3b82f6;              /* blue-500 */

/* Thumb */
width: 18px;
height: 18px;
background: white;
border-radius: 50%;
box-shadow: 0 1px 3px rgba(0, 0, 0, 0.3);
/* on */ transform: translateX(18px);
transition: transform 0.2s ease;
```

## Scrollbar

```css
::-webkit-scrollbar { width: 5px; height: 5px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: #1e2235; border-radius: 99px; }
::-webkit-scrollbar-thumb:hover { background: #2e3248; }
```

## Toast Notifications

```css
position: fixed;
bottom: 24px;
right: 24px;
padding: 10px 20px;
border-radius: 0.5rem;
font-size: 13px;
font-weight: 500;
box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3), 0 4px 6px rgba(0, 0, 0, 0.2);
animation: slideUp 0.25s ease forwards;

/* Success */ background: #22c55e; color: white;
/* Error */   background: #ef4444; color: white;
```

## Charts

### Vertical bar chart
```css
/* Container */ height: 120px; display: flex; align-items: flex-end; gap: 8px;
/* Bar */ background: #3b82f6; border-radius: 3px 3px 0 0; transition: height 0.3s;
/* Label */ font-size: 11px; color: #5c6080;
/* Value */ font-size: 11px; font-weight: 600; color: #e2e4f0;
```

### Horizontal bar chart
```css
/* Track */ height: 6px; background: #1e2235; border-radius: 3px;
/* Fill */ border-radius: 3px; transition: width 0.3s;
/* Label */ width: 80px; font-size: 12px; color: #5c6080;
/* Count */ font-size: 12px; font-weight: 600; color: #e2e4f0;
```
