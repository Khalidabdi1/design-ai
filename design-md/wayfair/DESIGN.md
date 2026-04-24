# Wayfair Design System

> Home furnishings retail with broad catalog density, warm merchandising, and soft home-oriented polish. Wayfair's public site uses a white base, dark text, subtle category framing, and the Wayfair purple identity across a very broad home-goods catalog.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Wayfair feels like **home shopping at marketplace scale with catalog breadth and aspirational room styling**.
### Mood & Feeling
- Home-focused
- Broad
- Comfortable
- Promotional
- Mainstream decor retail
### Design Density
**High density.** Catalog depth is large, but categories and sale messaging keep orientation intact.
### Visual Character
- White and soft-neutral surfaces
- Purple brand accent
- Dense home-category navigation
- Lifestyle and room-based merchandising

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--wayfair-purple` | `#7B189F` | Brand accent |
| `--wayfair-white` | `#FFFFFF` | Main surface |
| `--wayfair-surface` | `#F8F7F5` | Soft background |
| `--wayfair-ink` | `#1F2937` | Text |
| `--wayfair-muted` | `#6B7280` | Secondary text |
| `--wayfair-border` | `#E5E7EB` | Borders |
| `--wayfair-sale` | `#C74634` | Sale/urgency accent |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use clear home-retail typography with strong category and product browsing support.

## 4. Component Stylings
```css
.button-primary { background:#7b189f; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#1f2937; border:1px solid #e5e7eb; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e7eb; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Keep room-based and category-based browsing obvious
- Balance sale messaging with home inspiration
- Support catalog depth without losing comfort

## 6. Depth & Elevation
Wayfair uses **light catalog-card framing** with minimal shadow and strong merchandising hierarchy.

## 7. Do's and Don'ts
### Do
- Keep it broad, home-focused, and retail-clear
- Use purple as a brand anchor and sale accents selectively
- Preserve room/category browsing logic
### Don't
- Don’t over-minimalize the catalog experience
- Don’t turn it into luxury editorial furniture design

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack home category and sale modules
- Keep search and major merchandising paths easy to reach

## 9. Agent Prompt Guide
```text
Design this like Wayfair: broad home-furnishings retail UI with white surfaces, soft neutrals, purple brand accents, dense category browsing, and room-based merchandising clarity.
```
