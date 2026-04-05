# PlayStation Design System

> Premium gaming ecosystem with iconic blue identity. PlayStation Blue (#003791), dark immersive backgrounds, SST typography, trophy achievements, and controller-centric interactions.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
PlayStation embodies a **premium, immersive gaming** design philosophy. The interface is sleek, cinematic, and confident—designed to showcase games as the stars while maintaining Sony's sophisticated brand identity. Every element communicates quality, innovation, and the excitement of gaming.

### Mood & Feeling
- **Premium & Confident**: Deep blacks and signature PlayStation Blue convey sophistication
- **Cinematic**: Large imagery, smooth transitions, and theatrical presentation
- **Achievement-driven**: Trophy system, progress tracking, and status displays
- **Social yet personal**: Friends lists, parties, and shared experiences alongside individual libraries
- **Console-native**: Designed for controllers first, then adapted for web/mobile

### Design Density
**Low-to-medium density** with generous whitespace. Content is hero-sized with focus on game artwork. Navigation is minimal and peripheral, keeping the spotlight on games and media. Cards are large and touch-friendly.

### Visual Character
- Iconic PlayStation Blue as the signature accent
- Deep black backgrounds creating theater-like immersion
- Game artwork as primary visual content (hero images, box art)
- Smooth, sweeping animations and transitions
- Rounded corners with subtle glows and highlights
- Trophy iconography integrated throughout
- Controller button prompts as UI elements

---

## 2. Color Palette & Roles

### Primary Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--ps-blue-primary` | `#003791` | Core PlayStation Blue, headers, key branding |
| `--ps-blue-light` | `#0070d1` | Interactive elements, links, highlights |
| `--ps-blue-bright` | `#00bfff` | Accent highlights, active states |
| `--ps-white` | `#ffffff` | Primary text, icons on dark backgrounds |

### Background Colors

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#000000` | Main app background, pure black for OLED |
| `--background-secondary` | `#1f1f1f` | Cards, panels, elevated surfaces |
| `--background-tertiary` | `#2d2d2d` | Hover states, input fields |
| `--background-elevated` | `#383838` | Modals, dropdowns, popovers |
| `--background-gradient-start` | `#000000` | Gradient overlays on hero images |
| `--background-gradient-end` | `transparent` | Fade to image content |

### PS Plus & Subscription Colors

| Token | Hex | Role |
|-------|-----|------|
| `--ps-plus-yellow` | `#ffb800` | PS Plus branding, premium badge |
| `--ps-plus-gold` | `#d4af37` | PS Plus Premium tier |
| `--ps-plus-gradient-start` | `#ffb800` | PS Plus gradient |
| `--ps-plus-gradient-end` | `#ff8c00` | PS Plus gradient end |
| `--ps-now-blue` | `#0070d1` | Streaming service accent |

### Trophy System Colors

| Token | Hex | Role |
|-------|-----|------|
| `--trophy-platinum` | `#7b9fcc` | Platinum trophy (rarest) |
| `--trophy-gold` | `#cd9a1a` | Gold trophy |
| `--trophy-silver` | `#a8a8a8` | Silver trophy |
| `--trophy-bronze` | `#cd7f32` | Bronze trophy (most common) |
| `--trophy-glow` | `rgba(123, 159, 204, 0.4)` | Trophy highlight glow |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--text-primary` | `#ffffff` | Primary headings, game titles |
| `--text-secondary` | `#b3b3b3` | Body text, descriptions |
| `--text-tertiary` | `#808080` | Metadata, timestamps, muted info |
| `--text-link` | `#0070d1` | Hyperlinks, interactive text |
| `--text-disabled` | `#4a4a4a` | Disabled states |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--success` | `#00c853` | Purchase complete, download finished |
| `--warning` | `#ffb800` | Storage warnings, update available |
| `--error` | `#ff4444` | Errors, failed downloads |
| `--info` | `#0070d1` | Informational messages |
| `--online` | `#00c853` | Online status indicator |
| `--offline` | `#808080` | Offline status |
| `--busy` | `#ff4444` | Do not disturb |

### Gradient Definitions

| Name | Definition | Usage |
|------|------------|-------|
| Hero Overlay | `linear-gradient(to top, #000000 0%, transparent 60%)` | Game hero images |
| PS Blue Gradient | `linear-gradient(135deg, #003791 0%, #0070d1 100%)` | Featured sections |
| PS Plus Gradient | `linear-gradient(135deg, #ffb800 0%, #ff8c00 100%)` | PS Plus badges |
| Card Hover | `linear-gradient(180deg, transparent 0%, rgba(0,112,209,0.2) 100%)` | Hover effects |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary PlayStation font */
--font-primary: 'SST', 'Sony SST', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;

/* Condensed variant for tight spaces */
--font-condensed: 'SST Condensed', 'SST', sans-serif;

/* Japanese variant */
--font-japanese: 'SST Japanese', 'Hiragino Sans', 'Yu Gothic', sans-serif;

/* System fallback */
--font-system: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Title | 48px | 700 | 1.1 | -0.02em | `--text-primary` |
| Page Title | 32px | 700 | 1.2 | -0.01em | `--text-primary` |
| Section Header | 24px | 600 | 1.3 | 0 | `--text-primary` |
| Card Title | 18px | 600 | 1.3 | 0 | `--text-primary` |
| Subsection | 16px | 600 | 1.4 | 0 | `--text-primary` |
| Body Large | 16px | 400 | 1.5 | 0 | `--text-secondary` |
| Body Regular | 14px | 400 | 1.5 | 0 | `--text-secondary` |
| Body Small | 13px | 400 | 1.4 | 0 | `--text-tertiary` |
| Caption | 12px | 400 | 1.4 | 0.01em | `--text-tertiary` |
| Button Text | 14px | 600 | 1 | 0.02em | `--text-primary` |
| Price | 18px | 700 | 1 | 0 | `--text-primary` |
| Price Sale | 18px | 700 | 1 | 0 | `--ps-plus-yellow` |
| Badge | 11px | 700 | 1 | 0.05em | `--text-primary` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 300 | Light | Large display text, promotional |
| 400 | Regular | Body text, descriptions |
| 500 | Medium | UI labels, navigation |
| 600 | Semibold | Card titles, section headers |
| 700 | Bold | Page titles, prices, emphasis |

### Marketing Typography

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Campaign Hero | 72px | 700 | Major launches, events |
| Event Title | 56px | 700 | State of Play, showcases |
| Feature Headline | 40px | 600 | Feature section headers |
| Tagline | 24px | 400 | Supporting copy |

---

## 4. Component Stylings

### Buttons

#### Primary Button (PS Blue)
```css
.button-primary {
  background: linear-gradient(180deg, #0070d1 0%, #005bb5 100%);
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 12px 24px;
  min-height: 44px;
  border-radius: 22px;
  border: none;
  text-transform: none;
  transition: all 200ms ease;
  box-shadow: 0 2px 8px rgba(0, 112, 209, 0.3);
}

.button-primary:hover {
  background: linear-gradient(180deg, #0080e6 0%, #0070d1 100%);
  transform: translateY(-1px);
  box-shadow: 0 4px 12px rgba(0, 112, 209, 0.4);
}

.button-primary:active {
  background: #005bb5;
  transform: translateY(0);
}

.button-primary:disabled {
  background: #383838;
  color: #808080;
  box-shadow: none;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.button-secondary {
  background: transparent;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 12px 24px;
  min-height: 44px;
  border-radius: 22px;
  border: 2px solid #ffffff;
  transition: all 200ms ease;
}

.button-secondary:hover {
  background: rgba(255, 255, 255, 0.1);
  border-color: #0070d1;
  color: #0070d1;
}
```

#### Add to Cart Button
```css
.button-cart {
  background: #0070d1;
  color: #ffffff;
  font-size: 16px;
  font-weight: 700;
  padding: 16px 32px;
  border-radius: 4px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
}

.button-cart:hover {
  background: #0080e6;
}
```

#### Icon Button
```css
.button-icon {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.1);
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #ffffff;
  transition: all 200ms ease;
}

.button-icon:hover {
  background: rgba(255, 255, 255, 0.2);
}

.button-icon:focus {
  outline: 2px solid #0070d1;
  outline-offset: 2px;
}
```

### Game Cards

#### Standard Game Card
```css
.game-card {
  background: #1f1f1f;
  border-radius: 8px;
  overflow: hidden;
  transition: all 300ms cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
  position: relative;
}

.game-card:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 32px rgba(0, 112, 209, 0.3);
  z-index: 10;
}

.game-card:focus {
  outline: 3px solid #0070d1;
  outline-offset: 2px;
}

.game-card-image {
  width: 100%;
  aspect-ratio: 1 / 1; /* Square box art */
  object-fit: cover;
}

.game-card-content {
  padding: 12px;
}

.game-card-title {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 4px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.game-card-platform {
  font-size: 12px;
  color: #808080;
}

.game-card-price {
  font-size: 16px;
  font-weight: 700;
  color: #ffffff;
  margin-top: 8px;
}

.game-card-price-sale {
  color: #ffb800;
}

.game-card-price-original {
  font-size: 14px;
  font-weight: 400;
  color: #808080;
  text-decoration: line-through;
  margin-right: 8px;
}
```

#### Featured Game Card (Large)
```css
.game-card-featured {
  aspect-ratio: 16 / 9;
  position: relative;
  border-radius: 12px;
  overflow: hidden;
}

.game-card-featured-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 24px;
  background: linear-gradient(to top, rgba(0, 0, 0, 0.9) 0%, transparent 100%);
}

.game-card-featured-title {
  font-size: 28px;
  font-weight: 700;
  color: #ffffff;
  margin-bottom: 8px;
}

.game-card-featured-meta {
  font-size: 14px;
  color: #b3b3b3;
}
```

### Badges & Tags

#### PS Plus Badge
```css
.badge-ps-plus {
  background: linear-gradient(135deg, #ffb800 0%, #ff8c00 100%);
  color: #000000;
  font-size: 11px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 4px;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

#### Discount Badge
```css
.badge-discount {
  background: #0070d1;
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 4px;
}
```

#### Platform Badge
```css
.badge-platform {
  background: rgba(255, 255, 255, 0.1);
  color: #ffffff;
  font-size: 11px;
  font-weight: 500;
  padding: 4px 8px;
  border-radius: 4px;
}

.badge-ps5 {
  border: 1px solid #0070d1;
}

.badge-ps4 {
  border: 1px solid #003791;
}
```

### Trophy Components

#### Trophy Card
```css
.trophy-card {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #1f1f1f;
  border-radius: 8px;
}

.trophy-icon {
  width: 48px;
  height: 48px;
  flex-shrink: 0;
}

.trophy-icon-platinum {
  filter: drop-shadow(0 0 8px rgba(123, 159, 204, 0.6));
}

.trophy-icon-gold {
  filter: drop-shadow(0 0 8px rgba(205, 154, 26, 0.6));
}

.trophy-icon-silver {
  filter: drop-shadow(0 0 6px rgba(168, 168, 168, 0.4));
}

.trophy-icon-bronze {
  filter: drop-shadow(0 0 6px rgba(205, 127, 50, 0.4));
}

.trophy-info {
  flex: 1;
}

.trophy-name {
  font-size: 16px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 4px;
}

.trophy-description {
  font-size: 13px;
  color: #b3b3b3;
}

.trophy-rarity {
  font-size: 12px;
  color: #808080;
  margin-top: 4px;
}
```

#### Trophy Progress Bar
```css
.trophy-progress {
  background: #383838;
  border-radius: 4px;
  height: 8px;
  overflow: hidden;
}

.trophy-progress-fill {
  height: 100%;
  background: linear-gradient(90deg, #003791 0%, #0070d1 100%);
  border-radius: 4px;
  transition: width 500ms ease;
}

.trophy-summary {
  display: flex;
  gap: 16px;
  margin-top: 12px;
}

.trophy-count {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
}
```

### Navigation

#### Top Navigation Bar
```css
.nav-top {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 64px;
  background: rgba(0, 0, 0, 0.95);
  backdrop-filter: blur(20px);
  display: flex;
  align-items: center;
  padding: 0 24px;
  z-index: 1000;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.nav-logo {
  height: 32px;
  margin-right: 32px;
}

.nav-item {
  font-size: 14px;
  font-weight: 500;
  color: #b3b3b3;
  padding: 8px 16px;
  border-radius: 4px;
  transition: all 200ms ease;
}

.nav-item:hover {
  color: #ffffff;
  background: rgba(255, 255, 255, 0.1);
}

.nav-item.active {
  color: #ffffff;
}

.nav-item.active::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 0;
  right: 0;
  height: 2px;
  background: #0070d1;
}
```

#### Side Navigation (Console Style)
```css
.nav-side {
  width: 80px;
  background: #0a0a0a;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 16px 0;
  gap: 8px;
}

.nav-side-item {
  width: 56px;
  height: 56px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #808080;
  transition: all 200ms ease;
}

.nav-side-item:hover {
  color: #ffffff;
  background: rgba(255, 255, 255, 0.1);
}

.nav-side-item.active {
  color: #ffffff;
  background: #0070d1;
}
```

### Inputs

#### Search Input
```css
.input-search {
  background: #2d2d2d;
  border: 1px solid transparent;
  border-radius: 24px;
  color: #ffffff;
  font-size: 14px;
  padding: 12px 16px 12px 44px;
  width: 100%;
  transition: all 200ms ease;
}

.input-search:focus {
  outline: none;
  border-color: #0070d1;
  background: #383838;
}

.input-search::placeholder {
  color: #808080;
}

.input-search-icon {
  position: absolute;
  left: 16px;
  top: 50%;
  transform: translateY(-50%);
  color: #808080;
}
```

#### Text Input
```css
.input-text {
  background: #1f1f1f;
  border: 1px solid #383838;
  border-radius: 4px;
  color: #ffffff;
  font-size: 16px;
  padding: 14px 16px;
  width: 100%;
  transition: border-color 200ms ease;
}

.input-text:focus {
  outline: none;
  border-color: #0070d1;
}

.input-text:invalid {
  border-color: #ff4444;
}

.input-label {
  font-size: 14px;
  font-weight: 500;
  color: #b3b3b3;
  margin-bottom: 8px;
  display: block;
}
```

### Modals

```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.85);
  backdrop-filter: blur(8px);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 2000;
}

