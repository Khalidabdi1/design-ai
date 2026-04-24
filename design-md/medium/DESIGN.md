# Medium Design System

> Reading and writing platform with magazine-like simplicity and strong black-and-green branding. Medium's public site uses restrained editorial layout, serif-forward reading tone, and the signature Medium green (`#1A8917`).

---

## 1. Visual Theme & Atmosphere
### Overall Aesthetic
Medium feels like **digital magazine publishing with an intentionally quiet interface**.
### Mood & Feeling
- Editorial
- Calm
- Literary
- Minimal
- Reading-first
### Design Density
**Low density.** The interface stays out of the way of text and imagery.
### Visual Character
- Black and white frame
- Medium green brand accent
- Serif display and reading tone
- Minimal interface chrome

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--medium-green` | `#1A8917` | Primary brand accent |
| `--medium-black` | `#111111` | Text and anchor color |
| `--medium-white` | `#FFFFFF` | Canvas |
| `--medium-surface` | `#F7F7F7` | Soft support background |
| `--medium-muted` | `#6B6B6B` | Secondary text |
| `--medium-border` | `#E5E5E5` | Borders |

## 3. Typography Rules
### Font Stack
```css
--font-display: "Charter", Georgia, serif;
--font-sans: "Sohne", "Inter", system-ui, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```
### Type Scale
Hero `56/700`, H1 `40/700`, H2 `28/700`, Body `18/400`, Small `14/400`
### Typography Philosophy
Optimize for reading comfort and editorial credibility, not app-like sharpness.

## 4. Component Stylings
```css
.button-primary { background:#1a8917; color:#fff; border:none; border-radius:999px; min-height:42px; padding:0 18px; font-weight:600; }
.button-secondary { background:#fff; color:#111; border:1px solid #e5e5e5; border-radius:999px; min-height:42px; padding:0 18px; }
.card { background:#fff; border:1px solid #e5e5e5; border-radius:16px; }
```

## 5. Layout Principles
### Spacing Scale
`4, 8, 12, 16, 24, 32, 48, 64px`
### Layout Behavior
- Let story previews and reading paths lead
- Keep navigation secondary to content
- Preserve generous margins and calm pacing

## 6. Depth & Elevation
Medium uses **minimal elevation**, relying more on whitespace and text hierarchy than shadows.

## 7. Do's and Don'ts
### Do
- Keep it reading-first and quiet
- Use green as a restrained brand signal
- Preserve editorial typography
### Don't
- Don’t add unnecessary dashboard chrome
- Don’t make it feel like a noisy content marketplace

## 8. Responsive Behavior
### Breakpoints
- Mobile `<768px`
- Tablet `768px-1023px`
- Desktop `1024px+`
### Responsive Rules
- Preserve line length and reading comfort
- Keep actions secondary to content

## 9. Agent Prompt Guide
```text
Design this like Medium: calm editorial publishing UI with black-and-white structure, restrained green accents, serif-led reading typography, and minimal interface chrome.
```
