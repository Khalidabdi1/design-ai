# Box Design System

> Enterprise content management with white space, blue trust cues, and AI-era document workflows. Box's public site uses bright white canvases, navy-blue accents, structured product cards, and a calm enterprise tone.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Box feels like **document infrastructure for large organizations**. It is clean, process-oriented, and quietly premium.
### Mood & Feeling
- Secure
- Enterprise-ready
- Clean
- Content-centric
- AI-augmented
### Design Density
**Medium density.** Many product options are grouped into clear cards and panels.
### Visual Character
- White-first layout
- Deep blue trust accents
- Content and workflow cards
- Minimal decorative noise

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--box-blue` | `#0061D5` | Primary action |
| `--box-navy` | `#0D2B45` | Deep anchor color |
| `--box-white` | `#FFFFFF` | Canvas and cards |
| `--box-surface` | `#F7FAFF` | Soft support background |
| `--box-ink` | `#182230` | Primary text |
| `--box-muted` | `#5F6B7A` | Secondary text |
| `--box-border` | `#DCE6F2` | Borders |
| `--box-success` | `#16825D` | Positive state |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero | 56px | 700 | 1.05 |
| H1 | 40px | 700 | 1.1 |
| H2 | 30px | 700 | 1.14 |
| Body | 16px | 400 | 1.6 |
| Small | 14px | 400 | 1.5 |
### Typography Philosophy
Favor highly readable enterprise typography with clear, process-friendly hierarchy.

## 4. Component Stylings
```css
.button-primary { background:#0061d5; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#182230; border:1px solid #dce6f2; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #dce6f2; border-radius:22px; box-shadow:0 12px 24px rgba(13,43,69,.06); }
.input { background:#fff; border:1px solid #dce6f2; border-radius:14px; min-height:46px; padding:12px 14px; }
```
### Component Notes
- Document and workflow cards should feel systematic
- Blue drives action, not page saturation

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Group by product, department, and workflow
- Keep enterprise browsing highly scannable
- Pair AI capabilities with document context

## 6. Depth & Elevation
Box uses **light enterprise elevation** with crisp borders and soft shadows.

## 7. Do's and Don'ts
### Do
- Keep it trustworthy and document-centric
- Use blue with discipline
- Preserve structure over decoration
### Don't
- Don’t make it playful consumer storage UI
- Don’t clutter product option grids

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack content cards before shrinking
- Keep search, CTA, and category hierarchy obvious

## 9. Agent Prompt Guide
```text
Design this like Box: white enterprise document-platform surfaces, deep blue trust accents, structured workflow cards, minimal chrome, and calm AI-enabled content management clarity.
```