.modal {
  background: #1f1f1f;
  border-radius: 12px;
  max-width: 480px;
  width: 90%;
  max-height: 90vh;
  overflow: hidden;
  box-shadow: 0 24px 64px rgba(0, 0, 0, 0.5);
}

.modal-header {
  padding: 20px 24px;
  border-bottom: 1px solid #383838;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.modal-title {
  font-size: 20px;
  font-weight: 600;
  color: #ffffff;
}

.modal-close {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background: transparent;
  border: none;
  color: #808080;
  cursor: pointer;
  transition: all 200ms ease;
}

.modal-close:hover {
  background: rgba(255, 255, 255, 0.1);
  color: #ffffff;
}

.modal-body {
  padding: 24px;
}

.modal-footer {
  padding: 16px 24px;
  border-top: 1px solid #383838;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
}
```

### Download Progress

```css
.download-item {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #1f1f1f;
  border-radius: 8px;
}

.download-image {
  width: 64px;
  height: 64px;
  border-radius: 4px;
  object-fit: cover;
}

.download-info {
  flex: 1;
}

.download-title {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 4px;
}

.download-status {
  font-size: 13px;
  color: #b3b3b3;
  margin-bottom: 8px;
}

.download-progress-bar {
  height: 4px;
  background: #383838;
  border-radius: 2px;
  overflow: hidden;
}

