# Xbox Design System

> Microsoft Fluent Design meets gaming. Xbox Green (#107C10), deep dark backgrounds, Segoe UI typography, Game Pass branding, achievement gamerscore, and controller-centric Xbox ecosystem.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Xbox embodies a **modern, connected gaming** design philosophy rooted in Microsoft's Fluent Design System. The interface is bold, accessible, and social—designed around the Xbox ecosystem spanning console, PC, cloud, and mobile. Every element communicates inclusivity, community, and the power of play across devices.

### Mood & Feeling
- **Bold & Energetic**: Signature Xbox Green creates instant brand recognition and energy
- **Connected**: Cross-platform continuity from console to PC to mobile to cloud
- **Social-first**: Friends, parties, clubs, and Looking for Group (LFG) features
- **Achievement-driven**: Gamerscore, achievement hunting, and completion tracking
- **Accessible**: Microsoft's commitment to inclusive gaming built into the design
- **Game Pass forward**: Subscription value prominently showcased throughout

### Design Density
**Medium density** with efficient use of space. Content tiles are substantial but optimized for quick scanning. Navigation is fast with quick access panels. The interface balances game discovery with social features and system management.

### Visual Character
- Iconic Xbox Green as the signature accent
- Deep charcoal backgrounds with subtle depth layers
- Game art as primary visual content (hero images, box art, screenshots)
- Fluent Design acrylic blur and reveal effects
- Rounded corners with subtle animations
- Achievement iconography and gamerscore displays
- Controller button prompts as native UI elements
- Gamertag identity system with customizable avatars

---

## 2. Color Palette & Roles

### Primary Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--xbox-green-primary` | `#107C10` | Core Xbox Green, primary actions, branding |
| `--xbox-green-light` | `#0E8A0E` | Hover states, active elements |
| `--xbox-green-bright` | `#10B910` | Highlights, success states, Game Pass |
| `--xbox-green-dark` | `#0A5D0A` | Pressed states, depth |
| `--white` | `#ffffff` | Primary text, icons on dark backgrounds |

### Background Colors

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#0e0e0e` | Main app background, deepest layer |
| `--background-secondary` | `#1f1f1f` | Cards, panels, elevated surfaces |
| `--background-tertiary` | `#2d2d2d` | Hover states, input fields |
| `--background-elevated` | `#3a3a3a` | Modals, dropdowns, popovers |
| `--background-surface` | `#252525` | Content containers, list backgrounds |
| `--background-acrylic` | `rgba(30, 30, 30, 0.85)` | Fluent acrylic blur panels |

### Game Pass & Subscription Colors

| Token | Hex | Role |
|-------|-----|------|
| `--gamepass-green` | `#107C10` | Game Pass Core branding |
| `--gamepass-ultimate` | `#107C10` | Game Pass Ultimate |
| `--gamepass-gradient-start` | `#107C10` | Game Pass gradient |
| `--gamepass-gradient-end` | `#0E8A0E` | Game Pass gradient end |
| `--ea-play` | `#ff4747` | EA Play integration accent |
| `--cloud-gaming` | `#9147ff` | Cloud gaming indicator |

### Achievement & Gamerscore Colors

| Token | Hex | Role |
|-------|-----|------|
| `--achievement-unlocked` | `#107C10` | Unlocked achievement |
| `--achievement-locked` | `#404040` | Locked achievement |
| `--achievement-rare` | `#00b4ff` | Rare achievement |
| `--achievement-secret` | `#7b2cbf` | Secret/hidden achievement |
| `--gamerscore` | `#ffffff` | Gamerscore number display |
| `--completion-fill` | `#107C10` | Completion progress fill |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--text-primary` | `#ffffff` | Primary headings, game titles |
| `--text-secondary` | `#c8c8c8` | Body text, descriptions |
| `--text-tertiary` | `#8a8a8a` | Metadata, timestamps, muted info |
| `--text-link` | `#107C10` | Hyperlinks, interactive text |
| `--text-disabled` | `#5a5a5a` | Disabled states |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--success` | `#107C10` | Success, online, complete |
| `--warning` | `#f7630c` | Warnings, storage alerts |
| `--error` | `#e81123` | Errors, failed operations |
| `--info` | `#0078d4` | Informational messages (Microsoft Blue) |
| `--online` | `#107C10` | Online status |
| `--away` | `#f7630c` | Away status |
| `--busy` | `#e81123` | Do not disturb |
| `--offline` | `#8a8a8a` | Offline status |

### Gradient Definitions

| Name | Definition | Usage |
|------|------------|-------|
| Hero Overlay | `linear-gradient(to top, #0e0e0e 0%, transparent 60%)` | Game hero images |
| Xbox Green Gradient | `linear-gradient(135deg, #107C10 0%, #0E8A0E 100%)` | Featured actions |
| Game Pass Gradient | `linear-gradient(180deg, #107C10 0%, #0A5D0A 100%)` | Game Pass badges |
| Card Hover | `linear-gradient(180deg, transparent 0%, rgba(16, 124, 16, 0.15) 100%)` | Hover effects |
| Acrylic | `linear-gradient(180deg, rgba(255,255,255,0.05) 0%, transparent 100%)` | Fluent acrylic |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary Xbox/Microsoft font */
--font-primary: 'Segoe UI', 'Segoe UI Variable', -apple-system, BlinkMacSystemFont, Roboto, sans-serif;

/* Display variant for headers */
--font-display: 'Segoe UI Display', 'Segoe UI', sans-serif;

/* Semibold variant for emphasis */
--font-semibold: 'Segoe UI Semibold', 'Segoe UI', sans-serif;

/* System fallback */
--font-system: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Title | 48px | 600 | 1.1 | -0.01em | `--text-primary` |
| Page Title | 34px | 600 | 1.2 | -0.01em | `--text-primary` |
| Section Header | 24px | 600 | 1.3 | 0 | `--text-primary` |
| Card Title | 16px | 600 | 1.3 | 0 | `--text-primary` |
| Subsection | 14px | 600 | 1.4 | 0 | `--text-primary` |
| Body Large | 16px | 400 | 1.5 | 0 | `--text-secondary` |
| Body Regular | 14px | 400 | 1.5 | 0 | `--text-secondary` |
| Body Small | 13px | 400 | 1.4 | 0 | `--text-tertiary` |
| Caption | 12px | 400 | 1.4 | 0.01em | `--text-tertiary` |
| Button Text | 14px | 600 | 1 | 0.02em | `--text-primary` |
| Gamerscore | 20px | 700 | 1 | 0 | `--text-primary` |
| Price | 16px | 600 | 1 | 0 | `--text-primary` |
| Badge | 11px | 600 | 1 | 0.03em | `--text-primary` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 300 | Light | Large display text, marketing |
| 400 | Regular | Body text, descriptions |
| 600 | Semibold | Headers, titles, buttons, emphasis |
| 700 | Bold | Gamerscore, prices, key numbers |

### Marketing Typography

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Campaign Hero | 64px | 600 | Major launches, events |
| Event Title | 48px | 600 | Xbox showcases, reveals |
| Feature Headline | 36px | 600 | Feature section headers |
| Tagline | 20px | 400 | Supporting copy |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Xbox Green)
```css
.button-primary {
  background: #107C10;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 10px 24px;
  min-height: 40px;
  border-radius: 4px;
  border: none;
  text-transform: none;
  transition: all 150ms ease;
}

.button-primary:hover {
  background: #0E8A0E;
}

.button-primary:active {
  background: #0A5D0A;
  transform: scale(0.98);
}

.button-primary:focus {
  outline: 2px solid #ffffff;
  outline-offset: 2px;
}

.button-primary:disabled {
  background: #404040;
  color: #8a8a8a;
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
  padding: 10px 24px;
  min-height: 40px;
  border-radius: 4px;
  border: 2px solid #8a8a8a;
  transition: all 150ms ease;
}

.button-secondary:hover {
  border-color: #ffffff;
  background: rgba(255, 255, 255, 0.1);
}

.button-secondary:active {
  background: rgba(255, 255, 255, 0.15);
}
```

