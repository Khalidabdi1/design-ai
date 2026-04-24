# Monday.com Design System

> Work management with vivid color coding, polished SaaS structure, and strong product modularity. Monday.com's public site uses bright multicolor accents, white surfaces, dark text, and highly polished work-platform demos.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Monday.com feels like **structured work software with energetic visual coding**.
### Mood & Feeling
- Productive
- Bright
- Modular
- Modern
- Team-oriented
### Design Density
**Medium density.** Visual density comes from board states and tags, but page framing stays clean.
### Visual Character
- White layout with multicolor chips and status coding
- Rounded product cards
- Crisp board and workflow demos
- Confident SaaS polish

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--monday-blue` | `#006BFF` | Primary action |
| `--monday-pink` | `#FF3D71` | Accent/status |
| `--monday-green` | `#00C875` | Positive status |
| `--monday-yellow` | `#FFCB00` | Highlight/status |
| `--monday-purple` | `#784BD1` | Support accent |
| `--monday-white` | `#FFFFFF` | Main surface |
| `--monday-ink` | `#1F2430` | Text |
| `--monday-border` | `#E7EAF3` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Poppins", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Poppins", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `60/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use a clean modern sans with friendly energy and strong work-platform hierarchy.

## 4. Component Stylings
```css
.button-primary { background:#006bff; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#1f2430; border:1px solid #e7eaf3; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e7eaf3; border-radius:24px; box-shadow:0 12px 24px rgba(31,36,48,.06); }
.status-pill { border-radius:999px; padding:6px 10px; font-size:12px; font-weight:600; }
```
### Component Notes
- Board and workflow visuals should feel polished and colorful
- Multicolor status coding is core to the feel

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Organize by workflow, role, and platform outcome
- Use polished board demos and AI feature callouts
- Keep visual color coding structured, not chaotic

## 6. Depth & Elevation
Monday uses **soft SaaS elevation** around dense workflow cards.

## 7. Do's and Don'ts
### Do
- Keep it bright, modular, and work-platform clear
- Use status colors intentionally
- Preserve polished board and dashboard framing
### Don't
- Don’t flatten it into monochrome SaaS
- Don’t let colors become random decoration

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack boards and dashboards
- Preserve status visibility and CTA clarity

## 9. Agent Prompt Guide
```text
Design this like monday.com: white polished work-platform surfaces, strong blue CTA anchors, vivid status colors, rounded board demos, and modular productivity SaaS energy.
```
