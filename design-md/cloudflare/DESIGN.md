# Cloudflare Design System

> Internet infrastructure with bold contrast and unmistakable orange brand energy. Cloudflare's public site mixes white and dark surfaces, sharp typography, orange (`#F38020`) accents, and dense infrastructure storytelling for networking, security, and developer products.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Cloudflare feels like **internet-scale infrastructure marketed with confidence and technical sharpness**.
### Mood & Feeling
- Technical
- Fast
- Infrastructure-heavy
- Confident
- Global-scale
### Design Density
**Medium to high density.** Many products, but strong hierarchy keeps it navigable.
### Visual Character
- Orange brand highlights
- White and dark contrast sections
- Dense but structured product narratives
- Technical diagrams and metric framing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--cf-orange` | `#F38020` | Primary brand accent |
| `--cf-orange-deep` | `#E06A0A` | Hover / stronger accent |
| `--cf-black` | `#111111` | Strong contrast |
| `--cf-white` | `#FFFFFF` | Main surface |
| `--cf-surface` | `#F7F7F8` | Soft background |
| `--cf-ink` | `#1D1D1F` | Primary text |
| `--cf-muted` | `#5F6368` | Secondary text |
| `--cf-border` | `#E3E3E3` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Inter", system-ui, sans-serif;
--font-mono: "IBM Plex Mono", "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `60/700`, H1 `44/700`, H2 `32/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use crisp, technical, high-clarity type with strong contrast and little softness.

## 4. Component Stylings
```css
.button-primary { background:#f38020; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:700; }
.button-secondary { background:#fff; color:#1d1d1f; border:1px solid #e3e3e3; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e3e3e3; border-radius:20px; box-shadow:0 12px 24px rgba(0,0,0,.06); }
.code-card { background:#111; color:#fff; border-radius:20px; font-family:var(--font-mono); }
```
### Component Notes
- Product cards should feel technical, not playful
- Orange is strong and sparing

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Lead with product families and global scale
- Support deep browsing via cards and grouped navigation
- Use dark contrast sections for authority

## 6. Depth & Elevation
Cloudflare uses **clean contrast-based depth** with restrained card elevation.

## 7. Do's and Don'ts
### Do
- Keep it technical and fast
- Use orange as a bold structural signal
- Preserve dense but readable information architecture
### Don't
- Don’t over-soften it into generic SaaS
- Don’t flood the page with orange

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Stack complex product grids
- Keep headings strong and diagrams legible

## 9. Agent Prompt Guide
```text
Design this like Cloudflare: technical infrastructure marketing with white and dark contrast sections, strong orange accents, sharp sans-serif typography, grouped product cards, and internet-scale authority.
```