#### Game Pass Button
```css
.button-gamepass {
  background: linear-gradient(180deg, #107C10 0%, #0A5D0A 100%);
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 12px 28px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.button-gamepass:hover {
  background: linear-gradient(180deg, #0E8A0E 0%, #107C10 100%);
}

.button-gamepass-icon {
  width: 20px;
  height: 20px;
}
```

#### Icon Button
```css
.button-icon {
  width: 40px;
  height: 40px;
  border-radius: 4px;
  background: rgba(255, 255, 255, 0.1);
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #ffffff;
  transition: all 150ms ease;
}

.button-icon:hover {
  background: rgba(255, 255, 255, 0.15);
}

.button-icon:focus {
  outline: 2px solid #ffffff;
  outline-offset: 2px;
}
```

### Game Cards

#### Standard Game Tile
```css
.game-tile {
  background: #1f1f1f;
  border-radius: 8px;
  overflow: hidden;
  transition: all 200ms ease;
  cursor: pointer;
  position: relative;
}

.game-tile:hover {
  transform: scale(1.03);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.4);
  z-index: 10;
}

.game-tile:focus {
  outline: 3px solid #ffffff;
  outline-offset: 2px;
}

.game-tile-image {
  width: 100%;
  aspect-ratio: 2 / 3; /* Vertical box art */
  object-fit: cover;
}

.game-tile-content {
  padding: 12px;
}

.game-tile-title {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 4px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.game-tile-publisher {
  font-size: 12px;
  color: #8a8a8a;
}

.game-tile-price {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-top: 8px;
}

.game-tile-gamepass {
  position: absolute;
  top: 8px;
  left: 8px;
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
  padding: 32px;
  background: linear-gradient(to top, rgba(14, 14, 14, 0.95) 0%, transparent 100%);
}

.game-card-featured-title {
  font-size: 32px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 8px;
}

.game-card-featured-meta {
  font-size: 14px;
  color: #c8c8c8;
}

.game-card-featured-cta {
  margin-top: 16px;
  display: flex;
  gap: 12px;
}
```

