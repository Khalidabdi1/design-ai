# Zapier Design System

> Automation software with a bold orange identity, practical workflow structure, and AI workflow emphasis. Zapier's public site uses orange (`#FF4F00`), white space, dark text, and modular cards for apps, workflows, and automation tools.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Zapier feels like **workflow automation made practical, visible, and broadly useful**.
### Mood & Feeling
- Efficient
- Productive
- Platform-like
- Friendly
- Automation-first
### Design Density
**Medium density.** There are many automation concepts, but card grouping keeps the system approachable.
### Visual Character
- Orange brand anchor
- White cards and soft neutrals
- Connected workflow blocks
- App and automation module patterns

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--zapier-orange` | `#FF4F00` | Primary brand accent |
| `--zapier-orange-soft` | `#FFE6DA` | Soft support tint |
| `--zapier-white` | `#FFFFFF` | Main surface |
| `--zapier-surface` | `#FFF9F5` | Warm background |
| `--zapier-ink` | `#191919` | Text |
| `--zapier-muted` | `#667085` | Secondary text |
| `--zapier-border` | `#E8DDD5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Degular", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use straightforward modern type that makes automation concepts feel clear and usable.

## 4. Component Stylings
```css
.button-primary { background:#ff4f00; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#191919; border:1px solid #e8ddd5; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e8ddd5; border-radius:22px; box-shadow:0 12px 24px rgba(25,25,25,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Use connected app/workflow visuals
- Group by automation use case and platform product
- Keep orange limited to high-signal areas

## 6. Depth & Elevation
Zapier uses **friendly product-card elevation** on warm white surfaces.

## 7. Do's and Don'ts
### Do
- Keep workflow concepts visible and easy to scan
- Use orange as the anchor
- Preserve modular app and automation cards
### Don't
- Don’t overwhelm the page with warm accent blocks
- Don’t make workflow logic visually confusing

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack workflow diagrams and app cards
- Keep primary CTA and category hierarchy near the top

## 9. Agent Prompt Guide
```text
Design this like Zapier: orange-led automation SaaS with warm white surfaces, modular app and workflow cards, practical modern typography, and clear automation-platform structure.
```
