# Datadog Design System

> Observability software with dark dashboards, vivid purple brand cues, and dense technical clarity. Datadog's public site combines white and dark chart surfaces with strong violet-purple accents and crisp, technical product storytelling.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Datadog feels like **observability tooling made visually polished and technically credible**.
### Mood & Feeling
- Analytical
- Technical
- Fast
- Modern
- Engineer-friendly
### Design Density
**High density.** Product breadth and dashboards are information-rich but organized.
### Visual Character
- Purple/violet accents
- Dark product screenshots
- White marketing surfaces
- Metrics and chart-first framing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--dd-purple` | `#632CA6` | Brand accent |
| `--dd-purple-bright` | `#7F56D9` | Highlight accent |
| `--dd-black` | `#101828` | Dark dashboards |
| `--dd-white` | `#FFFFFF` | Main surface |
| `--dd-surface` | `#F7F7FB` | Light background |
| `--dd-ink` | `#1D2939` | Text |
| `--dd-muted` | `#667085` | Secondary text |
| `--dd-border` | `#E4E7EC` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "National 2", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "Roboto Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Favor sharp technical readability with enough contrast to support dense product detail.

## 4. Component Stylings
```css
.button-primary { background:#632ca6; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#1d2939; border:1px solid #e4e7ec; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e4e7ec; border-radius:22px; box-shadow:0 12px 24px rgba(16,24,40,.06); }
.dashboard { background:#101828; color:#fff; border-radius:22px; }
```
### Component Notes
- Pair light marketing copy with dark dashboard captures
- Purple drives brand identity and selected actions

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Organize by platform capability and developer workflow
- Let dashboards do the credibility work
- Keep product categories dense but clearly separated

## 6. Depth & Elevation
Datadog uses **dashboard contrast more than heavy shadow**.

## 7. Do's and Don'ts
### Do
- Keep it technical and observability-centric
- Use purple consistently but selectively
- Preserve dark dashboard realism
### Don't
- Don’t make it generic pastel SaaS
- Don’t flatten monitoring visuals into plain cards

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack dashboards vertically
- Preserve chart readability and code/metric contrast

## 9. Agent Prompt Guide
```text
Design this like Datadog: purple-branded observability SaaS, dark dashboards on white marketing surfaces, technical typography, dense but structured platform storytelling, and engineer-friendly product clarity.
```
