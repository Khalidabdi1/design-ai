# Udemy Design System

> Course marketplace with strong category browsing, educational commerce clarity, and a dark-purple brand anchor. Udemy's public site combines white surfaces, black text, purple accents, and broad catalog navigation.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Udemy feels like **skills learning presented as a large, accessible digital marketplace**.
### Mood & Feeling
- Educational
- Commercial
- Practical
- Broad
- Mainstream
### Design Density
**Medium to high density.** Categories and offers are numerous, but the structure is familiar and retail-like.
### Visual Character
- White and light-gray base
- Purple brand accents
- Course shelves and category navigation
- Broad educational-commerce framing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--udemy-purple` | `#A435F0` | Primary brand accent |
| `--udemy-purple-deep` | `#8710D8` | Hover/support |
| `--udemy-black` | `#1C1D1F` | Text anchor |
| `--udemy-white` | `#FFFFFF` | Main surface |
| `--udemy-surface` | `#F7F9FA` | Background |
| `--udemy-muted` | `#6A6F73` | Secondary text |
| `--udemy-border` | `#D1D7DC` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Udemy Sans", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Udemy Sans", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `52/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use educational-commerce typography that supports broad browsing and trust.

## 4. Component Stylings
```css
.button-primary { background:#a435f0; color:#fff; border:none; border-radius:8px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#1c1d1f; border:1px solid #d1d7dc; border-radius:8px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #d1d7dc; border-radius:14px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Lead with category and skill discovery
- Use partner/course cards and shelves
- Keep educational trust and conversion in balance

## 6. Depth & Elevation
Udemy uses **light marketplace-card depth** with clear edges rather than heavy shadow.

## 7. Do's and Don'ts
### Do
- Keep the marketplace broad and easy to browse
- Use purple as a clear brand signal
- Preserve educational trust
### Don't
- Don’t make it overly academic and formal
- Don’t clutter card shelves with decorative noise

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep course shelves readable on mobile
- Stack dense category structures before shrinking too far

## 9. Agent Prompt Guide
```text
Design this like Udemy: white educational marketplace surfaces, purple CTA accents, broad skill-category browsing, simple course cards, and practical learning-commerce clarity.
```
