# Miro Design System

> Collaborative whiteboard software with bright yellow branding and board-first visual structure. Miro's public site pairs white surfaces, dark text, vivid yellow (`#FFD02F`), and board-like product demos that emphasize teamwork and ideation.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Miro feels like **collaboration and ideation turned into a polished, visual workspace**.
### Mood & Feeling
- Collaborative
- Bright
- Inventive
- Structured
- Workshop-friendly
### Design Density
**Medium density.** Board demos contain lots of information, but the page framing stays simple.
### Visual Character
- Yellow brand punch
- White and light-gray surfaces
- Board-like product previews
- Friendly collaborative diagrams

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--miro-yellow` | `#FFD02F` | Primary brand accent |
| `--miro-black` | `#111111` | Text and CTA |
| `--miro-white` | `#FFFFFF` | Main surface |
| `--miro-surface` | `#F7F7F7` | Soft background |
| `--miro-ink` | `#1F2937` | Text |
| `--miro-muted` | `#6B7280` | Secondary text |
| `--miro-border` | `#E5E7EB` | Borders |
| `--miro-blue-soft` | `#EAF1FF` | Support tint |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Roobert", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Roobert", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use strong, friendly, workshop-ready typography with clear visual hierarchy.

## 4. Component Stylings
```css
.button-primary { background:#111; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e7eb; border-radius:999px; min-height:46px; padding:0 20px; }
.board-card { background:#fff; border:1px solid #e5e7eb; border-radius:24px; box-shadow:0 12px 24px rgba(17,17,17,.06); }
.chip { background:#ffd02f; color:#111; border-radius:999px; padding:6px 12px; }
```
### Component Notes
- Product previews should feel like real boards
- Yellow is a high-recognition accent, not a blanket background

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Use large board demos and collaborative workflow stories
- Keep feature modules visual and concrete
- Let teamwork use cases drive the page order

## 6. Depth & Elevation
Miro uses **card and board elevation** with soft shadows and bright contrast.

## 7. Do's and Don'ts
### Do
- Keep it collaborative and visually organized
- Use yellow as a memorable brand accent
- Preserve board realism and workshop energy
### Don't
- Don’t reduce the experience to generic enterprise project management
- Don’t overuse decorative gradients

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack board demos vertically
- Maintain legible collaboration artifacts and labels

## 9. Agent Prompt Guide
```text
Design this like Miro: bright collaborative whiteboard SaaS with yellow brand accents, real board-style demo cards, friendly strong typography, and visual teamwork workflows on clean white surfaces.
```
