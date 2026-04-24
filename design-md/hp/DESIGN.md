# HP Design System

> Consumer and business computing with blue brand trust, clean hardware merchandising, and accessible technology framing. HP's public site uses white and pale-blue surfaces, product imagery, and mainstream tech-retail structure.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
HP feels like **broad-access technology retail with clean blue trust framing**.
### Mood & Feeling
- Trustworthy
- Mainstream
- Practical
- Tech-commerce
- Family-to-business broad
### Design Density
**Medium density.** Many product lines, but approachable organization.
### Visual Character
- White and soft-blue base
- Blue CTAs and links
- Hardware-led product rows
- Mainstream technology polish

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--hp-blue` | `#0096D6` | Primary accent |
| `--hp-blue-deep` | `#0073A6` | Hover/support |
| `--hp-white` | `#FFFFFF` | Main surface |
| `--hp-surface` | `#F5FAFD` | Background |
| `--hp-ink` | `#111827` | Text |
| `--hp-muted` | `#6B7280` | Secondary text |
| `--hp-border` | `#D9EAF2` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Forma DJR", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Forma DJR", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#0096d6; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #d9eaf2; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #d9eaf2; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Organize by laptops, desktops, printers, and business solutions
- Use blue as a consistent trust/action signal

## 6. Depth & Elevation
HP uses **light retail-tech card separation**.

## 7. Do's and Don'ts
### Do
- Keep it clean and broad-access
- Use blue consistently
- Preserve hardware-led merchandising
### Don't
- Don’t overcomplicate product-family navigation
- Don’t use overly flashy visual effects

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack product modules and keep category navigation easy

## 9. Agent Prompt Guide
```text
Design this like HP: clean blue-led technology retail UI with white and pale-blue surfaces, accessible hardware merchandising, and broad mainstream computing trust.
```