### Badges & Tags

#### Game Pass Badge
```css
.badge-gamepass {
  background: #107C10;
  color: #ffffff;
  font-size: 11px;
  font-weight: 600;
  padding: 4px 8px;
  border-radius: 2px;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.badge-gamepass-ultimate {
  background: linear-gradient(135deg, #107C10 0%, #0E8A0E 100%);
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
  border-radius: 2px;
}

.badge-xbox-series {
  background: #1f1f1f;
  border: 1px solid #107C10;
}

.badge-xbox-one {
  background: #1f1f1f;
  border: 1px solid #8a8a8a;
}

.badge-pc {
  background: #1f1f1f;
  border: 1px solid #0078d4;
}

.badge-cloud {
  background: #1f1f1f;
  border: 1px solid #9147ff;
}
```

#### Smart Delivery Badge
```css
.badge-smart-delivery {
  background: transparent;
  border: 1px solid #107C10;
  color: #107C10;
  font-size: 10px;
  font-weight: 600;
  padding: 3px 6px;
  border-radius: 2px;
  text-transform: uppercase;
}
```

### Achievement Components

#### Achievement Card
```css
.achievement-card {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #1f1f1f;
  border-radius: 8px;
  transition: background 150ms ease;
}

.achievement-card:hover {
  background: #252525;
}

.achievement-icon {
  width: 64px;
  height: 64px;
  border-radius: 4px;
  flex-shrink: 0;
}

.achievement-icon-locked {
  filter: grayscale(100%) brightness(0.4);
}

.achievement-icon-rare {
  box-shadow: 0 0 12px rgba(0, 180, 255, 0.5);
}

.achievement-info {
  flex: 1;
}

.achievement-name {
  font-size: 15px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 4px;
}

.achievement-description {
  font-size: 13px;
  color: #c8c8c8;
  margin-bottom: 4px;
}

.achievement-gamerscore {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  font-weight: 600;
  color: #ffffff;
}

.achievement-gamerscore-icon {
  width: 16px;
  height: 16px;
  color: #107C10;
}

.achievement-rarity {
  font-size: 12px;
  color: #00b4ff;
}
```

#### Gamerscore Display
```css
.gamerscore-display {
  display: flex;
  align-items: center;
  gap: 8px;
}

.gamerscore-icon {
  width: 24px;
  height: 24px;
  color: #107C10;
}

.gamerscore-value {
  font-size: 20px;
  font-weight: 700;
  color: #ffffff;
}

.gamerscore-label {
  font-size: 12px;
  color: #8a8a8a;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

#### Achievement Progress
```css
.achievement-progress {
  background: #404040;
  border-radius: 2px;
  height: 4px;
  overflow: hidden;
}

.achievement-progress-fill {
  height: 100%;
  background: #107C10;
  border-radius: 2px;
  transition: width 300ms ease;
}

.achievement-stats {
  display: flex;
  justify-content: space-between;
  margin-top: 8px;
  font-size: 13px;
  color: #c8c8c8;
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
  height: 56px;
  background: rgba(14, 14, 14, 0.95);
  backdrop-filter: blur(20px);
  display: flex;
  align-items: center;
  padding: 0 24px;
  z-index: 1000;
}

.nav-logo {
  height: 24px;
  margin-right: 32px;
}