.download-progress-fill {
  height: 100%;
  background: #0070d1;
  border-radius: 2px;
  transition: width 200ms linear;
}

.download-percent {
  font-size: 14px;
  font-weight: 600;
  color: #0070d1;
  min-width: 48px;
  text-align: right;
}
```

### User Profile

```css
.profile-card {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #1f1f1f;
  border-radius: 12px;
}

.profile-avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  border: 2px solid #0070d1;
}

.profile-name {
  font-size: 18px;
  font-weight: 600;
  color: #ffffff;
}

.profile-psn-id {
  font-size: 14px;
  color: #808080;
}

.profile-level {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-top: 8px;
}

.profile-level-badge {
  background: linear-gradient(135deg, #003791 0%, #0070d1 100%);
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 4px 12px;
  border-radius: 12px;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-2` | 2px | Tight gaps, inline elements |
| `--spacing-4` | 4px | Icon padding, compact gaps |
| `--spacing-8` | 8px | Standard small gaps |
| `--spacing-12` | 12px | Card internal padding |
| `--spacing-16` | 16px | Standard gaps, list items |
| `--spacing-24` | 24px | Section gaps, card padding |
| `--spacing-32` | 32px | Large section breaks |
| `--spacing-48` | 48px | Major section separation |
| `--spacing-64` | 64px | Hero spacing, page sections |

### Core Layout Structure

```
┌─────────────────────────────────────────────────────────────┐
│                    Navigation Bar (64px)                     │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│     ┌─────────────────────────────────────────────────┐     │
│     │              Hero/Featured Content               │     │
│     │              (Full width, 16:9)                  │     │
│     └─────────────────────────────────────────────────┘     │
│                                                              │
│     Section Title                                            │
│     ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐       │
│     │Game│ │Game│ │Game│ │Game│ │Game│ │Game│ │Game│ ←→    │
│     └────┘ └────┘ └────┘ └────┘ └────┘ └────┘ └────┘       │
│                                                              │
│     Section Title                                            │
│     ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐ ┌────┐              │
│     │Card│ │Card│ │Card│ │Card│ │Card│ │Card│ ←→           │
│     └────┘ └────┘ └────┘ └────┘ └────┘ └────┘              │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

### Store Layout Grid

```
┌─────────────────────────────────────────────────────────────┐
│ Sidebar       │                Content Area                  │
│ (240px)       │                                              │
│               │  ┌──────────────────────────────────────┐   │
│ Categories    │  │         Game Detail Header            │   │
│ ─────────     │  │         Hero Image (16:9)             │   │
│ ○ All Games   │  └──────────────────────────────────────┘   │
│ ○ New         │                                              │
│ ○ Deals       │  ┌─────────────────┐ ┌──────────────────┐   │
│ ○ PS Plus     │  │                 │ │   Game Info       │   │
│               │  │   Screenshots    │ │   Price: $59.99   │   │
│ Filters       │  │   Gallery        │ │   [Add to Cart]   │   │
│ ─────────     │  │                 │ │   [Wishlist]      │   │
│ Platform      │  └─────────────────┘ └──────────────────┘   │
│ Genre         │                                              │
│ Price         │  Description                                 │
│               │  ─────────────                              │
│               │  Lorem ipsum dolor sit amet...              │
│               │                                              │
└───────────────┴─────────────────────────────────────────────┘
```

### Grid System

| Name | Columns | Gap | Max Width | Usage |
|------|---------|-----|-----------|-------|
| Store Grid | 5-6 | 16px | 1440px | Game browse pages |
| Featured | 3 | 24px | 1440px | Featured sections |
| Detail | 2 (60/40) | 32px | 1200px | Product pages |
| List | 1 | 8px | 800px | Settings, downloads |

### Content Width

| Context | Max Width | Center |
|---------|-----------|--------|
| Full bleed hero | 100% | No |
| Content container | 1440px | Yes |
| Text content | 720px | Yes |
| Modal content | 480px | Yes |
| Narrow forms | 400px | Yes |

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Base surfaces, cards at rest |
| Level 1 | `0 2px 8px rgba(0, 0, 0, 0.3)` | Buttons, subtle lift |
| Level 2 | `0 8px 24px rgba(0, 0, 0, 0.4)` | Hovered cards, dropdowns |
| Level 3 | `0 16px 48px rgba(0, 0, 0, 0.5)` | Modals, dialogs |
| Level 4 | `0 24px 64px rgba(0, 0, 0, 0.6)` | Overlays, full-screen panels |

### Glow Effects

| Type | Effect | Usage |
|------|--------|-------|
| Blue Glow | `0 0 24px rgba(0, 112, 209, 0.4)` | Selected items, focus states |
| Trophy Glow | `0 0 16px rgba(205, 154, 26, 0.5)` | Trophy unlocked animations |
| Active Glow | `0 0 32px rgba(0, 191, 255, 0.3)` | Active/playing states |

### Surface Hierarchy

```
┌─────────────────────────────────────────────────────────┐
│ Overlays & Modals                    #1f1f1f + blur     │
├─────────────────────────────────────────────────────────┤
│ Elevated (Dropdowns, Popovers)       #383838            │
├─────────────────────────────────────────────────────────┤
│ Cards & Panels                       #1f1f1f            │
├─────────────────────────────────────────────────────────┤
│ Primary Background                   #000000            │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Content, cards |
| Sticky | 100 | Navigation, fixed headers |
| Dropdown | 200 | Menus, autocomplete |
| Overlay | 300 | Game card hover expansion |
| Modal | 400 | Dialogs, purchase confirmations |
| Toast | 500 | Notifications, trophy popups |
| System | 1000 | Controller prompts, critical alerts |

### Blur Effects

```css
.backdrop-blur {
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
}

.nav-blur {
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(20px) saturate(180%);
}

.modal-blur {
  backdrop-filter: blur(8px);
}
```

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use PlayStation Blue (#003791, #0070d1) as primary accent | Brand recognition, trust |
| Maintain pure black backgrounds (#000000) | OLED optimization, cinematic feel |
| Showcase game art prominently | Games are the hero content |
| Use smooth, cinematic animations (300-500ms) | Premium, console-like feel |
| Display trophy counts and progress | Achievement engagement |
| Show PS Plus benefits prominently | Subscription value |
| Use rounded corners (8-12px) | Modern, friendly aesthetic |
| Provide controller button prompts | Console-first experience |
| Include platform badges (PS5/PS4) | Compatibility clarity |
| Use gradient overlays on images | Text readability |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Don't use light backgrounds as default | Breaks immersion, off-brand |
| Avoid sharp corners (0px radius) | Feels dated, not PlayStation |
| Don't hide prices or purchase CTAs | Users expect clear commerce |
| Avoid small game artwork | Art sells games, needs prominence |
| Don't use generic blue (#0000ff) | Must use PlayStation Blue specifically |
| Avoid slow, heavy animations (>500ms) | Feels sluggish on console |
| Don't forget platform compatibility | PS5/PS4 distinction is crucial |
| Avoid cluttered trophy displays | Trophy prestige requires clean presentation |
| Don't mix PS Plus yellow with other yellows | Brand consistency |
| Avoid hiding online status | Social features are core to PSN |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use official game titles | Abbreviate or modify game names |
| Show accurate prices with regional currency | Display incorrect pricing |
| Indicate free PS Plus games clearly | Hide subscription requirements |
| Display game ratings (ESRB/PEGI) | Omit content ratings |
| Use "Add to Cart" / "Buy Now" | Vague purchase language |
| Show download size clearly | Hide storage requirements |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| 4K TV | >2560px | Scaled UI, larger text, full grid |
| TV/Desktop Large | 1920px - 2559px | Standard console UI |
| Desktop | 1280px - 1919px | Full layout, 5-column grid |
| Tablet | 768px - 1279px | 3-4 column grid, collapsible sidebar |
| Mobile | <768px | Single column, bottom navigation |

### Device-Specific Adaptations

| Component | Console/TV | Desktop | Mobile |
|-----------|------------|---------|--------|
| Navigation | D-pad focus, side rail | Top bar, mouse hover | Bottom tabs |
| Game Cards | Large (200px+), focus highlight | Medium (150-200px), hover | Full-width list |
| Buttons | Large (56px height), glow focus | Standard (44px), hover | Touch-optimized (48px) |
| Typography | Larger scale (+25%) | Standard | Compact |
| Spacing | Generous | Standard | Tighter |

### Console Controller Navigation

```css
/* Focus states for controller navigation */
.focusable:focus {
  outline: 3px solid #0070d1;
  outline-offset: 4px;
  box-shadow: 0 0 24px rgba(0, 112, 209, 0.5);
}

.game-card:focus {
  transform: scale(1.1);
  z-index: 100;
}

/* D-pad navigation grid */
.grid-navigable {
  display: grid;
  gap: 16px;
}

.grid-navigable:focus-within {
  scroll-padding: 24px;
}
```

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Buttons | 44px × 44px | iOS/Android standards |
| Game Cards | Full card area | Entire card is tappable |
| List Items | 48px height | Comfortable thumb reach |
| Close buttons | 44px × 44px | Easy dismissal |
| Navigation items | 48px × 48px | Bottom tab bar |

### Mobile Navigation

```css
.mobile-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 64px;
  background: #0a0a0a;
  border-top: 1px solid #2d2d2d;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-bottom: env(safe-area-inset-bottom);
}

.mobile-nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  color: #808080;
  font-size: 10px;
}

