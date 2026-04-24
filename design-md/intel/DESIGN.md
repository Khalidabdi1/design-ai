# Intel Design System

> Computing and silicon innovation with blue brand authority and clean technology framing. Intel's public site uses white and blue surfaces, a modern sans stack, and broad product storytelling around AI and chips.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Intel feels like **core computing infrastructure expressed through clean, corporate-tech clarity**.
### Mood & Feeling
- Technical
- Trustworthy
- Broad
- Corporate-tech
- Performance-aware
### Design Density
**Medium density.** Many computing stories are present, but the layout remains structured.
### Visual Character
- Intel blue anchors
- White and pale-blue support surfaces
- Product and research storytelling
- Clean technical utility

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--intel-blue` | `#0071C5` | Primary brand accent |
| `--intel-blue-deep` | `#004A86` | Strong support blue |
| `--intel-white` | `#FFFFFF` | Main surface |
| `--intel-surface` | `#F5F9FF` | Support background |
| `--intel-ink` | `#14213D` | Text |
| `--intel-muted` | `#64748B` | Secondary text |
| `--intel-border` | `#DCE7F5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Intel Clear", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Intel Clear", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `30/700`, Body `16/400`, Small `14/400`

## 4. Component Stylings
```css
.button-primary { background:#0071c5; color:#fff; border:none; border-radius:999px; min-height:44px; padding:0 18px; font-weight:700; }
.button-secondary { background:#fff; color:#14213d; border:1px solid #dce7f5; border-radius:999px; min-height:44px; padding:0 18px; }
.card { background:#fff; border:1px solid #dce7f5; border-radius:20px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48px`
### Layout Behavior
- Group by AI, PCs, data center, and partner technology
- Use blue to organize, not overwhelm
- Pair technical stories with strong product proof

## 6. Depth & Elevation
Intel uses **light technical-card framing** with pale-blue support surfaces.

## 7. Do's and Don'ts
### Do
- Keep it credible and technology-forward
- Use Intel blue consistently
- Preserve broad computing hierarchy
### Don't
- Don’t make it overly playful
- Don’t bury technical proof beneath generic marketing

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack product families cleanly
- Keep hero and category CTAs visible

## 9. Agent Prompt Guide
```text
Design this like Intel: blue-led computing brand UI with white and pale-blue surfaces, clean technical typography, structured AI and hardware storytelling, and corporate-tech clarity.
```
