# Lenovo Design System

> Computing and device retail with black-red branding, practical hierarchy, and broad catalog structure. Lenovo's public site uses a black-white base, red brand accents, and hardware-forward merchandising.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Lenovo feels like **global device commerce with practical, high-contrast product hierarchy**.
### Mood & Feeling
- Practical
- Global-tech
- Business-capable
- Hardware-led
- Mainstream
### Design Density
**Medium to high density.** Many categories and promos are present.
### Visual Character
- Black, white, and red brand framing
- Hardware and laptop imagery
- Broad category modules
- Straightforward retail-tech presentation

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--lenovo-red` | `#E2231A` | Primary brand accent |
| `--lenovo-black` | `#111111` | Text and strong contrast |
| `--lenovo-white` | `#FFFFFF` | Main surface |
| `--lenovo-surface` | `#F7F7F7` | Background |
| `--lenovo-muted` | `#6B7280` | Secondary text |
| `--lenovo-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Lato", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Lato", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#e2231a; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:14px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Organize by brand line, use case, and buyer type
- Keep hardware and sale promotions scannable

## 6. Depth & Elevation
Lenovo uses **simple commerce-card depth** with strong contrast and clear modules.

## 7. Do's and Don'ts
### Do
- Keep it hardware-focused and practical
- Use red as the brand signal
- Preserve broad catalog hierarchy
### Don't
- Don’t turn it into abstract premium lifestyle tech
- Don’t clutter category paths

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack hardware sections and preserve category access

## 9. Agent Prompt Guide
```text
Design this like Lenovo: black-white-red technology retail UI with practical hardware merchandising, simple category structure, and broad computing-product clarity.
```