.mobile-nav-item.active {
  color: #0070d1;
}
```

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Brand Colors
PlayStation Blue Primary: #003791
PlayStation Blue Light: #0070d1
PlayStation Blue Bright: #00bfff
White: #ffffff

# Backgrounds
Primary (Black): #000000
Secondary (Dark Gray): #1f1f1f
Tertiary: #2d2d2d
Elevated: #383838

# PS Plus
PS Plus Yellow: #ffb800
PS Plus Gold: #d4af37

# Trophy Colors
Platinum: #7b9fcc
Gold: #cd9a1a
Silver: #a8a8a8
Bronze: #cd7f32

# Text
Primary: #ffffff
Secondary: #b3b3b3
Tertiary: #808080
Link: #0070d1

# Radii
Small: 4px
Medium: 8px
Large: 12px
Round: 22px (pill buttons)
Circle: 50%

# Fonts
Primary: 'SST', 'Sony SST', system-ui, sans-serif
Weights: 400 (body), 500 (UI), 600 (headers), 700 (titles)

# Shadows
Hover: 0 8px 32px rgba(0, 112, 209, 0.3)
Modal: 0 24px 64px rgba(0, 0, 0, 0.5)
Glow: 0 0 24px rgba(0, 112, 209, 0.4)
```

### Example Prompts