.nav-item {
  font-size: 14px;
  font-weight: 500;
  color: #c8c8c8;
  padding: 8px 16px;
  border-radius: 4px;
  transition: all 150ms ease;
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
  bottom: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: #107C10;
}
```

#### Guide Menu (Side Panel)
```css
.guide-panel {
  position: fixed;
  left: 0;
  top: 0;
  bottom: 0;
  width: 400px;
  background: rgba(30, 30, 30, 0.95);
  backdrop-filter: blur(40px);
  transform: translateX(-100%);
  transition: transform 200ms ease;
  z-index: 2000;
  display: flex;
  flex-direction: column;
}

.guide-panel.open {
  transform: translateX(0);
}

.guide-header {
  padding: 16px 24px;
  border-bottom: 1px solid #404040;
  display: flex;
  align-items: center;
  gap: 16px;
}

.guide-tabs {
  display: flex;
  gap: 4px;
  padding: 0 16px;
  border-bottom: 1px solid #404040;
}

.guide-tab {
  padding: 12px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #8a8a8a;
  border-bottom: 2px solid transparent;
  transition: all 150ms ease;
}

.guide-tab:hover {
  color: #ffffff;
}

.guide-tab.active {
  color: #ffffff;
  border-bottom-color: #107C10;
}

.guide-content {
  flex: 1;
  overflow-y: auto;
  padding: 16px;
}
```

### Inputs

#### Search Input
```css
.input-search {
  background: #2d2d2d;
  border: 2px solid transparent;
  border-radius: 4px;
  color: #ffffff;
  font-size: 14px;
  padding: 10px 12px 10px 40px;
  width: 100%;
  transition: all 150ms ease;
}

.input-search:focus {
  outline: none;
  border-color: #107C10;
  background: #1f1f1f;
}

.input-search::placeholder {
  color: #8a8a8a;
}

.input-search-icon {
  position: absolute;
  left: 12px;
  top: 50%;
  transform: translateY(-50%);
  color: #8a8a8a;
  width: 20px;
  height: 20px;
}
```

#### Text Input
```css
.input-text {
  background: #1f1f1f;
  border: 2px solid #404040;
  border-radius: 4px;
  color: #ffffff;
  font-size: 14px;
  padding: 12px 14px;
  width: 100%;
  transition: border-color 150ms ease;
}

.input-text:focus {
  outline: none;
  border-color: #107C10;
}

.input-text:invalid {
  border-color: #e81123;
}

.input-label {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 8px;
  display: block;
}
```

### Modals

```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(4px);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 3000;
}

.modal {
  background: #1f1f1f;
  border-radius: 8px;
  max-width: 500px;
  width: 90%;
  max-height: 90vh;
  overflow: hidden;
  box-shadow: 0 16px 48px rgba(0, 0, 0, 0.5);
}

.modal-header {
  padding: 20px 24px;
  border-bottom: 1px solid #404040;
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
  width: 36px;
  height: 36px;
  border-radius: 4px;
  background: transparent;
  border: none;
  color: #8a8a8a;
  cursor: pointer;
  transition: all 150ms ease;
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
  border-top: 1px solid #404040;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
}
```

### Gamertag Profile Card

```css
.gamertag-card {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background: #1f1f1f;
  border-radius: 8px;
}

.gamertag-avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  border: 2px solid #107C10;
}

.gamertag-info {
  flex: 1;
}

.gamertag-name {
  font-size: 18px;
  font-weight: 600;
  color: #ffffff;
  display: flex;
  align-items: center;
  gap: 8px;
}

.gamertag-status {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #107C10;
}

.gamertag-status.away {
  background: #f7630c;
}

.gamertag-status.offline {
  background: #8a8a8a;
}

.gamertag-presence {
  font-size: 13px;
  color: #c8c8c8;
  margin-top: 4px;
}

.gamertag-gamerscore {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
  margin-top: 8px;
}
```

### Activity Feed Item

```css
.activity-item {
  display: flex;
  gap: 12px;
  padding: 16px;
  border-bottom: 1px solid #2d2d2d;
}

.activity-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  flex-shrink: 0;
}

.activity-content {
  flex: 1;
}

.activity-text {
  font-size: 14px;
  color: #ffffff;
}

.activity-text strong {
  font-weight: 600;
}

.activity-game {
  color: #107C10;
  font-weight: 500;
}

.activity-timestamp {
  font-size: 12px;
  color: #8a8a8a;
  margin-top: 4px;
}

