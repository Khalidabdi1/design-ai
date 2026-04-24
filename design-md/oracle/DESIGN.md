# Oracle Design System

> Enterprise cloud and applications with stark red-black branding and high-density product breadth. Oracle's public site uses white, black, and Oracle red to frame an extensive enterprise product catalog.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Oracle feels like **large-scale enterprise technology with sharp, no-nonsense branding**.
### Mood & Feeling
- Corporate
- Technical
- Enterprise-heavy
- Direct
- Global
### Design Density
**High density.** Product breadth is large, but navigation and modules keep it structured.
### Visual Character
- Red-black-white brand frame
- Dense enterprise product menus
- Strong text hierarchy
- Minimal playful elements

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--oracle-red` | `#C74634` | Primary brand accent |
| `--oracle-black` | `#161513` | Strong contrast |
| `--oracle-white` | `#FFFFFF` | Main surface |
| `--oracle-surface` | `#F5F5F5` | Soft support background |
| `--oracle-ink` | `#1F1F1F` | Primary text |
| `--oracle-muted` | `#666666` | Secondary text |
| `--oracle-border` | `#E3E3E3` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Oracle Sans", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Oracle Sans", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use strong, enterprise-readable type with direct hierarchy and minimal flourish.

## 4. Component Stylings
```css
.button-primary { background:#c74634; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#1f1f1f; border:1px solid #e3e3e3; border-radius:999px; min-height:44px; padding:0 20px; }
.card { background:#fff; border:1px solid #e3e3e3; border-radius:18px; box-shadow:0 10px 22px rgba(0,0,0,.05); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Group by enterprise solution family
- Support very broad navigation without losing hierarchy
- Use red mainly for emphasis and CTA

## 6. Depth & Elevation
Oracle uses **light card elevation** with stronger reliance on text structure and contrast than shadow.

## 7. Do's and Don'ts
### Do
- Keep it direct and enterprise-capable
- Use red-black-white consistently
- Preserve large product-family hierarchy
### Don't
- Don’t soften it into playful startup UI
- Don’t scatter too many accent colors across the page

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Collapse dense menus into clean stacks
- Keep enterprise CTA paths visible

## 9. Agent Prompt Guide
```text
Design this like Oracle: red-black-white enterprise technology branding, strong direct typography, structured product-family navigation, light card framing, and large-scale cloud-platform seriousness.
```
