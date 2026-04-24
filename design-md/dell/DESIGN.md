# Dell Design System

> Technology retail and enterprise computing with blue trust cues and hardware-led commerce. Dell's public site uses white surfaces, blue branding, and broad hardware/category merchandising.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Dell feels like **enterprise-capable hardware commerce with mainstream technology trust**.
### Mood & Feeling
- Practical
- Tech-forward
- Enterprise-friendly
- Commerce-oriented
- Trustworthy
### Design Density
**Medium to high density.** Hardware choices and promos are broad, but structured.
### Visual Character
- White retail-tech surfaces
- Blue brand anchor
- Product and hardware modules
- Clean merchandising

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--dell-blue` | `#0076CE` | Primary brand accent |
| `--dell-white` | `#FFFFFF` | Main surface |
| `--dell-surface` | `#F5F8FB` | Background |
| `--dell-ink` | `#111827` | Text |
| `--dell-muted` | `#6B7280` | Secondary text |
| `--dell-border` | `#DCE5F0` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Roboto", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Roboto", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#0076ce; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111827; border:1px solid #dce5f0; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #dce5f0; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Organize by device line and customer type
- Keep promos, categories, and enterprise options cleanly separated

## 6. Depth & Elevation
Dell uses **light commerce-card depth** with strong border clarity.

## 7. Do's and Don'ts
### Do
- Keep it trustworthy and hardware-first
- Use blue as the stable technology cue
- Preserve product-family hierarchy
### Don't
- Don’t over-style the experience beyond the products
- Don’t crowd major category paths

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack product modules and keep category browsing obvious

## 9. Agent Prompt Guide
```text
Design this like Dell: white and blue technology-commerce UI with clean hardware merchandising, practical product-family structure, and enterprise-friendly trust cues.
```
