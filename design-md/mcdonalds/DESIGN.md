# McDonald's Design System

> Fast-food commerce with strong red-and-yellow branding, friendly utility, and mainstream consumer accessibility. McDonald's public site uses bright brand color, white space, large food imagery, and clear app/deal CTAs.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
McDonald's feels like **global fast-food branding turned into a familiar, mobile-friendly digital ordering and offer interface**.
### Mood & Feeling
- Friendly
- Bold
- Accessible
- Promotional
- Mainstream
### Design Density
**Medium density.** Deals, food categories, and app benefits are clear and direct.
### Visual Character
- Bright red and yellow identity
- White support surfaces
- Large food imagery
- Simple offer and app-focused modules

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--mcd-red` | `#DA291C` | Primary brand anchor |
| `--mcd-yellow` | `#FFC72C` | Highlight and brand support |
| `--mcd-white` | `#FFFFFF` | Main surface |
| `--mcd-black` | `#111111` | Text |
| `--mcd-muted` | `#666666` | Secondary text |
| `--mcd-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Speedee", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `52/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#da291c; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#ffc72c; color:#111; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:18px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Lead with offers, app benefits, and menu highlights
- Keep ordering and location actions clear
- Use food imagery generously but simply

## 6. Depth & Elevation
McDonald's uses **light consumer-card framing** with direct promotional hierarchy.

## 7. Do's and Don'ts
### Do
- Keep it bold, friendly, and mobile-order ready
- Use red and yellow with confidence
- Preserve promotional clarity
### Don't
- Don’t overcomplicate with gourmet editorial minimalism
- Don’t hide app or deal CTAs

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep app/order/deals actions near the top
- Stack food promos clearly and maintain strong imagery

## 9. Agent Prompt Guide
```text
Design this like McDonald's: bold red-and-yellow fast-food UI with white support surfaces, large food imagery, simple offer cards, and strong app-and-order consumer clarity.
```
