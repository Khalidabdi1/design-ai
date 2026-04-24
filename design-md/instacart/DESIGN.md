# Instacart Design System

> Grocery marketplace with fresh green branding and a practical shopping-first interface. Instacart's public site uses white surfaces, grocery imagery, rounded shopping controls, and the signature Instacart green (`#43B02A`).

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Instacart feels like **everyday grocery shopping optimized for speed and familiarity**.
### Mood & Feeling
- Fresh
- Helpful
- Practical
- Family-friendly
- Marketplace clear
### Design Density
**Medium density.** Store, category, and cart flows are active but approachable.
### Visual Character
- Green action accents
- White cards and shopping surfaces
- Food and grocery imagery
- Rounded search and category controls

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--instacart-green` | `#43B02A` | Primary brand accent |
| `--instacart-green-deep` | `#2F8B1E` | Hover/support |
| `--instacart-white` | `#FFFFFF` | Main surface |
| `--instacart-surface` | `#F7FBF5` | Soft background |
| `--instacart-ink` | `#1F2937` | Text |
| `--instacart-muted` | `#6B7280` | Secondary text |
| `--instacart-border` | `#E1ECD9` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Averta", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Averta", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `54/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use clear, practical, mainstream consumer-commerce typography.

## 4. Component Stylings
```css
.button-primary { background:#43b02a; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#1f2937; border:1px solid #e1ecd9; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #e1ecd9; border-radius:20px; }
.search-shell { background:#fff; border:1px solid #e1ecd9; border-radius:999px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Prioritize search, stores, and category browsing
- Keep grocery imagery practical and appetizing
- Use green to orient actions and confidence

## 6. Depth & Elevation
Instacart uses **light marketplace-card elevation** with clear product and store modules.

## 7. Do's and Don'ts
### Do
- Keep it fast, fresh, and shopping-first
- Use green as a clear trust/action cue
- Preserve simple grocery discovery patterns
### Don't
- Don’t overdecorate with lifestyle flourishes
- Don’t bury store and category actions

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep search and store selection obvious
- Preserve large touch targets for shopping actions

## 9. Agent Prompt Guide
```text
Design this like Instacart: fresh green grocery-marketplace UI with white rounded cards, practical shopping controls, appetizing product imagery, and simple fast consumer-commerce flows.
```
