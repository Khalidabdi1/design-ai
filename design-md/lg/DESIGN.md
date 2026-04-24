# LG Design System

> Consumer electronics and appliances with deep red branding, glossy product presentation, and broad lifestyle-tech merchandising. LG's public site uses white and dark surfaces, a burgundy-red accent, and premium home-tech imagery.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
LG feels like **consumer electronics and home appliances presented with premium mainstream polish**.
### Mood & Feeling
- Premium
- Mainstream
- Home-tech
- Broad
- Product-first
### Design Density
**Medium density.** Product lines are broad, but organized through strong imagery and category bands.
### Visual Character
- White and dark sections
- Burgundy/red brand cues
- Appliance and electronics hero imagery
- Broad product merchandising

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--lg-red` | `#A50034` | Primary brand accent |
| `--lg-black` | `#111111` | Text and dark framing |
| `--lg-white` | `#FFFFFF` | Main surface |
| `--lg-surface` | `#F7F7F7` | Background |
| `--lg-muted` | `#6B7280` | Secondary text |
| `--lg-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "LG Smart", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "LG Smart", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `50/700`, H1 `36/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#a50034; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Organize by product family and room/appliance context
- Use premium imagery to drive interest
- Keep category breadth controlled

## 6. Depth & Elevation
LG uses **light premium retail framing** with imagery-driven emphasis.

## 7. Do's and Don'ts
### Do
- Keep it premium but accessible
- Use burgundy-red as a precise brand anchor
- Preserve home-tech breadth
### Don't
- Don’t overdecorate beyond product imagery
- Don’t lose retail scanability

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack product modules and maintain category discoverability

## 9. Agent Prompt Guide
```text
Design this like LG: premium home-tech retail UI with white and dark sections, burgundy-red brand accents, product-first hero imagery, and broad but clean category merchandising.
```