.activity-media {
  margin-top: 12px;
  border-radius: 8px;
  overflow: hidden;
}

.activity-media img {
  width: 100%;
  max-height: 300px;
  object-fit: cover;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-2` | 2px | Tight gaps, borders |
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
┌──────────────────────────────────────────────────────────────┐
│                   Navigation Bar (56px)                       │
├──────────────────────────────────────────────────────────────┤
│                                                               │
│    ┌──────────────────────────────────────────────────┐      │
│    │              Hero/Featured Content                │      │
│    │              (Full width, 16:9)                   │      │
│    └──────────────────────────────────────────────────┘      │
│                                                               │
│    Game Pass                                                  │
│    ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐  │
│    │Game │ │Game │ │Game │ │Game │ │Game │ │Game │ │Game │ ←→│
│    └─────┘ └─────┘ └─────┘ └─────┘ └─────┘ └─────┘ └─────┘  │
│                                                               │
│    Recently Played                                            │
│    ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐          │
│    │Tile │ │Tile │ │Tile │ │Tile │ │Tile │ │Tile │ ←→        │
│    └─────┘ └─────┘ └─────┘ └─────┘ └─────┘ └─────┘          │
│                                                               │
│    Friends Activity                                           │
│    ├────────────────────────────────────────────────────┤    │
│    │ Avatar │ Gamertag unlocked Achievement in Game     │    │
│    ├────────────────────────────────────────────────────┤    │
│                                                               │
└──────────────────────────────────────────────────────────────┘
```

### Store Layout Grid

```
┌──────────────────────────────────────────────────────────────┐
│ Filters      │                  Content Area                  │
│ (280px)      │                                                │
│              │  ┌───────────────────────────────────────┐    │
│ Categories   │  │          Game Detail Header            │    │
│ ──────────   │  │          Hero Image (16:9)             │    │
│ ○ All Games  │  └───────────────────────────────────────┘    │
│ ○ Game Pass  │                                                │
│ ○ New        │  ┌──────────────────┐ ┌───────────────────┐   │
│ ○ Sales      │  │                  │ │    Game Info       │   │
│              │  │   Screenshots    │ │    $59.99          │   │
│ Filters      │  │   Gallery        │ │    [Buy Now]       │   │
│ ──────────   │  │                  │ │    [Add to List]   │   │
│ Platform     │  └──────────────────┘ └───────────────────┘   │
│ Genre        │                                                │
│ Price        │  Description                                   │
│ Rating       │  ──────────────                               │
│              │  Lorem ipsum dolor sit amet...                │
│              │                                                │
└──────────────┴───────────────────────────────────────────────┘
```

### Grid System

| Name | Columns | Gap | Max Width | Usage |
|------|---------|-----|-----------|-------|
| Store Grid | 5-7 | 16px | 1600px | Game browse pages |
| Featured | 3-4 | 24px | 1600px | Featured sections |
| Detail | 2 (65/35) | 32px | 1400px | Product pages |
| List | 1 | 8px | 800px | Settings, downloads |

### Content Width

| Context | Max Width | Center |
|---------|-----------|--------|
| Full bleed hero | 100% | No |
| Content container | 1600px | Yes |
| Text content | 800px | Yes |
| Modal content | 500px | Yes |
| Narrow forms | 420px | Yes |

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Base surfaces |
| Level 1 | `0 2px 4px rgba(0, 0, 0, 0.2)` | Buttons, subtle lift |
| Level 2 | `0 4px 16px rgba(0, 0, 0, 0.3)` | Cards, dropdowns |
| Level 3 | `0 8px 24px rgba(0, 0, 0, 0.4)` | Hovered cards |
| Level 4 | `0 16px 48px rgba(0, 0, 0, 0.5)` | Modals, dialogs |

### Focus & Glow Effects

| Type | Effect | Usage |
|------|--------|-------|
| Focus Ring | `outline: 2px solid #ffffff` | Keyboard focus |
| Green Glow | `0 0 16px rgba(16, 124, 16, 0.4)` | Selected items, CTA |
| Achievement Glow | `0 0 12px rgba(0, 180, 255, 0.5)` | Rare achievements |
| Active Game | `0 0 20px rgba(16, 124, 16, 0.3)` | Currently playing |

### Surface Hierarchy

```
┌───────────────────────────────────────────────────────────┐
│ Overlays & Modals                    #1f1f1f + blur       │
├───────────────────────────────────────────────────────────┤
│ Elevated (Guide, Dropdowns)          #3a3a3a              │
├───────────────────────────────────────────────────────────┤
│ Cards & Panels                       #1f1f1f              │
├───────────────────────────────────────────────────────────┤
│ Surface                              #252525              │
├───────────────────────────────────────────────────────────┤
│ Primary Background                   #0e0e0e              │
└───────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Content, cards |
| Sticky | 100 | Navigation, fixed headers |
| Dropdown | 200 | Menus, autocomplete |
| Overlay | 300 | Game tile expansion |
| Guide | 400 | Guide panel |
| Modal | 500 | Dialogs, purchases |
| Toast | 600 | Notifications, achievements |
| System | 1000 | Controller prompts |

### Fluent Design Effects

```css
/* Acrylic blur effect */
.acrylic {
  background: rgba(30, 30, 30, 0.85);
  backdrop-filter: blur(40px) saturate(125%);
  -webkit-backdrop-filter: blur(40px) saturate(125%);
}

/* Reveal highlight (on hover) */
.reveal-highlight {
  position: relative;
  overflow: hidden;
}

.reveal-highlight::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    circle at var(--mouse-x, 50%) var(--mouse-y, 50%),
    rgba(255, 255, 255, 0.1) 0%,
    transparent 50%
  );
  opacity: 0;
  transition: opacity 150ms ease;
}

