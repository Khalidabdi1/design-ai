# Epic Games Store Design System

> Digital gaming marketplace with sleek, cinematic dark aesthetic. Deep black backgrounds (#121212, #202020), vibrant blue accent (#0074e4), bold yellow free game promotions, and immersive game imagery for a next-gen PC gaming experience.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Epic Games Store embraces a **premium, cinematic gaming** design philosophy. The interface is bold, modern, and content-forward—showcasing games as visual experiences rather than mere products. The dark canvas creates a theatrical backdrop where game artwork becomes the hero, while clean geometric elements provide structure and navigation.

### Mood & Feeling
- **Cinematic & Immersive**: Full-bleed imagery and dark backgrounds create theater-like experience
- **Premium & Modern**: Clean lines, generous spacing, sophisticated color palette
- **Discovery-Focused**: Curated collections and featured highlights guide exploration
- **Generous & Value-Driven**: Free games prominently celebrated with bold yellow accents
- **Social & Connected**: Friends activity, achievements, and community integration

### Design Density
**Medium density** with generous whitespace. Epic favors breathing room around content, letting large game artwork speak for itself. Cards have ample padding, sections are clearly delineated, and the overall feeling is more curated gallery than dense catalog.

### Visual Character
- Pure black and dark gray backgrounds as primary surfaces
- Blue accent (#0074e4) for primary interactions and CTAs
- Vibrant yellow for free game promotions and special offers
- Full-width hero images with gradient overlays
- Rounded corners creating friendly, modern feel
- Card-based layouts with hover elevations
- Horizontal carousels with smooth scrolling
- Minimalist iconography with consistent stroke weights

---

## 2. Color Palette & Roles

### Primary Dark Theme

| Token | Hex | Role |
|-------|-----|------|
| `--background-pure-black` | `#000000` | Deepest surfaces, modal overlays |
| `--background-primary` | `#121212` | Main app background |
| `--background-secondary` | `#202020` | Cards, elevated surfaces |
| `--background-tertiary` | `#2a2a2a` | Hover states, selected items |
| `--background-elevated` | `#303030` | Dropdowns, popovers |
| `--background-input` | `#3a3a3a` | Form inputs, search fields |
| `--background-sidebar` | `#18181c` | Left sidebar navigation |
| `--background-header` | `#121212` | Top navigation bar |

### Accent Colors

| Token | Hex | Role |
|-------|-----|------|
| `--accent-primary` | `#0074e4` | Primary buttons, links, selections |
| `--accent-primary-hover` | `#0084ff` | Primary button hover state |
| `--accent-primary-active` | `#0066cc` | Primary button pressed state |
| `--accent-secondary` | `#26bbff` | Light blue highlights, secondary accents |
| `--free-game-yellow` | `#f5a623` | Free game badges, promotions |
| `--free-game-yellow-bright` | `#ffcc00` | Free game banner highlights |
| `--sale-green` | `#00e676` | Sale badges, discount indicators |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--text-primary` | `#ffffff` | Primary body text, headers |
| `--text-secondary` | `#a8a8a8` | Secondary text, metadata |
| `--text-tertiary` | `#6b6b6b` | Tertiary text, placeholders |
| `--text-muted` | `#505050` | Disabled text, timestamps |
| `--text-link` | `#0074e4` | Hyperlinks |
| `--text-link-hover` | `#26bbff` | Link hover state |
| `--text-price` | `#ffffff` | Price displays |
| `--text-discount` | `#00e676` | Discounted price |
| `--text-original-price` | `#6b6b6b` | Strikethrough original price |

### Status & Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--status-online` | `#00e676` | Online friends indicator |
| `--status-away` | `#f5a623` | Away status |
| `--status-offline` | `#505050` | Offline status |
| `--status-in-game` | `#0074e4` | Currently playing game |
| `--success` | `#00e676` | Success confirmations |
| `--warning` | `#f5a623` | Warning states |
| `--error` | `#f44336` | Error states, critical alerts |
| `--info` | `#26bbff` | Informational messages |

### Badge & Tag Colors

| Token | Hex | Role |
|-------|-----|------|
| `--badge-free` | `#f5a623` | Free game badge |
| `--badge-sale` | `#00e676` | Sale/discount badge |
| `--badge-new` | `#0074e4` | New release badge |
| `--badge-coming-soon` | `#9c27b0` | Coming soon badge |
| `--badge-early-access` | `#ff6f00` | Early access indicator |
| `--badge-owned` | `#303030` | Owned game indicator |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary app font - Brutal Type */
--font-primary: "Brutal Type", "Inter", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

/* System font fallback */
--font-system: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;

/* Display/Marketing font */
--font-display: "Brutal Type Bold", "Inter Bold", sans-serif;

/* Monospace (codes, technical) */
--font-mono: "JetBrains Mono", "Fira Code", Consolas, Monaco, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Title | 48px | Bold | 56px | -0.02em | `--text-primary` |
| Page Title | 32px | Bold | 40px | -0.01em | `--text-primary` |
| Section Header | 24px | SemiBold | 32px | 0 | `--text-primary` |
| Card Title | 16px | Medium | 22px | 0 | `--text-primary` |
| Subtitle | 14px | Regular | 20px | 0 | `--text-secondary` |
| Body Text | 14px | Regular | 22px | 0.01em | `--text-primary` |
| Body Small | 13px | Regular | 18px | 0 | `--text-secondary` |
| Caption | 12px | Regular | 16px | 0.02em | `--text-tertiary` |
| Button Text | 14px | SemiBold | 20px | 0.02em | `--text-primary` |
| Price (Large) | 20px | Bold | 24px | 0 | `--text-primary` |
| Price (Small) | 14px | Medium | 18px | 0 | `--text-primary` |
| Badge Text | 11px | Bold | 14px | 0.05em | `--text-primary` |
| Nav Item | 13px | Medium | 18px | 0.01em | `--text-secondary` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, descriptions |
| 500 | Medium | Card titles, navigation, emphasized text |
| 600 | SemiBold | Section headers, buttons |
| 700 | Bold | Hero titles, page titles, prices |

### Marketing Typography

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Campaign Headline | 64px | Bold | Major sale events, launches |
| Feature Title | 40px | Bold | Featured game spotlights |
| Promo Subtitle | 20px | Regular | Campaign descriptions |
| Banner CTA | 16px | SemiBold | Call-to-action buttons |
| Free Badge | 14px | Bold | "FREE" label uppercase |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Blue)
```css
.button-primary {
  background: #0074e4;
  border: none;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 12px 24px;
  height: 44px;
  cursor: pointer;
  transition: background 150ms ease;
}

.button-primary:hover {
  background: #0084ff;
}

.button-primary:active {
  background: #0066cc;
}

.button-primary:disabled {
  background: #303030;
  color: #6b6b6b;
  cursor: not-allowed;
}
```

#### Secondary Button (Outlined)
```css
.button-secondary {
  background: transparent;
  border: 2px solid #505050;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 10px 22px;
  height: 44px;
  cursor: pointer;
  transition: all 150ms ease;
}

.button-secondary:hover {
  border-color: #ffffff;
  background: rgba(255, 255, 255, 0.05);
}
```

#### Tertiary Button (Ghost)
```css
.button-tertiary {
  background: transparent;
  border: none;
  color: #0074e4;
  font-size: 14px;
  font-weight: 600;
  padding: 12px 16px;
  cursor: pointer;
}

.button-tertiary:hover {
  color: #26bbff;
  text-decoration: underline;
}
```

#### Add to Cart Button
```css
.button-cart {
  background: #0074e4;
  border: none;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 14px 28px;
  height: 48px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.button-cart:hover {
  background: #0084ff;
}
```

#### Free Game Button
```css
.button-free {
  background: #f5a623;
  border: none;
  border-radius: 8px;
  color: #000000;
  font-size: 14px;
  font-weight: 700;
  padding: 14px 28px;
  height: 48px;
}

.button-free:hover {
  background: #ffcc00;
}
```

### Inputs

#### Search Input
```css
.search-input {
  background: #202020;
  border: 1px solid #303030;
  border-radius: 24px;
  color: #ffffff;
  font-size: 14px;
  padding: 12px 20px;
  padding-left: 44px;
  width: 100%;
  transition: all 150ms ease;
}

.search-input:focus {
  border-color: #0074e4;
  outline: none;
  background: #2a2a2a;
}

.search-input::placeholder {
  color: #6b6b6b;
}

.search-icon {
  position: absolute;
  left: 16px;
  color: #6b6b6b;
  width: 20px;
  height: 20px;
}
```

#### Text Input
```css
.input-text {
  background: #303030;
  border: 1px solid #404040;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  padding: 12px 16px;
  height: 48px;
}

.input-text:focus {
  border-color: #0074e4;
  outline: none;
}

.input-text:disabled {
  background: #202020;
  color: #6b6b6b;
}
```

#### Select Dropdown
```css
.select {
  background: #303030;
  border: 1px solid #404040;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  padding: 12px 40px 12px 16px;
  height: 48px;
  appearance: none;
  cursor: pointer;
}

.select:focus {
  border-color: #0074e4;
  outline: none;
}
```

### Cards

#### Game Card (Standard)
```css
.game-card {
  background: #202020;
  border-radius: 12px;
  overflow: hidden;
  position: relative;
  cursor: pointer;
  transition: transform 200ms ease, box-shadow 200ms ease;
}

.game-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.4);
}

.game-card-image {
  width: 100%;
  aspect-ratio: 16/9;
  object-fit: cover;
}

.game-card-info {
  padding: 16px;
}

.game-card-title {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  margin-bottom: 8px;
  line-height: 1.4;
}

.game-card-meta {
  color: #6b6b6b;
  font-size: 12px;
}
```

#### Game Card (Large/Featured)
```css
.game-card-featured {
  background: #202020;
  border-radius: 16px;
  overflow: hidden;
  position: relative;
  aspect-ratio: 16/9;
}

.game-card-featured-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.game-card-featured-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 32px;
  background: linear-gradient(to top, rgba(0, 0, 0, 0.9) 0%, transparent 100%);
}

.game-card-featured-title {
  color: #ffffff;
  font-size: 28px;
  font-weight: 700;
  margin-bottom: 8px;
}
```

#### Free Game Card
```css
.free-game-card {
  background: linear-gradient(135deg, #1a1a1a 0%, #121212 100%);
  border: 1px solid #f5a623;
  border-radius: 12px;
  overflow: hidden;
  position: relative;
}

.free-game-badge {
  position: absolute;
  top: 12px;
  left: 12px;
  background: #f5a623;
  color: #000000;
  font-size: 11px;
  font-weight: 700;
  text-transform: uppercase;
  padding: 4px 10px;
  border-radius: 4px;
  letter-spacing: 0.05em;
}

.free-game-timer {
  color: #f5a623;
  font-size: 12px;
  font-weight: 500;
}
```

#### Library Game Card
```css
.library-card {
  background: #202020;
  border-radius: 8px;
  display: flex;
  align-items: center;
  padding: 12px;
  gap: 16px;
  cursor: pointer;
  transition: background 150ms ease;
}

.library-card:hover {
  background: #2a2a2a;
}

.library-card.selected {
  background: #303030;
  border-left: 3px solid #0074e4;
}

.library-card-icon {
  width: 48px;
  height: 48px;
  border-radius: 8px;
  object-fit: cover;
}

.library-card-name {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
}

.library-card-status {
  color: #6b6b6b;
  font-size: 12px;
}
```

### Price Tags

#### Standard Price
```css
.price-tag {
  display: flex;
  align-items: center;
  gap: 8px;
}

.price-current {
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
}
```

#### Discounted Price
```css
.price-discounted {
  display: flex;
  align-items: center;
  gap: 12px;
}

.discount-badge {
  background: #00e676;
  color: #000000;
  font-size: 14px;
  font-weight: 700;
  padding: 6px 10px;
  border-radius: 6px;
}

.price-original {
  color: #6b6b6b;
  font-size: 14px;
  text-decoration: line-through;
}

.price-final {
  color: #ffffff;
  font-size: 16px;
  font-weight: 600;
}
```

#### Free Price Tag
```css
.price-free {
  background: #f5a623;
  color: #000000;
  font-size: 14px;
  font-weight: 700;
  padding: 8px 16px;
  border-radius: 6px;
  text-transform: uppercase;
}
```

### Navigation

#### Main Header
```css
.header-main {
  background: #121212;
  height: 64px;
  display: flex;
  align-items: center;
  padding: 0 24px;
  border-bottom: 1px solid #202020;
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-logo {
  width: 32px;
  height: 36px;
  margin-right: 24px;
}

.header-search {
  flex: 1;
  max-width: 400px;
}

.header-actions {
  display: flex;
  align-items: center;
  gap: 16px;
  margin-left: auto;
}
```

#### Left Sidebar
```css
.sidebar {
  width: 240px;
  background: #18181c;
  padding: 24px 0;
  height: 100vh;
  position: fixed;
  left: 0;
  top: 64px;
}

.sidebar-section {
  padding: 0 16px;
  margin-bottom: 24px;
}

.sidebar-section-title {
  color: #6b6b6b;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  padding: 8px 12px;
}

.sidebar-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 12px;
  border-radius: 8px;
  color: #a8a8a8;
  font-size: 13px;
  font-weight: 500;
  cursor: pointer;
  transition: all 150ms ease;
}

.sidebar-item:hover {
  background: #202020;
  color: #ffffff;
}

.sidebar-item.active {
  background: #0074e4;
  color: #ffffff;
}

.sidebar-item-icon {
  width: 20px;
  height: 20px;
}
```

#### Tab Navigation
```css
.tabs {
  display: flex;
  gap: 0;
  border-bottom: 1px solid #303030;
}

.tab {
  padding: 16px 24px;
  color: #a8a8a8;
  font-size: 14px;
  font-weight: 500;
  border: none;
  background: transparent;
  cursor: pointer;
  position: relative;
}

.tab:hover {
  color: #ffffff;
}

.tab.active {
  color: #ffffff;
}

.tab.active::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: #0074e4;
}
```

### Cart & Wishlist

#### Cart Icon Button
```css
.cart-button {
  position: relative;
  background: transparent;
  border: none;
  padding: 8px;
  cursor: pointer;
}

.cart-icon {
  width: 24px;
  height: 24px;
  color: #ffffff;
}

.cart-badge {
  position: absolute;
  top: 0;
  right: 0;
  background: #0074e4;
  color: #ffffff;
  font-size: 10px;
  font-weight: 700;
  min-width: 18px;
  height: 18px;
  border-radius: 9px;
  display: flex;
  align-items: center;
  justify-content: center;
}
```

#### Cart Dropdown
```css
.cart-dropdown {
  position: absolute;
  top: 100%;
  right: 0;
  width: 380px;
  background: #202020;
  border-radius: 12px;
  padding: 16px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.5);
}

.cart-item {
  display: flex;
  gap: 12px;
  padding: 12px 0;
  border-bottom: 1px solid #303030;
}

.cart-item-image {
  width: 80px;
  height: 45px;
  border-radius: 4px;
  object-fit: cover;
}

.cart-item-title {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
}

.cart-item-price {
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  margin-left: auto;
}

.cart-total {
  display: flex;
  justify-content: space-between;
  padding-top: 16px;
  font-size: 16px;
  font-weight: 600;
}
```

#### Wishlist Button
```css
.wishlist-button {
  background: transparent;
  border: 2px solid #505050;
  border-radius: 8px;
  width: 48px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 150ms ease;
}

.wishlist-button:hover {
  border-color: #ffffff;
  background: rgba(255, 255, 255, 0.05);
}

.wishlist-button.active {
  background: #0074e4;
  border-color: #0074e4;
}

.wishlist-icon {
  width: 20px;
  height: 20px;
  color: #ffffff;
}
```

### Social Features

#### Friend Row
```css
.friend-row {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  gap: 12px;
  cursor: pointer;
  border-radius: 8px;
  transition: background 150ms ease;
}

.friend-row:hover {
  background: #2a2a2a;
}

.friend-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  position: relative;
}

.friend-status-dot {
  position: absolute;
  bottom: 0;
  right: 0;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  border: 2px solid #121212;
}

.friend-status-dot.online {
  background: #00e676;
}

.friend-status-dot.in-game {
  background: #0074e4;
}

.friend-status-dot.offline {
  background: #505050;
}

.friend-info {
  flex: 1;
}

.friend-name {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
}

.friend-activity {
  color: #6b6b6b;
  font-size: 12px;
}

.friend-activity.in-game {
  color: #0074e4;
}
```

#### Achievement Card
```css
.achievement-card {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #202020;
  border-radius: 12px;
}

.achievement-icon {
  width: 64px;
  height: 64px;
  border-radius: 8px;
}

.achievement-icon.locked {
  opacity: 0.3;
  filter: grayscale(100%);
}

.achievement-info {
  flex: 1;
}

.achievement-name {
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  margin-bottom: 4px;
}

.achievement-description {
  color: #a8a8a8;
  font-size: 13px;
}

.achievement-rarity {
  color: #0074e4;
  font-size: 12px;
  font-weight: 500;
}

.achievement-progress {
  width: 100%;
  height: 4px;
  background: #303030;
  border-radius: 2px;
  margin-top: 8px;
}

.achievement-progress-fill {
  height: 100%;
  background: #0074e4;
  border-radius: 2px;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.85);
  backdrop-filter: blur(8px);
}

.modal {
  background: #202020;
  border-radius: 16px;
  max-width: 560px;
  width: 90%;
  overflow: hidden;
  box-shadow: 0 24px 64px rgba(0, 0, 0, 0.5);
}

.modal-header {
  padding: 24px 24px 0;
}

.modal-title {
  color: #ffffff;
  font-size: 24px;
  font-weight: 600;
}

.modal-close {
  position: absolute;
  top: 16px;
  right: 16px;
  background: transparent;
  border: none;
  color: #6b6b6b;
  cursor: pointer;
  padding: 8px;
}

.modal-close:hover {
  color: #ffffff;
}

.modal-body {
  padding: 24px;
  color: #a8a8a8;
}

.modal-footer {
  padding: 16px 24px 24px;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
}
```

### Tooltips

```css
.tooltip {
  background: #303030;
  border-radius: 8px;
  padding: 12px 16px;
  color: #ffffff;
  font-size: 13px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.4);
  max-width: 280px;
}

.tooltip-arrow {
  fill: #303030;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | 4px | Tight gaps, icon spacing |
| `--spacing-sm` | 8px | Component internal padding |
| `--spacing-md` | 12px | Small gaps between elements |
| `--spacing-lg` | 16px | Standard gaps, card padding |
| `--spacing-xl` | 24px | Section spacing |
| `--spacing-2xl` | 32px | Major section breaks |
| `--spacing-3xl` | 48px | Page section margins |
| `--spacing-4xl` | 64px | Hero section padding |

### Core Layout Structure

```
+------------------------------------------------------------------+
|  Header (Logo, Search, Cart, User)                       64px    |
+----------+-------------------------------------------------------+
|          |                                                       |
| Sidebar  |              Main Content Area                        |
|          |                                                       |
|  240px   |              Flexible (min 960px)                     |
|          |                                                       |
| - Store  |  +-------------------------------------------+        |
| - Library|  |     Featured Hero Carousel                |        |
| - Friends|  +-------------------------------------------+        |
| - etc.   |                                                       |
|          |  +-------------------------------------------+        |
|          |  |     Content Sections (Grid/Carousel)      |        |
|          |  +-------------------------------------------+        |
|          |                                                       |
+----------+-------------------------------------------------------+
```

### Store Page Layout

```
+------------------------------------------------------------------+
|                    Featured Carousel (Full Width)                |
|                    Aspect Ratio: 21:9 (2560x1080)                |
+------------------------------------------------------------------+
|                                                                  |
|  Free Games This Week                                            |
|  +------------+ +------------+ +------------+ +------------+     |
|  |  FREE      | |  FREE      | |  COMING    | |            |     |
|  |  GAME 1    | |  GAME 2    | |  SOON      | |    ...     |     |
|  +------------+ +------------+ +------------+ +------------+     |
|                                                                  |
+------------------------------------------------------------------+
|                                                                  |
|  Top New Releases                                                |
|  +--------+ +--------+ +--------+ +--------+ +--------+ +-----+  |
|  |  GAME  | |  GAME  | |  GAME  | |  GAME  | |  GAME  | | ... |  |
|  +--------+ +--------+ +--------+ +--------+ +--------+ +-----+  |
|                                                                  |
+------------------------------------------------------------------+
```

### Library Layout

```
+----------+-------------------------------------------------------+
| Games    |                                                       |
| Filter   |           Currently Selected Game                     |
|          |  +-------------------------------------------+        |
| [Search] |  |            Hero Background                |        |
|          |  |                                           |        |
| All (42) |  |    +------+                               |        |
| Installed|  |    | PLAY |  Game Title                   |        |
| Favorites|  |    +------+  Developer                    |        |
|          |  +-------------------------------------------+        |
| -------- |                                                       |
|          |  +-------------------------------------------+        |
| Game 1   |  |  Activity | Achievements | Cloud Saves   |        |
| Game 2   |  +-------------------------------------------+        |
| Game 3   |  |                                           |        |
| Game 4   |  |     Content based on selected tab         |        |
| Game 5   |  |                                           |        |
+----------+-------------------------------------------------------+
```

### Content Widths

| Context | Width | Notes |
|---------|-------|-------|
| Content container (max) | 1600px | Centered with auto margins |
| Store grid | 1440px | 4-5 column game grid |
| Detail page | 1200px | Game detail content |
| Modal small | 400px | Simple confirmations |
| Modal medium | 560px | Forms, settings |
| Modal large | 800px | Complex dialogs |
| Sidebar | 240px | Fixed width |

### Game Image Sizes

| Type | Dimensions | Aspect Ratio | Usage |
|------|------------|--------------|-------|
| Hero/Featured | 2560×1080 | 21:9 | Carousel hero images |
| Landscape Wide | 1920×1080 | 16:9 | Game detail hero |
| Card Standard | 400×225 | 16:9 | Store cards |
| Card Tall | 600×800 | 3:4 | Vertical game cards |
| Thumbnail | 200×112 | 16:9 | List views, cart |
| Icon | 256×256 | 1:1 | Library icons |
| Logo | Variable | Variable | Game logos (PNG) |

### Whitespace Philosophy
- **Generous and premium**: Content has room to breathe
- **Clear visual hierarchy**: Sections clearly separated
- **Focus on imagery**: Games are visual-first
- **Consistent rhythm**: Regular spacing creates calm experience
- **Responsive scaling**: Spacing reduces proportionally on smaller screens

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Flat surfaces, base elements |
| Level 1 | `0 2px 8px rgba(0,0,0,0.2)` | Subtle lift, cards at rest |
| Level 2 | `0 4px 16px rgba(0,0,0,0.3)` | Hovered cards |
| Level 3 | `0 8px 24px rgba(0,0,0,0.4)` | Dropdowns, elevated cards |
| Level 4 | `0 16px 48px rgba(0,0,0,0.5)` | Modals, important overlays |
| Level 5 | `0 24px 64px rgba(0,0,0,0.6)` | Full-screen overlays |

### Surface Hierarchy

```
+------------------------------------------------------------------+
| Modal/Overlay                              #202020 + Level 4      |
+------------------------------------------------------------------+
| Dropdown/Popover                           #303030 + Level 3      |
+------------------------------------------------------------------+
| Card Hover                                 #2a2a2a + Level 2      |
+------------------------------------------------------------------+
| Card/Elevated                              #202020 + Level 1      |
+------------------------------------------------------------------+
| Primary Content                            #121212               |
+------------------------------------------------------------------+
| Sidebar/Recessed                           #18181c               |
+------------------------------------------------------------------+
| Deepest (overlay backdrop)                 #000000               |
+------------------------------------------------------------------+
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, game cards |
| Sticky | 10 | Section headers within scroll |
| Header | 100 | Main navigation header |
| Sidebar | 50 | Left sidebar (below header) |
| Dropdown | 200 | Search results, menus |
| Popover | 300 | Quick actions, tooltips |
| Modal | 400 | Dialogs, confirmations |
| Toast | 500 | Notifications |
| Tooltip | 600 | Help tooltips |

### Gradient Treatments

```css
/* Hero image overlay (bottom fade) */
.hero-overlay {
  background: linear-gradient(
    to top,
    rgba(18, 18, 18, 1) 0%,
    rgba(18, 18, 18, 0.8) 20%,
    transparent 60%
  );
}

/* Card hover glow */
.card-glow:hover {
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.4),
              0 0 0 1px rgba(0, 116, 228, 0.2);
}

/* Free game banner gradient */
.free-game-gradient {
  background: linear-gradient(
    135deg,
    rgba(245, 166, 35, 0.2) 0%,
    transparent 50%
  );
}

/* Blue accent gradient */
.accent-gradient {
  background: linear-gradient(
    135deg,
    #0074e4 0%,
    #26bbff 100%
  );
}
```

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use pure black (#121212) as primary background | Cinematic, premium feel |
| Make free games prominent with yellow (#f5a623) | Core value proposition |
| Use blue (#0074e4) consistently for primary actions | Clear interaction patterns |
| Let game artwork fill cards edge-to-edge | Visual-first experience |
| Apply generous border-radius (8-16px) | Modern, friendly aesthetic |
| Show countdown timers on free game offers | Creates urgency |
| Use full-bleed hero images | Cinematic impact |
| Keep navigation minimal and clean | Focus on content |
| Show "In Library" badges on owned games | Prevents confusion |
| Include social proof (friends who own game) | Community connection |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Don't use light backgrounds | Breaks dark theme immersion |
| Avoid sharp corners (< 8px radius) | Feels dated, less premium |
| Don't hide free game offers | Core differentiator |
| Avoid cluttered layouts | Epic favors curation over density |
| Don't use colored text for body copy | Maintain readability |
| Avoid small, cramped touch targets | Mobile/controller accessibility |
| Don't obscure game artwork with overlays | Games should be the hero |
| Avoid auto-playing video with sound | Respect user attention |
| Don't use generic placeholder images | Quality matters |
| Avoid inconsistent icon styles | Maintain visual coherence |

### Content Guidelines

| Do | Don't |
|----|-------|
| Clear, prominent pricing | Hidden costs or unclear pricing |
| Show platform compatibility icons | Assume single platform |
| Display file size for downloads | Surprise users with storage needs |
| Include age ratings | Skip content warnings |
| Show "Free" prominently when applicable | Bury free offers |
| Display refund policy clearly | Hide return information |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Desktop XL | >1600px | Full layout, 5-column grids |
| Desktop | 1200px - 1600px | Standard layout, 4-column grids |
| Desktop SM | 960px - 1199px | Compact layout, 3-column grids |
| Tablet | 768px - 959px | Sidebar collapses, 2-column grids |
| Mobile | <768px | Single column, bottom navigation |

### Desktop Scaling

| Viewport | Content Width | Grid Columns | Sidebar |
|----------|---------------|--------------|---------|
| >1600px | 1440px | 5 | 240px |
| 1200-1600px | 1200px | 4 | 240px |
| 960-1199px | 100% - 48px | 3 | 200px |
| <960px | 100% - 32px | 2 | Collapsed |

### Component Adaptations

| Component | Desktop | Tablet | Mobile |
|-----------|---------|--------|--------|
| Sidebar | Fixed visible | Collapsible drawer | Bottom sheet |
| Game Grid | 4-5 columns | 2-3 columns | 1-2 columns |
| Hero Carousel | Full width 21:9 | Full width 16:9 | Full width 4:3 |
| Cart | Dropdown | Dropdown | Full page |
| Search | Header input | Icon + modal | Icon + full screen |
| Game Cards | Hover effects | Touch effects | Tap to expand |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Buttons | 44px × 44px | WCAG 2.1 compliant |
| Navigation items | 48px height | Comfortable tapping |
| Game cards | 160px min width | Visible and tappable |
| Close buttons | 44px × 44px | Easy dismissal |
| Cart items | 72px height | Clear tap zones |

### Image Handling

| Type | Desktop | Tablet | Mobile |
|------|---------|--------|--------|
| Hero | 2560×1080 | 1920×1080 | 1280×960 |
| Cards | 400×225 | 300×169 | Full width |
| Thumbnails | 200×112 | 160×90 | 120×67 |
| Load Strategy | Eager | Lazy | Lazy + LQIP |

### Mobile Specific

```css
/* Bottom navigation for mobile */
.mobile-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 64px;
  background: #18181c;
  border-top: 1px solid #303030;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-bottom: env(safe-area-inset-bottom);
}

/* Safe areas */
.content-area {
  padding-left: env(safe-area-inset-left);
  padding-right: env(safe-area-inset-right);
}
```

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
Primary Background: #121212
Secondary Background: #202020
Sidebar Background: #18181c
Elevated Surface: #303030

Accent Primary (Blue): #0074e4
Accent Hover: #0084ff
Free Game Yellow: #f5a623
Sale Green: #00e676

Text Primary: #ffffff
Text Secondary: #a8a8a8
Text Tertiary: #6b6b6b
Text Link: #0074e4

Status Online: #00e676
Status In-Game: #0074e4
Status Offline: #505050

Border Radius Small: 8px
Border Radius Medium: 12px
Border Radius Large: 16px
Border Radius Full: 9999px (pills)

Font Primary: "Brutal Type", system fonts
Font Size Body: 14px
Font Size Title: 24-48px
Font Weight Normal: 400
Font Weight Medium: 500
Font Weight SemiBold: 600
Font Weight Bold: 700
```

### Example Prompts

#### Store Game Card
```
Create an Epic Games Store game card:
- Card background: #202020
- Border-radius: 12px
- Game image: 16:9 aspect ratio, full bleed
- Title: 14px medium #ffffff below image
- Developer: 12px #6b6b6b
- Price: 14px semibold #ffffff
- Hover: translateY(-4px) with shadow 0 8px 24px rgba(0,0,0,0.4)
- For free games: Add yellow "FREE" badge top-left
```

#### Free Game Banner
```
Design an Epic free game promotion card:
- Border: 1px solid #f5a623
- "FREE" badge: #f5a623 background, #000000 text, 11px bold uppercase
- Timer: #f5a623 text showing "Free until [date]"
- CTA button: #f5a623 background, #000000 text
- Gradient overlay: subtle yellow to transparent
```

#### Primary Button
```
Create Epic Games Store primary button:
- Background: #0074e4
- Border-radius: 8px
- Text: 14px semibold #ffffff
- Padding: 12px 24px
- Height: 44px
- Hover: background #0084ff
- Active: background #0066cc
- Disabled: background #303030, color #6b6b6b
```

#### Library Game Entry
```
Design a library game list item:
- Container: #202020 background, 8px radius
- Padding: 12px
- Game icon: 48px square with 8px radius
- Name: 14px medium #ffffff
- Status: 12px #6b6b6b (installed, not installed, update)
- Hover: background #2a2a2a
- Selected: background #303030, 3px left border #0074e4
```

#### Cart Dropdown
```
Create a shopping cart dropdown:
- Container: #202020, 12px radius, 380px width
- Shadow: 0 8px 32px rgba(0,0,0,0.5)
- Item row: game thumbnail (80x45), title, price
- Divider: 1px #303030
- Total row: 16px semibold
- Checkout button: full width #0074e4 primary button
```

### CSS Variables Template

```css
:root {
  /* Backgrounds */
  --bg-pure-black: #000000;
  --bg-primary: #121212;
  --bg-secondary: #202020;
  --bg-tertiary: #2a2a2a;
  --bg-elevated: #303030;
  --bg-input: #3a3a3a;
  --bg-sidebar: #18181c;
  
  /* Accent */
  --accent-primary: #0074e4;
  --accent-primary-hover: #0084ff;
  --accent-primary-active: #0066cc;
  --accent-secondary: #26bbff;
  --free-yellow: #f5a623;
  --sale-green: #00e676;
  
  /* Text */
  --text-primary: #ffffff;
  --text-secondary: #a8a8a8;
  --text-tertiary: #6b6b6b;
  --text-muted: #505050;
  --text-link: #0074e4;
  
  /* Status */
  --status-online: #00e676;
  --status-in-game: #0074e4;
  --status-away: #f5a623;
  --status-offline: #505050;
  
  /* Semantic */
  --success: #00e676;
  --warning: #f5a623;
  --error: #f44336;
  --info: #26bbff;
  
  /* Typography */
  --font-primary: "Brutal Type", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  --font-size-xs: 11px;
  --font-size-sm: 12px;
  --font-size-base: 14px;
  --font-size-lg: 16px;
  --font-size-xl: 20px;
  --font-size-2xl: 24px;
  --font-size-3xl: 32px;
  --font-size-4xl: 48px;
  
  /* Spacing */
  --spacing-xs: 4px;
  --spacing-sm: 8px;
  --spacing-md: 12px;
  --spacing-lg: 16px;
  --spacing-xl: 24px;
  --spacing-2xl: 32px;
  --spacing-3xl: 48px;
  --spacing-4xl: 64px;
  
  /* Borders */
  --radius-sm: 8px;
  --radius-md: 12px;
  --radius-lg: 16px;
  --radius-full: 9999px;
  
  /* Shadows */
  --shadow-sm: 0 2px 8px rgba(0, 0, 0, 0.2);
  --shadow-md: 0 4px 16px rgba(0, 0, 0, 0.3);
  --shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.4);
  --shadow-xl: 0 16px 48px rgba(0, 0, 0, 0.5);
}
```

---

## Summary

Epic Games Store's design system creates a premium, cinematic gaming marketplace through:

1. **Deep black palette** (#121212 → #000000) for immersive, theater-like experience
2. **Vibrant blue accent (#0074e4)** for clear, confident interactions
3. **Bold yellow (#f5a623)** celebrating free games as a core value proposition
4. **Generous border-radius (8-16px)** for modern, approachable aesthetic
5. **Full-bleed imagery** letting games speak for themselves
6. **Medium density layouts** with breathing room between elements
7. **Clean typography** using Brutal Type for distinctive brand voice

When implementing Epic Games Store-style interfaces, prioritize:
- Dark, cinematic backgrounds that make game art pop
- Clear visual hierarchy with prominent free game offers
- Smooth hover transitions and elevation changes
- Consistent blue for actions, yellow for free, green for sales
- Mobile-first touch targets with responsive adaptations
- Social features that connect players with friends
- Premium spacing that creates calm, focused browsing
