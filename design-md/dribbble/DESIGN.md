# Dribbble Design System

> Design discovery with soft pink branding, gallery density, and polished creative-marketplace framing. Dribbble's public site uses white space, dark text, rounded search and filter controls, and a signature pink accent.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Dribbble feels like **creative inspiration and hiring wrapped into a polished gallery marketplace**.
### Mood & Feeling
- Creative
- Friendly
- Trend-aware
- Marketplace-driven
- Design-community focused
### Design Density
**High density.** Project grids are packed, but the chrome stays soft and navigable.
### Visual Character
- White surface base
- Pink accent cues
- Dense shot galleries
- Rounded filter chips and hiring cards

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--dribbble-pink` | `#EA4C89` | Primary brand accent |
| `--dribbble-black` | `#111111` | Text |
| `--dribbble-white` | `#FFFFFF` | Canvas |
| `--dribbble-surface` | `#F8F8F8` | Background |
| `--dribbble-muted` | `#6B7280` | Secondary text |
| `--dribbble-border` | `#E5E7EB` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Mona Sans", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Mona Sans", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use modern creative-platform typography that feels polished and browseable.

## 4. Component Stylings
```css
.button-primary { background:#ea4c89; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e7eb; border-radius:999px; min-height:42px; padding:0 18px; }
.tile { background:#fff; border-radius:18px; overflow:hidden; }
.filter-chip { background:#fff; border:1px solid #e5e7eb; border-radius:999px; padding:8px 12px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Let image-heavy creative tiles dominate
- Keep search and filter systems obvious
- Support discovery, hiring, and services in one frame

## 6. Depth & Elevation
Dribbble uses **light gallery elevation** with rounded image tiles and soft chrome.

## 7. Do's and Don'ts
### Do
- Keep it gallery-first and design-community oriented
- Use pink as a compact brand accent
- Preserve soft rounded controls
### Don't
- Don’t crowd the page with heavy enterprise UI
- Don’t flatten shot cards into generic rectangles

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep shot grids legible and filters scrollable
- Preserve search and hiring CTA prominence

## 9. Agent Prompt Guide
```text
Design this like Dribbble: polished creative-gallery UI with white space, rounded image tiles, soft pink accents, modern typography, and dense but elegant discovery browsing.
```