#### Game Store Card
```
Create a game card for the PlayStation Store:
- Card: #1f1f1f background, 8px border-radius
- Image: Square (1:1) game box art, fills top of card
- Content padding: 12px
- Title: 14px semibold white, single line with ellipsis
- Platform: 12px #808080, "PS5" with blue border badge
- Price: 16px bold white, align bottom
- Sale price: Yellow #ffb800 with strikethrough original
- Hover: scale(1.05), blue glow shadow
- PS Plus badge if applicable: Yellow gradient, uppercase
```

#### Trophy Notification
```
Design a trophy unlock notification popup:
- Container: #1f1f1f, 12px radius, slide in from right
- Width: 320px
- Trophy icon: 48px with type-specific glow effect
- Trophy type: Platinum/Gold/Silver/Bronze
- Title: 16px semibold white
- Description: 13px #b3b3b3
- Game name: 12px #808080
- Rarity: "Ultra Rare 2.5%" in #0070d1
- Animation: Shimmer effect on platinum/gold
- Sound: Trophy unlock chime (reference only)
```

#### User Profile Header
```
Create a PSN user profile header:
- Banner: Full width, gradient overlay at bottom
- Avatar: 96px circle with 3px #0070d1 border
- Username: 24px bold white
- PSN ID: 16px #808080
- Trophy level: Blue gradient badge with level number
- Trophy summary: Row of platinum/gold/silver/bronze counts
- Online status: Green dot #00c853 if online
- "Add Friend" button: PS Blue pill button
```

