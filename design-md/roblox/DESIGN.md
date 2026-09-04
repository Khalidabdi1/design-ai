# Roblox Design System

> Playful, high-energy platform design for a user-generated game universe. Roblox's public product pairs a clean white/dark UI shell with bold rounded typography, saturated accent colors, and thumbnail-driven discovery grids that showcase millions of community-built experiences.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Roblox feels like **a game console dashboard built for a younger, creative audience**. The chrome is clean and modern, but every surface leans into bold color, rounded shapes, and thumbnail artwork to keep the platform feeling energetic and game-like.

### Mood & Feeling
- Playful, energetic, and imaginative
- Bright and youthful without feeling childish
- Confident use of a single brand red/black identity
- Discovery-driven and grid-heavy
- Friendly and approachable for creators and players alike

### Design Density
**Medium-to-high density.** Discovery pages show large grids of game thumbnails with compact metadata; profile and settings screens are calmer and more form-like.

### Visual Character
- White canvas in light mode, deep charcoal (`#1D1D1D`) in dark mode
- Signature red/black (`#FF3D42`-adjacent brand red) reserved for logo, CTAs, and Robux accents
- Rounded-rectangle thumbnails and pill-shaped buttons and chips
- Bold, chunky sans-serif typography for headings and CTAs
- 3D game thumbnails and avatar renders as primary visual content

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--rbx-red` | `#E2242A` | Primary brand accent, CTAs, logo |
| `--rbx-black` | `#1D1D1D` | Wordmark, dark-mode base surface |
| `--rbx-white` | `#FFFFFF` | Primary light-mode surface |
| `--rbx-ink` | `#1D1D1D` | Primary text (light mode) |
| `--rbx-ink-dark` | `#F2F2F2` | Primary text (dark mode) |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--rbx-green` | `#00A14B` | Success, online/available status |
| `--rbx-robux-gold` | `#F0C000` | Robux currency accent |
| `--rbx-muted` | `#6B6B6B` | Secondary text, metadata |
| `--rbx-border` | `#E5E5E5` | Card outlines, dividers |
| `--rbx-surface-alt` | `#F5F5F5` | Section backgrounds, hover states |
| `--rbx-surface-dark` | `#232527` | Card surface in dark mode |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Builder Sans", "Gotham", "Helvetica Neue", sans-serif;
--font-sans: "Builder Sans", "Helvetica Neue", Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Title | 40px | 800 | 1.1 | -0.01em | `#1D1D1D` |
| Page Title | 28px | 700 | 1.2 | 0 | `#1D1D1D` |
| Card Title | 16px | 700 | 1.3 | 0 | `#1D1D1D` |
| Body | 14px | 500 | 1.5 | 0 | `#1D1D1D` |
| Meta / Stats | 12px | 500 | 1.3 | 0 | `#6B6B6B` |
| Button Label | 14px | 700 | 1.2 | 0.01em | `#FFFFFF` |

### Typography Philosophy
Type should be **bold, rounded, and confident** — chunky weights on titles and buttons, with a friendly geometric sans that reads well at small sizes across dense thumbnail grids.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #e2242a;
  color: #ffffff;
  border: none;
  border-radius: 8px;
  min-height: 44px;
  padding: 0 24px;
  font-size: 14px;
  font-weight: 700;
}

.button-primary:hover {
  background: #c71f24;
}

.button-secondary {
  background: #f5f5f5;
  color: #1d1d1d;
  border: none;
  border-radius: 8px;
  min-height: 44px;
  padding: 0 24px;
  font-weight: 700;
}
```

### Game Card

```css
.game-card {
  background: #ffffff;
  border-radius: 12px;
  overflow: hidden;
}

.game-thumbnail {
  width: 100%;
  aspect-ratio: 1 / 1;
  border-radius: 12px;
  object-fit: cover;
}

.game-card-title {
  font-weight: 700;
  font-size: 14px;
  margin-top: 8px;
}
```

### Robux/Currency Chip

```css
.robux-chip {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  background: #f5f5f5;
  border-radius: 999px;
  padding: 4px 10px;
  font-weight: 700;
  color: #1d1d1d;
}
```

### Component Notes
- Game thumbnails are near-square with rounded corners and prominent artwork
- Robux currency always pairs a gold icon with bold numeric text
- Primary CTAs (Play, Get) use the brand red; secondary actions use neutral gray
- Avatar and 3D render previews get generous space; never crop tightly

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Icon-to-text gaps |
| `--space-2` | `8px` | Card internal spacing |
| `--space-3` | `12px` | Grid gutter (compact) |
| `--space-4` | `16px` | Grid gutter (standard) |
| `--space-5` | `24px` | Section spacing |
| `--space-6` | `40px` | Page-level margins |

### Layout Behavior
- Discovery pages use a responsive grid of near-square game cards (2 to 6+ columns by width)
- Horizontal carousels group games by category (Recommended, Popular, Continue Playing)
- Persistent top bar with search, Robux balance, and avatar/profile access
- Sidebar or bottom nav provides quick access to Home, Discover, Avatar, and Create

### Whitespace Philosophy
Whitespace should feel **energetic but organized** — enough gutter between thumbnails to keep grids scannable while preserving a dense, discovery-rich feed.

---

## 6. Depth & Elevation

### Elevation Strategy
Roblox uses **light, functional elevation** — mostly flat cards with subtle hover lift, and stronger shadows reserved for modals and the avatar/character viewer.

```css
--shadow-card: 0 1px 3px rgba(0, 0, 0, 0.08);
--shadow-card-hover: 0 4px 12px rgba(0, 0, 0, 0.15);
--shadow-modal: 0 8px 32px rgba(0, 0, 0, 0.25);
```

### Surface Hierarchy
- Flat white/charcoal base canvas
- Slightly elevated game cards with hover lift
- Elevated modals for purchases, avatar customization, and settings

---

## 7. Do's and Don'ts

### Do
- Keep game thumbnails and avatar art as the dominant visual content
- Use the brand red intentionally for primary actions and identity, not as a wash
- Maintain bold, rounded typography across headings and buttons
- Keep Robux and currency elements visually consistent everywhere they appear

### Don't
- Do not desaturate the brand identity into a generic enterprise palette
- Do not crop or distort game/avatar thumbnails from their native aspect ratio
- Do not overload cards with more than title, creator, and one or two stats
- Do not mix multiple accent colors for primary CTAs on the same screen

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single/double-column grid, bottom tab navigation |
| Tablet | `768px - 1023px` | Three to four-column grid, collapsible side nav |
| Desktop | `1024px+` | Five to six-column grid, persistent side navigation and top bar |

### Responsive Rules
- Game card grid columns scale fluidly with viewport width
- Carousels convert to swipeable horizontal scroll on touch devices
- Bottom tab bar on mobile becomes a persistent side rail on desktop
- Maintain minimum 44px touch targets for Play/Get buttons on all sizes

---

## 9. Agent Prompt Guide

### Quick Reference
- White/charcoal canvas with a confident brand red for CTAs and identity
- Near-square game thumbnails with rounded corners in dense discovery grids
- Bold, rounded, energetic typography on headings and buttons
- Light elevation with hover lift; stronger shadows reserved for modals

### Prompt Template
```text
Design this like Roblox's current public product and brand style:
- clean white or dark charcoal canvas with a confident brand-red accent for CTAs
- dense, responsive grid of near-square game/avatar thumbnails with rounded corners
- bold, chunky, rounded typography for headings and buttons
- gold-accented currency chips, light card elevation, and hover lift
- playful, energetic, discovery-first layout with horizontal category carousels
```
