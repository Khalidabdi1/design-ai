# Instagram Design System

> Visual-first storytelling with a clean, content-forward chrome. Instagram's public product wraps a minimal white (or true-black dark mode) interface around a vivid gradient brand mark, letting photos and video carry the visual weight while UI chrome stays quiet, fast, and instantly familiar.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Instagram feels like **a gallery wall with a phone-sized frame**. Chrome recedes almost entirely — thin dividers, small icons, and generous negative space — so uploaded photos and video remain the dominant visual element on every screen.

### Mood & Feeling
- Content-first and editorial
- Clean, fast, and effortless
- Youthful but visually neutral
- Warm brand accent used sparingly, never as a wash
- Immediate and tactile (taps, holds, swipes)

### Design Density
**Low-to-medium density.** Feeds are a single vertical column of large media with minimal metadata; grids (profile, explore) pack tightly but rely on square media rather than typographic detail.

### Visual Character
- Pure white canvas in light mode, near-black (`#000000`) in dark mode
- Signature gradient (purple → pink → orange) reserved for logo, stories ring, and highlights
- Circular avatars and story rings as the primary identity motif
- Full-bleed media with minimal cropping chrome
- Iconography over text labels throughout navigation

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--ig-white` | `#FFFFFF` | Primary light-mode surface |
| `--ig-black` | `#000000` | Primary dark-mode surface |
| `--ig-ink` | `#262626` | Primary text (light mode) |
| `--ig-ink-dark` | `#F5F5F5` | Primary text (dark mode) |
| `--ig-border` | `#DBDBDB` | Dividers, card outlines |

### Brand Gradient

| Token | Value | Role |
|-------|-------|------|
| `--ig-gradient` | `linear-gradient(45deg, #405DE6, #5851DB, #833AB4, #C13584, #E1306C, #FD1D1D, #F56040, #F77737, #FCAF45, #FFDC80)` | Logo, story ring, active highlight |
| `--ig-purple` | `#833AB4` | Gradient anchor, accent states |
| `--ig-pink` | `#E1306C` | Gradient anchor, like/heart accent |
| `--ig-orange` | `#F77737` | Gradient anchor, warm highlight |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--ig-blue` | `#0095F6` | Links, primary CTA, "Follow" button |
| `--ig-red` | `#ED4956` | Like/heart fill, error/destructive state |
| `--ig-muted` | `#8E8E8E` | Secondary text, timestamps |
| `--ig-surface-alt` | `#FAFAFA` | Subtle section backgrounds |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: -apple-system, "Helvetica Neue", Helvetica, Arial, sans-serif;
--font-display: "Billabong", cursive; /* wordmark only */
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Wordmark | 32px | 400 (script) | 1 | 0 | `#262626` |
| Page Title | 20px | 600 | 1.3 | 0 | `#262626` |
| Username / Handle | 14px | 600 | 1.4 | 0 | `#262626` |
| Body | 14px | 400 | 1.5 | 0 | `#262626` |
| Caption | 14px | 400 | 1.4 | 0 | `#262626` |
| Meta / Timestamp | 12px | 400 | 1.4 | 0 | `#8E8E8E` |
| Button Label | 14px | 600 | 1.2 | 0 | `#FFFFFF` |

### Typography Philosophy
Type should be **quiet and utilitarian** — a single system sans throughout, low visual competition with media, and bold weight reserved for usernames and calls to action.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0095f6;
  color: #ffffff;
  border: none;
  border-radius: 8px;
  min-height: 32px;
  padding: 0 16px;
  font-size: 14px;
  font-weight: 600;
}

.button-primary:hover {
  background: #1877f2;
}

.button-secondary {
  background: #efefef;
  color: #262626;
  border: none;
  border-radius: 8px;
  min-height: 32px;
  padding: 0 16px;
  font-weight: 600;
}
```

### Story Ring

```css
.story-ring {
  width: 66px;
  height: 66px;
  border-radius: 50%;
  padding: 3px;
  background: linear-gradient(45deg, #833ab4, #e1306c, #f77737);
}

.story-ring img {
  border: 3px solid #ffffff;
  border-radius: 50%;
}
```

### Post Card

```css
.post-card {
  background: #ffffff;
  border: 1px solid #dbdbdb;
  border-radius: 8px;
}

.post-media {
  width: 100%;
  aspect-ratio: 1 / 1;
  object-fit: cover;
}
```

### Component Notes
- Like, comment, share, and save icons stay outline-style at rest, filled on active state
- Avatars are always circular; never use square or rounded-square crops
- Buttons and inputs use small radii (6–8px), not pill shapes

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Icon padding |
| `--space-2` | `8px` | Inline element gaps |
| `--space-3` | `12px` | Card interior padding |
| `--space-4` | `16px` | Section spacing |
| `--space-5` | `24px` | Feed item separation |
| `--space-6` | `32px` | Grid and profile section gaps |

### Layout Behavior
- Single-column feed with full-width media capped at a fixed max width
- Profile and explore views use tight 3-column square grids
- Navigation is icon-only, fixed to the bottom on mobile and left rail on desktop
- Minimal chrome around media; let content define the rhythm

### Whitespace Philosophy
Whitespace exists to **separate content units, not to decorate them** — thin borders and small gaps do the work instead of large empty margins.

---

## 6. Depth & Elevation

### Elevation Strategy
Instagram is largely **flat**. Depth is implied through thin borders and subtle shadows on modals and dropdowns rather than persistent card elevation.

```css
--shadow-modal: 0 4px 24px rgba(0, 0, 0, 0.15);
--shadow-dropdown: 0 2px 8px rgba(0, 0, 0, 0.12);
--border-hairline: 1px solid #dbdbdb;
```

### Surface Hierarchy
- White/black base canvas
- Hairline-bordered cards and grid cells
- Elevated modals for stories, comments, and post composer overlays

---

## 7. Do's and Don'ts

### Do
- Let photos and video be the visual focus on every screen
- Reserve the brand gradient for logo, rings, and small highlight moments
- Keep navigation icon-driven and instantly recognizable
- Preserve true black in dark mode, not dark gray

### Don't
- Do not wash large surfaces in the brand gradient
- Do not add heavy shadows or skeuomorphic depth to media cards
- Do not replace circular avatars with other shapes
- Do not clutter the feed with dense metadata or multiple competing CTAs

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single-column feed, bottom tab bar, full-width media |
| Tablet | `768px - 1023px` | Centered feed column, side padding increases |
| Desktop | `1024px+` | Left icon rail navigation, centered max-width feed, right-side suggestions panel |

### Responsive Rules
- Media aspect ratios stay consistent across breakpoints; never crop unexpectedly
- Bottom tab bar on mobile becomes a left icon rail on desktop
- Story rings and avatars scale down but remain circular at every size
- Keep tap targets at least 44px on touch devices

---

## 9. Agent Prompt Guide

### Quick Reference
- White (or true-black dark mode) canvas with minimal chrome
- Brand gradient reserved for logo, story rings, and small accents
- Circular avatars, square media grids, icon-only navigation
- Flat surfaces with hairline borders instead of heavy shadows

### Prompt Template
```text
Design this like Instagram's current public product and brand style:
- clean white or true-black canvas with content-first layout
- circular avatars and story rings using the signature purple-to-orange gradient
- full-bleed square/vertical media with minimal surrounding chrome
- icon-only navigation, flat surfaces, and hairline borders instead of shadows
- quiet system typography that never competes with photos and video
```