.reveal-highlight:hover::before {
  opacity: 1;
}

/* Reveal border */
.reveal-border {
  position: relative;
}

.reveal-border::after {
  content: '';
  position: absolute;
  inset: 0;
  border: 1px solid transparent;
  border-image: radial-gradient(
    circle at var(--mouse-x, 50%) var(--mouse-y, 50%),
    rgba(255, 255, 255, 0.3) 0%,
    transparent 50%
  ) 1;
}
```

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use Xbox Green (#107C10) as primary accent | Brand recognition, Xbox identity |
| Maintain dark backgrounds (#0e0e0e, #1f1f1f) | Console-optimized, reduces eye strain |
| Showcase Game Pass value prominently | Key subscription driver |
| Display gamerscore and achievements | Core Xbox engagement mechanic |
| Use white focus rings for accessibility | High contrast, controller navigation |
| Show platform badges (Series X|S, One, PC, Cloud) | Cross-platform clarity |
| Implement Fluent Design principles | Microsoft ecosystem consistency |
| Use Segoe UI font family | Microsoft/Xbox brand typography |
| Provide controller button prompts | Console-first experience |
| Show friends' online status | Social gaming is core to Xbox |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Don't use light backgrounds as default | Off-brand, breaks console experience |
| Avoid colors other than Xbox Green for CTAs | Brand consistency, recognition |
| Don't hide gamerscore/achievements | Achievements are core to Xbox culture |
| Avoid tiny game tiles | Art sells games, needs visibility |
| Don't use rounded pill buttons | Xbox uses subtle 4px radius |
| Avoid heavy animations (>200ms) | Feels sluggish, Xbox is snappy |
| Don't forget Smart Delivery badges | Key Xbox feature communication |
| Avoid hiding Game Pass availability | Subscription value must be clear |
| Don't use PlayStation-style glows | Distinct console identities |
| Avoid cluttered interfaces | Xbox prioritizes clean, scannable layouts |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use official game titles | Abbreviate game names |
| Show accurate regional pricing | Display wrong currency |
| Indicate Game Pass inclusion | Hide subscription benefits |
| Display ESRB/PEGI ratings | Omit content ratings |
| Use "Buy" / "Get" / "Play" | Vague action language |
| Show download/install size | Hide storage requirements |
| Display achievement count clearly | Make gamerscore hard to find |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| 4K TV | >2560px | Scaled UI (150-200%), larger tiles |
| TV/Desktop Large | 1920px - 2559px | Standard console UI |
| Desktop | 1280px - 1919px | Full layout, 5-6 column grid |
| Tablet | 768px - 1279px | 3-4 column grid, hamburger nav |
| Mobile | <768px | 2 column grid, bottom navigation |

### Device-Specific Adaptations

| Component | Console/TV | Desktop | Mobile |
|-----------|------------|---------|--------|
| Navigation | Guide panel, D-pad | Top bar, mouse | Bottom tabs |
| Game Tiles | Large (180px+), focus | Medium (140px), hover | Grid (2-up) |
| Buttons | Large (48px), focus ring | Standard (40px) | Touch (44px) |
| Typography | Scaled +20-30% | Standard | Compact |
| Spacing | Generous (TV viewing) | Standard | Tighter |

### Controller Navigation

```css
/* Focus states for controller navigation */
.focusable:focus {
  outline: 3px solid #ffffff;
  outline-offset: 2px;
}

