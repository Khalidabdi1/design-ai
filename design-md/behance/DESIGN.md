# Behance Design System

> Creative portfolio discovery with Adobe-adjacent polish, white gallery surfaces, and strong project framing. Behance's public site uses a white and light-gray base, dark text, blue Adobe-style action accents, and dense creative-grid browsing.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Behance feels like **creative discovery at marketplace scale**. The product is gallery-first, but still polished and structured.
### Mood & Feeling
- Creative
- Gallery-driven
- Professional
- Broad
- Discoverable
### Design Density
**High density.** Project grids are visually dense, but filtering and whitespace keep them usable.
### Visual Character
- White gallery background
- Dense portfolio tiles
- Simple utility chrome
- Adobe-style blue action accents

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--behance-blue` | `#1769FF` | Primary action |
| `--behance-black` | `#111111` | Text |
| `--behance-white` | `#FFFFFF` | Main surface |
| `--behance-surface` | `#F5F5F5` | Background |
| `--behance-muted` | `#6B6B6B` | Secondary text |
| `--behance-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Adobe Clean", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Adobe Clean", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use neutral creative-platform typography that supports portfolios and filters rather than dominating them.

## 4. Component Stylings
```css
.button-primary { background:#1769ff; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.tile { background:#fff; border-radius:16px; overflow:hidden; }
.filter-chip { background:#fff; border:1px solid #e5e5e5; border-radius:999px; padding:8px 12px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Let project imagery dominate
- Keep discovery, filters, and categories easy to scan
- Avoid heavy chrome around portfolio content

## 6. Depth & Elevation
Behance uses **gallery-style minimal elevation**, relying more on image tiles and spacing than shadow.

## 7. Do's and Don'ts
### Do
- Keep portfolios and creative imagery central
- Use blue for actions and navigation cues
- Preserve dense but clean discovery grids
### Don't
- Don’t overdecorate the frame around projects
- Don’t make Behance feel like generic SaaS admin UI

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Preserve grid legibility
- Keep filter chips usable and scrollable

## 9. Agent Prompt Guide
```text
Design this like Behance: white creative-gallery UI with Adobe-style blue actions, dense project discovery grids, light filter chips, and portfolio-first visual hierarchy.
```
