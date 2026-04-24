# Best Buy Design System

> Electronics retail with strong blue-yellow branding and high-visibility merchandising. Best Buy's public site uses a vivid cobalt blue foundation, bright yellow branding, white content surfaces, and dense retail promotion modules.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Best Buy feels like **electronics retail with big merchandising energy and high-contrast brand recognition**.
### Mood & Feeling
- Promotional
- Utility-focused
- Mainstream retail
- Tech-commerce
- Bold
### Design Density
**High density.** Promotions, product shelves, and categories are tightly packed.
### Visual Character
- Bright blue brand frame
- Yellow labels and highlights
- White promo cards
- Dense merchandising modules

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--bb-blue` | `#0046BE` | Primary brand anchor |
| `--bb-yellow` | `#FFF200` | Highlight / promo |
| `--bb-white` | `#FFFFFF` | Cards and surfaces |
| `--bb-surface` | `#F3F6FB` | Background |
| `--bb-ink` | `#111827` | Text |
| `--bb-muted` | `#6B7280` | Secondary text |
| `--bb-border` | `#DCE5F5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Human BBY", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Human BBY", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use strong, retail-readable typography that supports promotions and category browsing.

## 4. Component Stylings
```css
.button-primary { background:#0046be; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #dce5f5; border-radius:999px; min-height:44px; padding:0 18px; }
.promo-card { background:#fff; border:1px solid #dce5f5; border-radius:16px; }
.badge { background:#fff200; color:#111; border-radius:999px; padding:6px 10px; font-weight:700; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Prioritize promotions, deals, and categories
- Keep retail shelves easy to scan
- Use blue and yellow for strong brand recognition

## 6. Depth & Elevation
Best Buy uses **retail-card separation** more than premium shadow depth.

## 7. Do's and Don'ts
### Do
- Keep it promotional and immediately scannable
- Use blue and yellow decisively
- Preserve retail shelf and category clarity
### Don't
- Don’t over-minimalize it into boutique ecommerce
- Don’t reduce promo emphasis too much

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack promo modules and keep deal CTA visible
- Preserve readable shelf structure

## 9. Agent Prompt Guide
```text
Design this like Best Buy: bold electronics-retail UI with cobalt blue framing, yellow promo highlights, white merchandising cards, dense category browsing, and mainstream high-visibility commerce energy.
```