/* Game tile focus expansion */
.game-tile:focus {
  transform: scale(1.05);
  z-index: 100;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.4);
}

/* D-pad grid navigation */
.nav-grid {
  display: grid;
  gap: 8px;
}

/* Spatial navigation hints */
[data-nav-up],
[data-nav-down],
[data-nav-left],
[data-nav-right] {
  position: relative;
}
```

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Buttons | 40px × 40px | Xbox standard |
| Game Tiles | Full tile area | Entire card tappable |
| List Items | 48px height | Touch-friendly |
| Close buttons | 44px × 44px | Easy dismissal |
| Nav items | 48px × 48px | Bottom tab bar |

### Mobile Navigation

```css
.mobile-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 56px;
  background: #0e0e0e;
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
  color: #8a8a8a;
  font-size: 10px;
  padding: 8px 16px;
}

.mobile-nav-item.active {
  color: #107C10;
}

.mobile-nav-item-icon {
  width: 24px;
  height: 24px;
}
```

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Brand Colors
Xbox Green Primary: #107C10
Xbox Green Light: #0E8A0E
Xbox Green Bright: #10B910
Xbox Green Dark: #0A5D0A
White: #ffffff

# Backgrounds
Primary (Darkest): #0e0e0e
Secondary (Cards): #1f1f1f
Surface: #252525
Tertiary: #2d2d2d
Elevated: #3a3a3a

# Status Colors
Online/Success: #107C10
Away/Warning: #f7630c
Busy/Error: #e81123
Offline: #8a8a8a
Info (MS Blue): #0078d4
Cloud Gaming: #9147ff

# Text
Primary: #ffffff
Secondary: #c8c8c8
Tertiary: #8a8a8a
Link: #107C10
Disabled: #5a5a5a

# Radii
Small: 2px
Medium: 4px
Large: 8px
XLarge: 12px
Circle: 50%

# Fonts
Primary: 'Segoe UI', system-ui, sans-serif
Weights: 400 (body), 600 (headers/buttons), 700 (numbers)

# Shadows
Hover: 0 8px 24px rgba(0, 0, 0, 0.4)
Modal: 0 16px 48px rgba(0, 0, 0, 0.5)
Focus: outline 3px solid #ffffff
```

### Example Prompts

#### Game Pass Game Tile
```
Create a Game Pass game tile:
- Container: #1f1f1f background, 8px border-radius
- Image: 2:3 vertical box art, fills top
- Game Pass badge: Top-left, green #107C10, "GAME PASS" text
- Content padding: 12px
- Title: 14px semibold white, ellipsis overflow
- Publisher: 12px #8a8a8a
- Platform badges: Small pills showing "Series X|S", "PC", "Cloud"
- Hover: scale(1.03), shadow lift
- Focus: 3px white outline, offset 2px
```

#### Achievement Unlock Notification
```
Design an achievement unlock toast:
- Container: #1f1f1f, 8px radius, slide from bottom-right
- Width: 360px
- Xbox sound icon + "Achievement Unlocked" header
- Achievement image: 64px square, 4px radius
- Title: 15px semibold white
- Description: 13px #c8c8c8
- Gamerscore: "G" icon + value in white, green icon
- Rare indicator: Blue #00b4ff text if <10% unlock rate
- Progress: Show X of Y if tracked
- Animation: Slide in, slight bounce, auto-dismiss 5s
```

#### Gamertag Profile Card
```
Create a Gamertag profile card:
- Card: #1f1f1f background, 8px radius
- Avatar: 64px circle with 2px #107C10 border
- Gamertag: 18px semibold white
- Online status: Green dot if online, orange if away
- Presence text: "Playing Halo Infinite" in #c8c8c8
- Gamerscore: G icon + number, prominent display
- Level/tenure: Xbox tenure icon if applicable
- "Add Friend" / "Message" buttons in row
- Hover: Slight background lighten to #252525
```

#### Game Pass Ultimate Card
```
Design a Game Pass Ultimate subscription card:
- Card: #1f1f1f background, 8px radius
- Header: Green gradient (#107C10 to #0A5D0A)
- Logo: Game Pass logo in white
- Tier: "ULTIMATE" badge
- Price: 24px bold white, "per month" in 14px #c8c8c8
- Features checklist: Green checkmarks
- Including: Xbox Live Gold, EA Play, Cloud Gaming icons
- CTA: "Join Now" green button, full width
- Current member: White outline instead of filled
```

