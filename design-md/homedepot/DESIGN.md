# Home Depot Design System

> Home improvement retail with vivid orange branding and highly practical commerce structure. Home Depot's public site uses strong orange (`#F96302`), white surfaces, black text, and tool-and-project-oriented shopping modules.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Home Depot feels like **project-driven home improvement retail with strong utilitarian energy**.
### Mood & Feeling
- Practical
- Rugged
- Retail-direct
- Project-oriented
- High-visibility
### Design Density
**High density.** Tools, categories, and promos are packed tightly for shopping utility.
### Visual Character
- Orange brand anchor
- White retail surfaces
- Dense category and promo modules
- DIY and contractor-oriented browsing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--hd-orange` | `#F96302` | Primary brand and promo accent |
| `--hd-black` | `#111111` | Text and contrast |
| `--hd-white` | `#FFFFFF` | Main surface |
| `--hd-surface` | `#F7F7F7` | Background |
| `--hd-muted` | `#666666` | Secondary text |
| `--hd-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Helvetica Neue", Arial, sans-serif;
--font-sans: "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `48/700`, H1 `34/700`, H2 `26/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use strong retail typography optimized for project search and product scanability.

## 4. Component Stylings
```css
.button-primary { background:#f96302; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:14px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Keep category and project entry points highly visible
- Support deal, tool, and home-upgrade browsing
- Use orange for urgency and brand recognition

## 6. Depth & Elevation
Home Depot uses **retail card framing** more than premium elevation.

## 7. Do's and Don'ts
### Do
- Keep it practical and high-visibility
- Use orange boldly but purposefully
- Preserve project-based category hierarchy
### Don't
- Don’t make it feel boutique or lifestyle-first
- Don’t hide shopping flows under decorative imagery

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep search and category access obvious
- Stack dense promo modules cleanly

## 9. Agent Prompt Guide
```text
Design this like Home Depot: practical orange-led home-improvement retail UI with white cards, high-visibility category access, project-driven shopping hierarchy, and rugged straightforward ecommerce structure.
```
