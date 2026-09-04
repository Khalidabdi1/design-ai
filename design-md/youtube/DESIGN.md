# YouTube Design System

> A dense, video-first grid built for endless discovery. YouTube's public product pairs a neutral white/dark surface with confident red brand accents, thumbnail-driven grids, and a persistent player chrome designed to keep video always in focus.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
YouTube feels like **an infinite video library organized as a scannable grid**. Thumbnails are the primary visual unit; surrounding chrome (metadata, nav, controls) stays compact and neutral so the grid itself does the work of discovery.

### Mood & Feeling
- Dense but scannable
- Neutral and utilitarian outside of the player
- Confident red as a decisive, sparingly used accent
- Functional and information-rich
- Fast-loading, infinite-scroll energy

### Design Density
**High density.** Home and search grids show dozens of thumbnails with tight metadata; the watch page is comparatively focused, prioritizing the player above a dense comments/related rail.

### Visual Character
- White canvas in light mode, near-black (`#0F0F0F`) in dark mode
- Signature red (`#FF0000`) reserved for logo, subscribe/live badges, and small alerts
- 16:9 thumbnail grid as the core layout unit
- Rounded-rectangle thumbnails and pill-shaped chips for filters
- Minimal line iconography for navigation and controls

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--yt-red` | `#FF0000` | Brand mark, subscribe button, live badge |
| `--yt-white` | `#FFFFFF` | Primary light-mode surface |
| `--yt-black` | `#0F0F0F` | Primary dark-mode surface |
| `--yt-ink` | `#0F0F0F` | Primary text (light mode) |
| `--yt-ink-dark` | `#F1F1F1` | Primary text (dark mode) |

### Support Palette

| Token | Hex | Role |
|-------|-----|------|
| `--yt-muted` | `#606060` | Secondary text, view counts, timestamps |
| `--yt-muted-dark` | `#AAAAAA` | Secondary text in dark mode |
| `--yt-border` | `#E5E5E5` | Dividers, chip outlines |
| `--yt-surface-alt` | `#F9F9F9` | Chip backgrounds, hover states |
| `--yt-surface-alt-dark` | `#272727` | Chip and hover backgrounds in dark mode |
| `--yt-live` | `#FF0000` | Live indicator badge |
| `--yt-progress` | `#FF0000` | Video scrub-bar progress fill |

---

## 3. Typography Rules

### Font Stack

```css
--font-sans: "Roboto", "Arial", sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Video Title (watch page) | 18px | 500 | 1.4 | 0 | `#0F0F0F` |
| Video Title (grid card) | 14px | 500 | 1.4 | 0 | `#0F0F0F` |
| Channel Name | 12px | 400 | 1.3 | 0 | `#606060` |
| Metadata (views/date) | 12px | 400 | 1.3 | 0 | `#606060` |
| Chip Label | 14px | 500 | 1.2 | 0 | `#0F0F0F` |
| Button Label | 14px | 500 | 1.2 | 0.3px | `#FFFFFF` |

### Typography Philosophy
Type should be **compact and information-dense**, favoring two-line title truncation and small metadata text so thumbnails remain the dominant visual signal.

---

## 4. Component Stylings

### Buttons

```css
.button-subscribe {
  background: #0f0f0f;
  color: #ffffff;
  border: none;
  border-radius: 18px;
  min-height: 36px;
  padding: 0 16px;
  font-size: 14px;
  font-weight: 500;
}

.button-subscribe.subscribed {
  background: #f2f2f2;
  color: #0f0f0f;
}

.chip {
  background: #f2f2f2;
  color: #0f0f0f;
  border-radius: 8px;
  padding: 6px 12px;
  font-size: 14px;
  font-weight: 500;
}

.chip.active {
  background: #0f0f0f;
  color: #ffffff;
}
```

### Video Card

```css
.video-thumbnail {
  width: 100%;
  aspect-ratio: 16 / 9;
  border-radius: 12px;
  object-fit: cover;
}

.video-card-meta {
  display: flex;
  gap: 12px;
  margin-top: 12px;
}
```

### Component Notes
- Thumbnails always maintain 16:9 aspect ratio with rounded corners
- Live and Premiere states use a small red pill badge overlaid on the thumbnail
- Subscribe button switches to a neutral "Subscribed" state after activation
- Filter chips use a horizontally scrolling row beneath the search/nav bar

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | `4px` | Icon padding |
| `--space-2` | `8px` | Chip and metadata gaps |
| `--space-3` | `12px` | Card internal spacing |
| `--space-4` | `16px` | Grid gutter |
| `--space-5` | `24px` | Section spacing |
| `--space-6` | `40px` | Page-level margins on desktop |

### Layout Behavior
- Home/search use a responsive multi-column thumbnail grid (1 to 5+ columns by width)
- Watch page splits into a primary player column and a secondary related/comments rail
- Persistent top bar (search, logo, account) and a collapsible left navigation rail
- Chips row provides quick category filtering directly beneath the top bar

### Whitespace Philosophy
Whitespace is **grid-driven, not generous** — enough gutter to separate thumbnails cleanly, with density prioritized over open marketing-style space.

---

## 6. Depth & Elevation

### Elevation Strategy
YouTube is mostly **flat**, with elevation reserved for menus, the mini-player, and modal overlays.

```css
--shadow-menu: 0 2px 6px rgba(0, 0, 0, 0.2);
--shadow-miniplayer: 0 4px 16px rgba(0, 0, 0, 0.3);
--shadow-card-hover: 0 1px 2px rgba(0, 0, 0, 0.1);
```

### Surface Hierarchy
- Flat white/black base grid
- Slightly raised chips and buttons
- Elevated dropdown menus, mini-player, and full-screen overlays

---

## 7. Do's and Don'ts

### Do
- Keep thumbnails as the dominant visual element in every grid
- Reserve red for brand mark, subscribe accents, and live/alert badges
- Maintain consistent 16:9 thumbnail framing across all card sizes
- Use compact, truncated metadata rather than verbose descriptions in grids

### Don't
- Do not saturate large surfaces in red
- Do not vary thumbnail aspect ratios within the same grid
- Do not let the player chrome compete visually with the video content
- Do not overload grid cards with more than title, channel, and two metadata lines

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Single-column vertical feed, full-width player, bottom tab bar |
| Tablet | `768px - 1279px` | Two to three-column grid, collapsible nav rail |
| Desktop | `1280px+` | Four to five-column grid, persistent nav rail, side-by-side watch layout |

### Responsive Rules
- Grid column count scales fluidly with viewport width, not fixed breakpoints alone
- Watch page collapses the related/comments rail below the player on mobile
- Navigation rail collapses to icon-only, then to a bottom tab bar on small screens
- Touch targets for controls and chips stay at least 40px on mobile

---

## 9. Agent Prompt Guide

### Quick Reference
- White/near-black canvas with red reserved for brand and small accents
- Dense thumbnail grid at consistent 16:9 ratio as the core layout unit
- Compact metadata typography, pill-shaped filter chips
- Flat surfaces with elevation only on menus and overlays

### Prompt Template
```text
Design this like YouTube's current public product and brand style:
- neutral white or near-black canvas with red used only for brand and small accents
- dense, responsive thumbnail grid at consistent 16:9 aspect ratio
- compact two-line titles with small muted metadata beneath each thumbnail
- pill-shaped filter chips, flat surfaces, and elevation reserved for menus/overlays
- persistent top search bar with a collapsible left navigation rail
```
