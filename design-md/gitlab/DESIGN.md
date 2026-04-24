# GitLab Design System

> DevSecOps platform with dark contrast, purple-orange brand energy, and lifecycle-spanning product messaging. GitLab's public site uses a modern sans stack, white and dark sections, and the recognizable GitLab orange and aubergine palette.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
GitLab feels like **the full software lifecycle packaged into a modern technical platform**.
### Mood & Feeling
- Technical
- Opinionated
- Platform-wide
- DevOps-heavy
- Modern
### Design Density
**Medium to high density.** Product breadth is large, but sections remain clearly grouped.
### Visual Character
- White layout with dark contrast bands
- Orange and aubergine brand accents
- Lifecycle and AI product framing
- Technical diagrams and screenshots

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--gitlab-orange` | `#FC6D26` | Primary brand accent |
| `--gitlab-aubergine` | `#554488` | Deep brand support |
| `--gitlab-black` | `#171321` | Dark contrast |
| `--gitlab-white` | `#FFFFFF` | Main surface |
| `--gitlab-surface` | `#F8F5FF` | Soft tinted background |
| `--gitlab-ink` | `#1F1F2D` | Text |
| `--gitlab-muted` | `#667085` | Secondary text |
| `--gitlab-border` | `#E4DFF1` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "GitLab Sans", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "GitLab Sans", "Inter", system-ui, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use technical, platform-capable typography with strong hierarchy and code-awareness.

## 4. Component Stylings
```css
.button-primary { background:#fc6d26; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#1f1f2d; border:1px solid #e4dff1; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e4dff1; border-radius:22px; box-shadow:0 12px 24px rgba(23,19,33,.07); }
.code-card { background:#171321; color:#fff; border-radius:20px; font-family:var(--font-mono); }
```
### Component Notes
- Orange should punctuate the page, not flood it
- Dark product proof helps technical credibility

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Organize by lifecycle stages and platform outcomes
- Pair strong claims with screenshots and diagrams
- Alternate white and dark sections for rhythm

## 6. Depth & Elevation
GitLab uses **contrast-driven depth** with moderate product-card elevation.

## 7. Do's and Don'ts
### Do
- Keep it platform-wide and technical
- Use orange and aubergine consistently
- Preserve lifecycle clarity
### Don't
- Don’t make it generic cloud SaaS blue
- Don’t soften away the technical edge

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack lifecycle sections vertically
- Keep CTAs and product proof readable

## 9. Agent Prompt Guide
```text
Design this like GitLab: orange-and-aubergine DevSecOps branding, white and dark contrast sections, technical product proof, lifecycle-wide organization, and modern developer-platform polish.
```