#### Store Game Detail Header
```
Create a store game detail header:
- Hero: 16:9 key art, full width
- Gradient overlay: Fade to #0e0e0e at bottom
- Title: 32px semibold white
- Publisher/Developer: 14px #c8c8c8
- Platform badges: Series X|S (green border), PC (blue border)
- Smart Delivery badge if applicable
- Price area: White or "Included with Game Pass" green
- CTA buttons: "Buy" (green) / "Add to List" (outline)
- ESRB rating badge
```

### CSS Variables Template

```css
:root {
  /* Brand Colors */
  --xbox-green-primary: #107C10;
  --xbox-green-light: #0E8A0E;
  --xbox-green-bright: #10B910;
  --xbox-green-dark: #0A5D0A;
  
  /* Backgrounds */
  --background-primary: #0e0e0e;
  --background-secondary: #1f1f1f;
  --background-surface: #252525;
  --background-tertiary: #2d2d2d;
  --background-elevated: #3a3a3a;
  
  /* Status */
  --status-online: #107C10;
  --status-away: #f7630c;
  --status-busy: #e81123;
  --status-offline: #8a8a8a;
  
  /* Semantic */
  --success: #107C10;
  --warning: #f7630c;
  --error: #e81123;
  --info: #0078d4;
  
  /* Text */
  --text-primary: #ffffff;
  --text-secondary: #c8c8c8;
  --text-tertiary: #8a8a8a;
  --text-link: #107C10;
  --text-disabled: #5a5a5a;
  
  /* Typography */
  --font-primary: 'Segoe UI', 'Segoe UI Variable', -apple-system, sans-serif;
  
  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  
  /* Radii */
  --radius-xs: 2px;
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-circle: 50%;
  
  /* Shadows */
  --shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.2);
  --shadow-md: 0 4px 16px rgba(0, 0, 0, 0.3);
  --shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.4);
  --shadow-xl: 0 16px 48px rgba(0, 0, 0, 0.5);
  
  /* Focus */
  --focus-ring: 3px solid #ffffff;
  --focus-offset: 2px;
  
  /* Transitions */
  --transition-fast: 100ms ease;
  --transition-normal: 150ms ease;
  --transition-slow: 200ms ease;
}
```

### Controller Button Prompts

```css
/* Xbox controller button colors */
.button-prompt {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 13px;
  color: #c8c8c8;
}

.button-prompt-icon {
  width: 24px;
  height: 24px;
}

/* Button face colors */
.btn-a { color: #3ddc84; }     /* A - Green */
.btn-b { color: #ea4335; }     /* B - Red */
.btn-x { color: #4285f4; }     /* X - Blue */
.btn-y { color: #fbbc04; }     /* Y - Yellow */

/* Bumpers/Triggers */
.btn-lb, .btn-rb { color: #ffffff; }
.btn-lt, .btn-rt { color: #ffffff; }

/* System buttons */
.btn-menu { color: #ffffff; }   /* Three lines */
.btn-view { color: #ffffff; }   /* Two squares */
.btn-xbox { color: #107C10; }   /* Xbox button */
```

---

## Summary

Xbox's design system delivers a **connected, cross-platform gaming experience** through:

1. **Iconic Xbox Green** (#107C10) as the signature accent driving brand recognition
2. **Deep charcoal backgrounds** (#0e0e0e, #1f1f1f) optimized for TVs and monitors
3. **Microsoft Fluent Design** integration with acrylic blur and reveal effects
4. **Achievement/Gamerscore system** with visible progress and rare achievement highlights
5. **Game Pass prominence** showcasing subscription value throughout the UI
6. **Segoe UI typography** maintaining Microsoft ecosystem consistency
7. **Controller-first navigation** with clear focus states and white outline rings
8. **Cross-platform badges** indicating Series X|S, One, PC, and Cloud availability
9. **Social gaming features** with friends' presence, activity feeds, and parties
10. **Snappy interactions** (100-200ms) creating a responsive, modern feel

When implementing Xbox-style interfaces, prioritize:
- Dark immersive backgrounds with clear hierarchy
- Xbox Green for primary actions and Game Pass elements
- White focus rings for accessibility and controller navigation
- Gamerscore and achievement visibility
- Cross-platform and Smart Delivery clarity
- Fluent Design principles (depth, motion, material)
- Social features and friend presence
- Fast, responsive animations
