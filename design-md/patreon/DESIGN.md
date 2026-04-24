# Patreon Design System

> Creator membership platform with a warm coral identity, rounded UI, and creator-economy pragmatism. Patreon's public site uses bright coral (`#FF424D`), white surfaces, friendly sans-serif typography, and approachable community-focused messaging.

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Patreon feels like **creator monetization software that is friendly, direct, and community-oriented**.
### Mood & Feeling
- Supportive
- Creator-focused
- Warm
- Practical
- Community-driven
### Design Density
**Medium density.** Creator tools and membership flows stay understandable through large, clear blocks.
### Visual Character
- Coral/red brand anchor
- White cards and soft neutral support surfaces
- Rounded modules
- Creator and fan relationship framing

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--patreon-coral` | `#FF424D` | Primary brand accent |
| `--patreon-black` | `#111111` | Strong text and CTA anchor |
| `--patreon-white` | `#FFFFFF` | Main surface |
| `--patreon-surface` | `#FFF7F6` | Warm background |
| `--patreon-muted` | `#666666` | Secondary text |
| `--patreon-border` | `#E9DDDA` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "ABC Favorit", "Inter", "Helvetica Neue", Arial, sans-serif;
--font-sans: "ABC Favorit", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `58/700`, H1 `42/700`, H2 `30/700`, Body `16/400`, Small `14/400`
### Typography Philosophy
Use friendly modern type that feels direct and creator-centric rather than corporate.

## 4. Component Stylings
```css
.button-primary { background:#111; color:#fff; border:none; border-radius:999px; min-height:46px; padding:0 20px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e9ddda; border-radius:999px; min-height:46px; padding:0 20px; }
.card { background:#fff; border:1px solid #e9ddda; border-radius:24px; box-shadow:0 12px 24px rgba(17,17,17,.06); }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Center creator outcomes and community support
- Keep pricing and membership logic easy to follow
- Use warm accents sparingly

## 6. Depth & Elevation
Patreon uses **soft rounded card elevation** on a warm-neutral foundation.

## 7. Do's and Don'ts
### Do
- Keep it creator-supportive and human
- Use coral as a strong brand marker
- Preserve clear monetization flows
### Don't
- Don’t overcomplicate it with creator-tool clutter
- Don’t make it cold fintech or enterprise SaaS

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Keep support/join actions prominent
- Stack pricing and creator benefit cards cleanly

## 9. Agent Prompt Guide
```text
Design this like Patreon: creator-membership UI with warm coral branding, rounded white cards, friendly modern typography, simple monetization flows, and community-focused product clarity.
```
