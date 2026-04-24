# SoFi Design System

> Consumer finance with a bright cyan-blue identity, rounded fintech surfaces, and benefit-led product framing. SoFi's public site uses strong teal/cyan branding, white cards, and mainstream financial product storytelling.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
SoFi feels like **consumer finance made more modern, optimistic, and product-bundled**.
### Mood & Feeling
- Trustworthy
- Modern
- Benefit-led
- Mainstream fintech
- Friendly
### Design Density
**Medium density.** Multiple financial products are grouped clearly with promo and trust modules.
### Visual Character
- Bright cyan-teal brand accent
- White cards and rounded shells
- Clean fintech marketing modules
- Benefit and bundle framing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--sofi-teal` | `#00A3E0` | Primary brand accent |
| `--sofi-teal-deep` | `#0087BC` | Hover/support |
| `--sofi-white` | `#FFFFFF` | Main surface |
| `--sofi-surface` | `#F3FBFE` | Background |
| `--sofi-ink` | `#0F172A` | Text |
| `--sofi-muted` | `#64748B` | Secondary text |
| `--sofi-border` | `#D9EEF5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Apercu", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Apercu", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `30/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#00a3e0; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#0f172a; border:1px solid #d9eef5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #d9eef5; border-radius:20px; box-shadow:0 12px 24px rgba(15,23,42,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Group by product type: banking, loans, invest, credit
- Keep benefits and trust cues close to CTAs
- Use teal as a bright confidence signal

## 6. Depth & Elevation
SoFi uses **soft fintech card elevation** on bright, rounded surfaces.

## 7. Do's and Don'ts
### Do
- Keep it modern, optimistic, and trustworthy
- Use teal as the stable brand anchor
- Preserve product-bundle clarity
### Don't
- Don’t make it cold legacy banking UI
- Don’t overdecorate with too many fintech effects

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack benefit cards and product promos cleanly
- Keep primary sign-up paths highly visible

## 9. Agent Prompt Guide
```text
Design this like SoFi: bright teal-led consumer-finance UI with rounded white cards, benefit-focused product modules, modern fintech trust cues, and clear banking-loans-invest navigation.
```
