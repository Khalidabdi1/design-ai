# Lowe's Design System

> Home improvement retail with deep blue trust cues, clean retail structure, and project-friendly browsing. Lowe's public site uses a blue-led brand frame, white surfaces, and straightforward shopping modules for tools, appliances, and project categories.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Lowe's feels like **practical home improvement shopping with a slightly calmer retail tone than orange-heavy competitors**.
### Mood & Feeling
- Practical
- Helpful
- Blue-trust retail
- Project-friendly
- Mainstream
### Design Density
**High density.** Many categories and promos, but framed clearly.
### Visual Character
- Deep blue brand framing
- White product and promo surfaces
- Utility-first category hierarchy
- Home project guidance modules

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--lowes-blue` | `#004990` | Primary brand accent |
| `--lowes-blue-bright` | `#0B63CE` | Support/action blue |
| `--lowes-white` | `#FFFFFF` | Main surface |
| `--lowes-surface` | `#F5F7FA` | Background |
| `--lowes-ink` | `#111827` | Text |
| `--lowes-muted` | `#6B7280` | Secondary text |
| `--lowes-border` | `#E1E7F0` | Borders |

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
Use practical, high-legibility retail type for project and product discovery.

## 4. Component Stylings
```css
.button-primary { background:#004990; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #e1e7f0; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e1e7f0; border-radius:14px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Prioritize search and major home project categories
- Keep promo and seasonal retail modules clear
- Use blue for trust and structure

## 6. Depth & Elevation
Lowe's uses **light retail separation** with borders and simple card modules.

## 7. Do's and Don'ts
### Do
- Keep it practical and project-friendly
- Use blue to anchor the experience
- Preserve clear retail hierarchy
### Don't
- Don’t overcomplicate the shopping flows
- Don’t make the visual tone too playful or luxury-coded

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep category/search access visible
- Stack retail modules before over-compressing them

## 9. Agent Prompt Guide
```text
Design this like Lowe's: blue-led home-improvement retail UI with white product cards, clear project-category browsing, practical search-first structure, and mainstream shopping clarity.
```