#### PS Plus Subscription Card
```
Design a PS Plus tier comparison card:
- Card: #1f1f1f background, 12px radius
- Header: Yellow-to-orange gradient (#ffb800 to #ff8c00)
- Tier name: "PS Plus Premium" in black, 20px bold
- Price: 24px bold white, "/month" in 14px #b3b3b3
- Features list: Check marks in #00c853
- CTA: "Subscribe" pill button in PS Blue
- Current plan indicator: White outline border
```

#### Download Queue Item
```
Create a download queue item:
- Container: #1f1f1f, 8px radius, flex row
- Game thumbnail: 64px square, 4px radius
- Title: 14px semibold white
- Status: "Downloading..." in 13px #b3b3b3
- Progress bar: 4px height, #383838 track, #0070d1 fill
- Percentage: 14px semibold #0070d1
- Actions: Pause/Cancel icon buttons
- Estimated time: 12px #808080
```

### CSS Variables Template

```css
:root {
  /* Brand Colors */
  --ps-blue-primary: #003791;
  --ps-blue-light: #0070d1;
  --ps-blue-bright: #00bfff;
  
  /* Backgrounds */
  --background-primary: #000000;
  --background-secondary: #1f1f1f;
  --background-tertiary: #2d2d2d;
  --background-elevated: #383838;
  
  /* PS Plus */
  --ps-plus-yellow: #ffb800;
  --ps-plus-gold: #d4af37;
  
  /* Trophy */
  --trophy-platinum: #7b9fcc;
  --trophy-gold: #cd9a1a;
  --trophy-silver: #a8a8a8;
  --trophy-bronze: #cd7f32;
  
  /* Text */
  --text-primary: #ffffff;
  --text-secondary: #b3b3b3;
  --text-tertiary: #808080;
  --text-link: #0070d1;
  
  /* Semantic */
  --success: #00c853;
  --warning: #ffb800;
  --error: #ff4444;
  
  /* Typography */
  --font-primary: 'SST', 'Sony SST', -apple-system, BlinkMacSystemFont, sans-serif;
  
  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  
  /* Radii */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-pill: 22px;
  --radius-circle: 50%;
  
  /* Shadows */
  --shadow-sm: 0 2px 8px rgba(0, 0, 0, 0.3);
  --shadow-md: 0 8px 24px rgba(0, 0, 0, 0.4);
  --shadow-lg: 0 16px 48px rgba(0, 0, 0, 0.5);
  --shadow-glow: 0 0 24px rgba(0, 112, 209, 0.4);
  
  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
  --transition-slow: 300ms cubic-bezier(0.4, 0, 0.2, 1);
}
```

