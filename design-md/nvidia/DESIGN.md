# NVIDIA Design System

> High-performance computing and AI with black surfaces, luminous green branding, and premium technical polish. NVIDIA's public site uses dark contrast, bright green (`#76B900`), and dramatic product/AI storytelling.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
NVIDIA feels like **advanced computing power presented with cinematic technical confidence**.
### Mood & Feeling
- Powerful
- Technical
- Premium
- AI-forward
- Performance-driven
### Design Density
**Medium density.** Visual drama is high, but structure stays controlled.
### Visual Character
- Black and charcoal surfaces
- NVIDIA green accent
- Strong hardware/AI imagery
- Premium dark technical branding

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--nvidia-green` | `#76B900` | Primary brand accent |
| `--nvidia-black` | `#0B0B0B` | Main contrast |
| `--nvidia-charcoal` | `#171717` | Dark surface |
| `--nvidia-white` | `#FFFFFF` | Text on dark / cards |
| `--nvidia-muted` | `#B0B3B8` | Secondary text |
| `--nvidia-border` | `#2B2B2B` | Dark borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "NVIDIA Sans", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "NVIDIA Sans", "Inter", system-ui, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `60/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use premium technical typography with strong contrast and performance-oriented hierarchy.

## 4. Component Stylings
```css
.button-primary { background:#76b900; color:#0b0b0b; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:transparent; color:#fff; border:1px solid #2b2b2b; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#171717; color:#fff; border:1px solid #2b2b2b; border-radius:22px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Use dark immersive sections
- Let AI and hardware visuals provide drama
- Keep product families clearly grouped

## 6. Depth & Elevation
NVIDIA uses **dark-surface contrast depth** more than visible shadow.

## 7. Do's and Don'ts
### Do
- Keep it premium, technical, and high-performance
- Use green as a sharp focal accent
- Preserve dark cinematic framing
### Don't
- Don’t soften it into generic SaaS
- Don’t use too many unrelated accent colors

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Preserve large visual impact and CTA clarity
- Stack hardware/AI stories vertically on small screens

## 9. Agent Prompt Guide
```text
Design this like NVIDIA: premium black-and-charcoal technical branding with bright green accents, cinematic AI/hardware storytelling, and strong high-performance product hierarchy.
```
