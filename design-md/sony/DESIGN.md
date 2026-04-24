# Sony Design System

> Consumer electronics with black-and-white premium restraint and entertainment-adjacent polish. Sony's public electronics site uses dark framing, white text and surfaces, and clean premium product presentation.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Sony feels like **premium electronics presented with controlled, entertainment-aware minimalism**.
### Mood & Feeling
- Premium
- Minimal
- Polished
- Hardware-led
- Confident
### Design Density
**Medium density.** Products are broad, but layout remains composed.
### Visual Character
- Black-dominant sections
- White type and clean product cards
- Minimal accent color
- Premium device photography

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--sony-black` | `#000000` | Main contrast |
| `--sony-white` | `#FFFFFF` | Main surface and text |
| `--sony-gray` | `#F5F5F5` | Soft background |
| `--sony-ink` | `#111111` | Primary text on light |
| `--sony-muted` | `#6B7280` | Secondary text |
| `--sony-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "SST", "Helvetica Neue", Arial, sans-serif;
--font-sans: "SST", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `52/700`, H1 `38/700`, H2 `28/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#111; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Use hero photography and premium product imagery
- Keep product-family navigation restrained and clean
- Let dark sections create authority and brand presence

## 6. Depth & Elevation
Sony uses **minimal premium depth** with strong contrast and image-led hierarchy.

## 7. Do's and Don'ts
### Do
- Keep it premium, dark, and controlled
- Use minimal accents and strong imagery
- Preserve polished product framing
### Don't
- Don’t add bright, noisy SaaS color systems
- Don’t overpack the UI chrome

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Preserve hero imagery and CTA clarity
- Stack product modules cleanly

## 9. Agent Prompt Guide
```text
Design this like Sony: premium black-and-white electronics UI with minimal accent color, polished product photography, restrained typography, and clean upscale hardware presentation.
```