### Controller Button Prompts

```css
/* PlayStation controller button icons */
.button-prompt {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 13px;
  color: #b3b3b3;
}

.button-prompt-icon {
  width: 24px;
  height: 24px;
}

/* Button colors */
.btn-cross { color: #5d9bec; }    /* X - Blue */
.btn-circle { color: #ef6d6d; }   /* O - Red */
.btn-square { color: #d98ad1; }   /* Square - Pink */
.btn-triangle { color: #77c785; } /* Triangle - Green */
```

---

## Summary

PlayStation's design system delivers a **premium, immersive gaming experience** through:

1. **Iconic PlayStation Blue** (#003791, #0070d1) as the signature accent color
2. **Pure black backgrounds** (#000000) optimized for OLED displays and cinematic immersion
3. **Game artwork as hero content** with large cards and smooth hover animations
4. **Trophy system integration** with distinct colors for platinum, gold, silver, and bronze
5. **PS Plus branding** using distinctive yellow (#ffb800) gradients
6. **Controller-first design** with focus states, button prompts, and D-pad navigation
7. **SST (Sony Sans Text)** typography for clean, modern readability
8. **Cinematic animations** (300-500ms) creating a premium console feel
9. **Generous spacing** and low-density layouts that let content breathe

When implementing PlayStation-style interfaces, prioritize:
- Dark immersive backgrounds that showcase game artwork
- Smooth, sweeping animations for card interactions
- Clear platform indicators (PS5/PS4)
- Trophy progress and achievements visibility
- PS Plus value proposition in store contexts
- Controller navigation support with visible focus states
