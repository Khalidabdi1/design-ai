# Snapchat Design System

> Camera-first social platform with ephemeral messaging. Signature Yellow (#FFFC00), playful Gen-Z aesthetic, Bitmoji-integrated, designed for spontaneous visual communication.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Snapchat embraces a **youthful, spontaneous, and ephemeral** design philosophy. The interface is built around the camera, treating it as the primary canvas rather than a feed. Every element feels playful, immediate, and personal—designed for quick, authentic moments rather than curated perfection.

### Mood & Feeling
- **Ephemeral**: Content disappears, creating urgency and authenticity
- **Playful**: Bold colors, fun animations, AR filters encourage creativity
- **Personal**: Bitmoji avatars, best friend rankings, streaks create intimate connections
- **Camera-First**: The camera is home, not a feature hidden behind menus
- **Gen-Z Native**: Speaks the language of younger generations without feeling forced

### Design Density
**Low-to-medium density** with generous touch targets and whitespace. The interface is optimized for quick thumb gestures—swiping, tapping, holding. Content takes center stage while navigation stays minimal and discoverable through gestures.

### Visual Character
- Camera viewfinder as the default home screen
- Circular avatars and story rings throughout
- Rounded corners on everything (cards, buttons, bubbles)
- Gradient-heavy visual treatments
- Ghost icon (Ghostface Chillah) as brand mascot
- Bold, vibrant color accents against clean backgrounds
- Heavy use of emojis, Bitmoji, and stickers as first-class UI elements

---

## 2. Color Palette & Roles

### Primary Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--snap-yellow` | `#FFFC00` | Primary brand color, logo, highlights |
| `--snap-yellow-light` | `#FFFB4D` | Yellow variants, glows |
| `--snap-yellow-dark` | `#E6E300` | Pressed states on yellow |
| `--snap-black` | `#000000` | Text on yellow, dark mode background |
| `--snap-white` | `#FFFFFF` | Light mode background, text on dark |

### Light Theme (Default)

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#FFFFFF` | Main app background |
| `--background-secondary` | `#F7F7F7` | Card backgrounds, subtle sections |
| `--background-tertiary` | `#EFEFEF` | Input fields, inactive areas |
| `--surface-elevated` | `#FFFFFF` | Floating cards, modals |
| `--border-subtle` | `#E8E8E8` | Subtle dividers, card borders |
| `--border-default` | `#D1D1D1` | Standard borders |

### Dark Theme

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#000000` | Main app background |
| `--background-secondary` | `#1C1C1C` | Card backgrounds, panels |
| `--background-tertiary` | `#2C2C2C` | Input fields, elevated sections |
| `--surface-elevated` | `#1C1C1C` | Floating elements |
| `--border-subtle` | `#2C2C2C` | Subtle dividers |
| `--border-default` | `#3C3C3C` | Standard borders |

### Text Colors

| Token | Light Mode | Dark Mode | Role |
|-------|------------|-----------|------|
| `--text-primary` | `#000000` | `#FFFFFF` | Headlines, primary content |
| `--text-secondary` | `#6E6E6E` | `#A0A0A0` | Subtitles, metadata, timestamps |
| `--text-tertiary` | `#999999` | `#666666` | Placeholders, hints |
| `--text-inverse` | `#FFFFFF` | `#000000` | Text on accent backgrounds |
| `--text-on-yellow` | `#000000` | `#000000` | Always black text on yellow |

### Chat Bubble Colors

| Token | Hex | Role |
|-------|-----|------|
| `--chat-sent` | `#0FADFF` | Sent text messages (blue) |
| `--chat-received` | `#9B9B9B` | Received text messages (gray) |
| `--chat-snap-sent` | `#E5395E` | Sent snap indicator (red) |
| `--chat-snap-received` | `#9B30FF` | Received snap indicator (purple) |
| `--chat-snap-viewed` | `#C4C4C4` | Opened/viewed snap |
| `--chat-delivered` | `#0FADFF` | Delivered message indicator |

### Snap Status Colors

| Token | Hex | Role |
|-------|-----|------|
| `--snap-red` | `#E5395E` | Snap without audio (sent/received) |
| `--snap-purple` | `#9B30FF` | Snap with audio |
| `--snap-blue` | `#0FADFF` | Chat message |
| `--snap-red-hollow` | `#E5395E` (outline) | Opened snap without audio |
| `--snap-purple-hollow` | `#9B30FF` (outline) | Opened snap with audio |
| `--snap-blue-hollow` | `#0FADFF` (outline) | Opened chat |

### Story Ring Gradients

| Type | Gradient | Role |
|------|----------|------|
| Unseen Story | `linear-gradient(135deg, #FFFC00 0%, #FF6600 100%)` | Yellow-orange ring |
| Close Friends | `linear-gradient(135deg, #00E676 0%, #00BFA5 100%)` | Green ring |
| Seen Story | `#D1D1D1` (solid) | Gray ring |
| Your Story | `linear-gradient(135deg, #0FADFF 0%, #7B68EE 100%)` | Blue-purple ring |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--success` | `#00E676` | Success states, streaks, verifications |
| `--warning` | `#FFB300` | Caution, pending states |
| `--error` | `#FF3B30` | Errors, destructive actions |
| `--info` | `#0FADFF` | Information, links |
| `--streak-fire` | `#FF9500` | Streak fire icon |

### Snapchat+ Premium

| Token | Hex | Role |
|-------|-----|------|
| `--plus-gold` | `#FFD700` | Snapchat+ badge |
| `--plus-gradient-start` | `#FFD700` | Premium gradient start |
| `--plus-gradient-end` | `#FF8C00` | Premium gradient end |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary app font */
--font-primary: 'Graphik', -apple-system, BlinkMacSystemFont, 'Avenir Next', 'Segoe UI', Roboto, sans-serif;

/* Display/Marketing font */
--font-display: 'Avenir Next', 'Graphik', system-ui, sans-serif;

/* Monospace for codes */
--font-mono: 'SF Mono', 'Menlo', 'Monaco', monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Title | 32px | 700 | 38px | -0.5px | `--text-primary` |
| Section Header | 24px | 700 | 30px | -0.3px | `--text-primary` |
| Page Title | 20px | 600 | 26px | 0 | `--text-primary` |
| Card Title | 17px | 600 | 22px | 0 | `--text-primary` |
| Body Large | 17px | 400 | 22px | 0 | `--text-primary` |
| Body Regular | 15px | 400 | 20px | 0 | `--text-primary` |
| Body Small | 13px | 400 | 18px | 0 | `--text-secondary` |
| Caption | 12px | 500 | 16px | 0.2px | `--text-secondary` |
| Micro | 10px | 600 | 14px | 0.5px | `--text-tertiary` |
| Username | 15px | 600 | 20px | 0 | `--text-primary` |
| Timestamp | 11px | 400 | 14px | 0.3px | `--text-tertiary` |
| Button Text | 15px | 600 | 20px | 0.3px | Contextual |
| Tab Label | 12px | 600 | 16px | 0.5px | Contextual |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, descriptions, chat messages |
| 500 | Medium | Subtitles, secondary buttons, metadata |
| 600 | Semibold | Usernames, titles, primary buttons |
| 700 | Bold | Headlines, section headers, emphasis |

### Text Styling

```css
/* Chat message text */
.chat-message {
  font-size: 15px;
  font-weight: 400;
  line-height: 20px;
  word-wrap: break-word;
}

/* Username in chat/story */
.username {
  font-size: 15px;
  font-weight: 600;
  line-height: 20px;
}

/* Discover headline */
.discover-headline {
  font-size: 20px;
  font-weight: 700;
  line-height: 24px;
  letter-spacing: -0.3px;
}

/* Story caption overlay */
.story-caption {
  font-size: 17px;
  font-weight: 500;
  line-height: 22px;
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.5);
}
```

---

## 4. Component Stylings

### Buttons

#### Primary Button (Yellow)
```css
.button-primary {
  background: #FFFC00;
  color: #000000;
  font-size: 15px;
  font-weight: 600;
  padding: 14px 24px;
  border-radius: 28px;
  border: none;
  min-height: 48px;
  transition: transform 150ms ease, background 150ms ease;
}

.button-primary:hover {
  background: #E6E300;
}

.button-primary:active {
  transform: scale(0.97);
  background: #D4D200;
}

.button-primary:disabled {
  background: #F0F0F0;
  color: #A0A0A0;
}
```

#### Secondary Button (Outlined)
```css
.button-secondary {
  background: transparent;
  color: #000000;
  font-size: 15px;
  font-weight: 600;
  padding: 14px 24px;
  border-radius: 28px;
  border: 2px solid #000000;
  min-height: 48px;
}

.button-secondary:hover {
  background: rgba(0, 0, 0, 0.05);
}

/* Dark mode variant */
.button-secondary.dark {
  color: #FFFFFF;
  border-color: #FFFFFF;
}
```

#### Ghost Button
```css
.button-ghost {
  background: transparent;
  color: #0FADFF;
  font-size: 15px;
  font-weight: 600;
  padding: 14px 24px;
  border: none;
}

.button-ghost:active {
  opacity: 0.7;
}
```

#### Icon Button
```css
.button-icon {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  background: rgba(0, 0, 0, 0.05);
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
}

.button-icon:active {
  background: rgba(0, 0, 0, 0.1);
}

/* Camera capture button */
.button-capture {
  width: 72px;
  height: 72px;
  border-radius: 50%;
  background: #FFFFFF;
  border: 4px solid #FFFFFF;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.button-capture:active {
  transform: scale(0.95);
}

.button-capture.recording {
  background: #E5395E;
  border-color: #E5395E;
}
```

### Chat Bubbles

#### Sent Message
```css
.chat-bubble-sent {
  background: #0FADFF;
  color: #FFFFFF;
  padding: 10px 14px;
  border-radius: 20px 20px 4px 20px;
  max-width: 75%;
  font-size: 15px;
  line-height: 20px;
}
```

#### Received Message
```css
.chat-bubble-received {
  background: #F0F0F0;
  color: #000000;
  padding: 10px 14px;
  border-radius: 20px 20px 20px 4px;
  max-width: 75%;
  font-size: 15px;
  line-height: 20px;
}

/* Dark mode */
.chat-bubble-received.dark {
  background: #2C2C2C;
  color: #FFFFFF;
}
```

#### Snap Indicator (in chat)
```css
.snap-indicator {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 0;
}

.snap-indicator-icon {
  width: 32px;
  height: 32px;
}

.snap-indicator.red .snap-indicator-icon {
  color: #E5395E;
}

.snap-indicator.purple .snap-indicator-icon {
  color: #9B30FF;
}

.snap-indicator.opened .snap-indicator-icon {
  fill: transparent;
  stroke: currentColor;
  stroke-width: 2px;
}

.snap-indicator-text {
  font-size: 13px;
  font-weight: 500;
  color: #6E6E6E;
}
```

### Story Ring / Avatar

#### Story Ring
```css
.story-ring {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  padding: 3px;
  background: linear-gradient(135deg, #FFFC00 0%, #FF6600 100%);
}

.story-ring-inner {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: #FFFFFF;
  padding: 2px;
}

.story-ring-avatar {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  object-fit: cover;
}

/* Viewed story */
.story-ring.viewed {
  background: #D1D1D1;
}

/* Close friends */
.story-ring.close-friends {
  background: linear-gradient(135deg, #00E676 0%, #00BFA5 100%);
}

/* No story */
.story-ring.no-story {
  background: transparent;
  border: 2px solid #E8E8E8;
}
```

#### Bitmoji Avatar
```css
.bitmoji-avatar {
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background: #FFFC00;
  overflow: hidden;
  position: relative;
}

.bitmoji-avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Bitmoji with action pose */
.bitmoji-avatar.action {
  width: 80px;
  height: 80px;
  border-radius: 0;
  background: transparent;
}

/* Status indicator */
.bitmoji-avatar .status {
  position: absolute;
  bottom: 2px;
  right: 2px;
  width: 14px;
  height: 14px;
  border-radius: 50%;
  border: 2px solid #FFFFFF;
  background: #00E676;
}
```

### Cards

#### Chat List Item
```css
.chat-list-item {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  gap: 12px;
  background: #FFFFFF;
}

.chat-list-item:active {
  background: #F7F7F7;
}

.chat-list-item-avatar {
  width: 56px;
  height: 56px;
  border-radius: 50%;
  flex-shrink: 0;
}

.chat-list-item-content {
  flex: 1;
  min-width: 0;
}

.chat-list-item-name {
  font-size: 15px;
  font-weight: 600;
  color: #000000;
}

.chat-list-item-preview {
  font-size: 13px;
  font-weight: 500;
  color: #6E6E6E;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.chat-list-item-meta {
  font-size: 11px;
  color: #999999;
}
```

#### Discover Card
```css
.discover-card {
  width: 100%;
  aspect-ratio: 16/9;
  border-radius: 16px;
  overflow: hidden;
  position: relative;
  background: #1C1C1C;
}

.discover-card-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.discover-card-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 16px;
  background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
}

.discover-card-title {
  font-size: 17px;
  font-weight: 700;
  color: #FFFFFF;
  line-height: 22px;
}

.discover-card-source {
  font-size: 12px;
  font-weight: 500;
  color: rgba(255, 255, 255, 0.7);
  margin-top: 4px;
}

/* Large discover card (featured) */
.discover-card.large {
  aspect-ratio: 4/5;
  border-radius: 24px;
}
```

#### Snap Map Friend Card
```css
.map-friend-card {
  background: #FFFFFF;
  border-radius: 20px;
  padding: 12px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
  display: flex;
  align-items: center;
  gap: 12px;
  max-width: 280px;
}

.map-friend-bitmoji {
  width: 48px;
  height: 48px;
}

.map-friend-info {
  flex: 1;
}

.map-friend-name {
  font-size: 15px;
  font-weight: 600;
  color: #000000;
}

.map-friend-location {
  font-size: 13px;
  color: #6E6E6E;
}

.map-friend-time {
  font-size: 11px;
  color: #999999;
}
```

### Navigation

#### Bottom Navigation
```css
.bottom-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 84px;
  padding-bottom: 20px; /* Safe area */
  background: #FFFFFF;
  display: flex;
  justify-content: space-around;
  align-items: center;
  border-top: 1px solid #E8E8E8;
}

.bottom-nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  padding: 8px 16px;
}

.bottom-nav-item-icon {
  width: 28px;
  height: 28px;
  color: #6E6E6E;
}

.bottom-nav-item.active .bottom-nav-item-icon {
  color: #000000;
}

.bottom-nav-item-label {
  font-size: 10px;
  font-weight: 600;
  color: #6E6E6E;
}

.bottom-nav-item.active .bottom-nav-item-label {
  color: #000000;
}

/* Camera button (center) */
.bottom-nav-camera {
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background: #FFFC00;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: -20px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.bottom-nav-camera-icon {
  width: 28px;
  height: 28px;
  color: #000000;
}
```

#### Header Navigation
```css
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 12px 16px;
  background: #FFFFFF;
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-title {
  font-size: 20px;
  font-weight: 700;
  color: #000000;
}

.header-icon {
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.header-icon svg {
  width: 24px;
  height: 24px;
  color: #000000;
}
```

### Inputs

#### Search Input
```css
.search-input {
  width: 100%;
  height: 44px;
  background: #F0F0F0;
  border: none;
  border-radius: 22px;
  padding: 0 16px 0 44px;
  font-size: 15px;
  font-weight: 400;
  color: #000000;
}

.search-input::placeholder {
  color: #999999;
}

.search-input-icon {
  position: absolute;
  left: 16px;
  top: 50%;
  transform: translateY(-50%);
  width: 20px;
  height: 20px;
  color: #999999;
}

/* Dark mode */
.search-input.dark {
  background: #2C2C2C;
  color: #FFFFFF;
}
```

#### Chat Input
```css
.chat-input-container {
  display: flex;
  align-items: flex-end;
  padding: 8px 12px;
  gap: 8px;
  background: #FFFFFF;
  border-top: 1px solid #E8E8E8;
}

.chat-input {
  flex: 1;
  min-height: 36px;
  max-height: 120px;
  background: #F0F0F0;
  border: none;
  border-radius: 18px;
  padding: 8px 16px;
  font-size: 15px;
  line-height: 20px;
  resize: none;
}

.chat-input-send {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background: #0FADFF;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
}

.chat-input-send svg {
  width: 20px;
  height: 20px;
  color: #FFFFFF;
}
```

### Modals & Overlays

#### Bottom Sheet
```css
.bottom-sheet-overlay {
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(4px);
}

.bottom-sheet {
  background: #FFFFFF;
  border-radius: 24px 24px 0 0;
  padding: 8px 0 34px;
  max-height: 85vh;
  overflow-y: auto;
}

.bottom-sheet-handle {
  width: 40px;
  height: 4px;
  background: #D1D1D1;
  border-radius: 2px;
  margin: 8px auto 16px;
}

.bottom-sheet-header {
  text-align: center;
  padding: 16px;
  border-bottom: 1px solid #E8E8E8;
}

.bottom-sheet-title {
  font-size: 17px;
  font-weight: 600;
  color: #000000;
}
```

#### Friend Profile Modal
```css
.profile-modal {
  background: #FFFFFF;
  border-radius: 24px;
  padding: 24px;
  text-align: center;
  max-width: 320px;
  margin: auto;
}

.profile-modal-bitmoji {
  width: 120px;
  height: 120px;
  margin: 0 auto 16px;
}

.profile-modal-name {
  font-size: 24px;
  font-weight: 700;
  color: #000000;
}

.profile-modal-username {
  font-size: 15px;
  font-weight: 500;
  color: #6E6E6E;
  margin-top: 4px;
}

.profile-modal-actions {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin-top: 24px;
}

.profile-modal-action {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
}

.profile-modal-action-icon {
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background: #F0F0F0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.profile-modal-action-label {
  font-size: 12px;
  font-weight: 500;
  color: #6E6E6E;
}
```

### Streaks & Badges

```css
.streak-indicator {
  display: flex;
  align-items: center;
  gap: 4px;
}

.streak-fire {
  width: 16px;
  height: 16px;
  color: #FF9500;
}

.streak-count {
  font-size: 13px;
  font-weight: 600;
  color: #FF9500;
}

/* Snapchat+ badge */
.plus-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  padding: 2px 8px;
  background: linear-gradient(135deg, #FFD700 0%, #FF8C00 100%);
  border-radius: 12px;
}

.plus-badge-text {
  font-size: 10px;
  font-weight: 700;
  color: #000000;
}

/* Best friend emoji indicators */
.friend-emoji {
  font-size: 14px;
  margin-left: 4px;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-2` | 2px | Micro gaps, icon padding |
| `--spacing-4` | 4px | Tight gaps, inline spacing |
| `--spacing-8` | 8px | Standard element gaps |
| `--spacing-12` | 12px | Card internal padding |
| `--spacing-16` | 16px | Section padding, margins |
| `--spacing-20` | 20px | Large gaps |
| `--spacing-24` | 24px | Modal padding, section breaks |
| `--spacing-32` | 32px | Major section spacing |

### Core Layout Structure

```
Camera View (Home)
┌─────────────────────────────────────┐
│  ┌─ Profile  Search ─┐              │
│  └───────────────────┘              │
│                                     │
│                                     │
│         [ Camera Feed ]             │
│                                     │
│                                     │
│  ┌── AR Lenses Carousel ──┐         │
│  └────────────────────────┘         │
│     ┌──────────────────┐            │
│     │  Capture Button  │            │
│     └──────────────────┘            │
│  ┌─Map─┬─Camera─┬─Chat─┐            │
│  └─────┴────────┴──────┘            │
└─────────────────────────────────────┘

Chat/Stories Screen
┌─────────────────────────────────────┐
│  ┌─ Back   Chat    New ─┐           │
│  └──────────────────────┘           │
│  ┌──────────────────────┐           │
│  │     Search Bar       │           │
│  └──────────────────────┘           │
│  ┌─ Stories (horizontal scroll) ──┐ │
│  │  [O] [O] [O] [O] [O] [O] [O]   │ │
│  └────────────────────────────────┘ │
│  ┌──────────────────────────────┐   │
│  │  Chat List Item              │   │
│  │  Chat List Item              │   │
│  │  Chat List Item              │   │
│  │  ...                         │   │
│  └──────────────────────────────┘   │
│  ┌─Map─┬─Camera─┬─Chat─┐            │
│  └─────┴────────┴──────┘            │
└─────────────────────────────────────┘
```

### Grid System
Snapchat uses a **fluid, gesture-based layout** rather than rigid grids. The primary navigation is horizontal swiping between major sections (Map | Camera | Chat | Discover).

#### Screen Navigation
- **Swipe Left** from Camera: Chat & Friends
- **Swipe Right** from Camera: Discover & Stories
- **Swipe Down** from Camera: Memories
- **Swipe Up** from Camera: Snap Map (or profiles)

### Content Width
- Full bleed for camera and stories
- 16px horizontal padding for lists and cards
- Max content width: 100% (edge-to-edge design)
- Modal max-width: 320px centered

### Whitespace Philosophy
- **Generous touch targets**: Minimum 44px for all interactive elements
- **Visual breathing room**: Stories and cards have clear separation
- **Camera dominance**: Camera view has minimal UI overlay
- **Dense chat lists**: Efficient vertical spacing for conversation scanning

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Flat surfaces, background |
| Level 1 | `0 1px 3px rgba(0,0,0,0.08)` | Subtle lift, cards |
| Level 2 | `0 4px 12px rgba(0,0,0,0.12)` | Floating buttons, chips |
| Level 3 | `0 8px 24px rgba(0,0,0,0.15)` | Modals, bottom sheets |
| Level 4 | `0 16px 48px rgba(0,0,0,0.2)` | Snap Map cards, overlays |

### Surface Hierarchy

```
┌─────────────────────────────────────────────────────────┐
│ Overlay (Modals, Profile)              Blur + Shadow    │
├─────────────────────────────────────────────────────────┤
│ Floating (Bottom sheets, Popovers)     #FFFFFF + L3     │
├─────────────────────────────────────────────────────────┤
│ Elevated (Cards, Buttons)              #FFFFFF + L1     │
├─────────────────────────────────────────────────────────┤
│ Primary (Main content)                 #FFFFFF          │
├─────────────────────────────────────────────────────────┤
│ Sunken (Inputs, secondary)             #F7F7F7          │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, camera feed |
| Sticky | 10 | Headers, navigation |
| Overlay Controls | 100 | Camera controls, AR lenses |
| Dropdown | 200 | Menus, autocomplete |
| Bottom Sheet | 300 | Action sheets, share menus |
| Modal | 400 | Dialogs, profiles |
| Toast | 500 | Notifications, snackbars |
| System | 600 | Loading states, critical alerts |

### Blur Effects

```css
/* Frosted glass effect */
.glass-surface {
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
}

/* Dark glass effect */
.glass-surface-dark {
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(20px);
}

/* Camera UI overlay */
.camera-overlay {
  background: transparent;
}

.camera-button-background {
  background: rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(8px);
  border-radius: 50%;
}
```

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use Snapchat Yellow (#FFFC00) as the primary brand accent | Instant brand recognition |
| Keep camera as the home screen experience | Camera-first philosophy |
| Use circular avatars and story rings consistently | Platform identity |
| Implement swipe gestures for navigation | Natural mobile interaction |
| Show Bitmoji avatars for personality | Personal connection |
| Use ephemeral indicators (viewed/delivered status) | Core platform concept |
| Apply rounded corners (16-24px on cards) | Friendly, approachable feel |
| Include streak indicators and friend emojis | Social engagement features |
| Use gradient story rings for unviewed content | Visual urgency |
| Design for full-bleed, edge-to-edge content | Modern mobile experience |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never make camera secondary to feeds | Breaks core platform identity |
| Avoid static, permanent content feel | Snapchat is about ephemeral moments |
| Don't use square avatars or sharp corners | Inconsistent with brand |
| Never use small touch targets (<44px) | Poor mobile usability |
| Avoid complex navigation hierarchies | Users expect swipe simplicity |
| Don't overload camera UI with controls | Keep focus on capturing |
| Avoid formal, corporate tone | Target audience is Gen-Z |
| Never show raw timestamps (use "2h ago") | More casual, approachable |
| Don't forget dark mode support | User expectation |
| Avoid heavy text-based interfaces | Visual-first platform |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use casual, friendly language | Formal corporate speak |
| Show relative timestamps ("Just now", "5m") | Exact timestamps everywhere |
| Include emoji and Bitmoji naturally | Text-heavy explanations |
| Give immediate visual feedback on actions | Silent state changes |
| Communicate through status colors | Rely only on text labels |
| Keep copy short and scannable | Long paragraphs of text |

---

## 8. Responsive Behavior

### Device Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Mobile Small | <375px | Compact layouts, smaller avatars |
| Mobile Standard | 375px-414px | Default design specs |
| Mobile Large | 414px-428px | Slightly larger touch targets |
| Tablet | 768px+ | Not primary target, scaled mobile |

### Mobile-First Adaptations

| Component | Standard Mobile | Large Mobile |
|-----------|-----------------|--------------|
| Story Ring | 64px | 72px |
| Avatar (Chat List) | 56px | 60px |
| Bottom Nav Height | 84px (with safe area) | 84px |
| Card Border Radius | 16px | 20px |
| Chat Bubble Max Width | 75% | 70% |

### Touch Targets

| Element | Minimum Size | Recommended |
|---------|--------------|-------------|
| Any tappable element | 44px × 44px | 48px × 48px |
| Primary CTA buttons | 48px height | 56px height |
| Capture button | 72px × 72px | 72px × 72px |
| Story ring (tappable) | 64px × 64px | 64px × 64px |
| Bottom nav item | 64px × 64px | 68px × 68px |

### Gesture Zones

```
┌─────────────────────────────────────┐
│          [Swipe Down]               │ → Memories / Profile
│  ┌───┐                       ┌───┐  │
│  │ < │                       │ > │  │
│  │ S │     [Camera View]     │ S │  │
│  │ W │                       │ W │  │
│  │ I │                       │ I │  │
│  │ P │                       │ P │  │
│  │ E │                       │ E │  │
│  └───┘                       └───┘  │
│   ↓                           ↓     │
│  Chat                      Discover │
│                                     │
│          [Swipe Up]                 │ → Snap Map
└─────────────────────────────────────┘
```

### Safe Areas

```css
/* iOS Safe Area handling */
.bottom-nav {
  padding-bottom: env(safe-area-inset-bottom, 20px);
}

.header {
  padding-top: env(safe-area-inset-top, 0);
}

.camera-controls {
  margin-bottom: calc(84px + env(safe-area-inset-bottom, 20px));
}
```

### Orientation
- **Portrait only** for main app experience
- Camera and stories locked to portrait
- Snaps can be viewed in captured orientation

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Brand Colors
Snap Yellow: #FFFC00
Snap Black: #000000
Snap White: #FFFFFF

# Chat Colors
Sent Message (Blue): #0FADFF
Received (Gray Light): #F0F0F0
Snap Red (No Audio): #E5395E
Snap Purple (Audio): #9B30FF

# Story Ring
Unseen: gradient(#FFFC00, #FF6600)
Viewed: #D1D1D1
Close Friends: gradient(#00E676, #00BFA5)

# Text
Primary: #000000 (light) / #FFFFFF (dark)
Secondary: #6E6E6E (light) / #A0A0A0 (dark)
Tertiary: #999999 (light) / #666666 (dark)

# Backgrounds
Light Primary: #FFFFFF
Light Secondary: #F7F7F7
Dark Primary: #000000
Dark Secondary: #1C1C1C

# Border Radius
Buttons: 28px (pill)
Cards: 16-24px
Chat Bubbles: 20px (with 4px tail)
Avatars: 50% (circle)

# Fonts
Primary: Graphik, Avenir Next, system-ui
Weights: 400, 500, 600, 700
Base Size: 15px
```

### Example Prompts

#### Chat List Screen
```
Create a Snapchat chat list following the design system:
- Header: White background, "Chat" title 20px bold, search + new chat icons
- Search bar: #F0F0F0 background, 44px height, 22px border-radius
- Stories row: Horizontal scroll, 64px story rings with gradient borders
- Each chat item: 56px Bitmoji avatar, username 15px semibold, preview 13px gray
- Status indicators: Red/purple filled squares for unopened, hollow for opened
- Streak fire emoji with count in orange
- Bottom nav: Map, Camera (yellow 56px circle), Chat icons
```

#### Story Ring Component
```
Design a Snapchat story ring:
- Outer ring: 64px circle
- Gradient border: 3px, from #FFFC00 to #FF6600
- Inner white ring: 2px
- Avatar: Circular Bitmoji image
- Viewed state: Solid #D1D1D1 border instead of gradient
- Username below: 12px medium, centered
- Tap area: Full 64px circle
```

#### Camera Capture Screen
```
Create the Snapchat camera interface:
- Full-bleed camera viewfinder
- Top row: Profile Bitmoji (left), Search icon (right)
- AR lens carousel: Horizontal scroll at bottom above capture
- Capture button: 72px white circle, 4px border
- Left of capture: Gallery thumbnail (rounded square)
- Right of capture: Flip camera icon
- Recording state: Red fill on capture button
- Bottom nav: Semi-transparent, icons for Map/Chat/Discover
```

#### Discover Card
```
Design a Snapchat Discover card:
- Card: 16/9 aspect ratio, 16px border-radius
- Background: Full-bleed image
- Gradient overlay: transparent to rgba(0,0,0,0.8) at bottom
- Title: 17px bold white, max 2 lines
- Source name: 12px medium, white at 70% opacity
- Optional: "Sponsored" tag in top corner
- Tap feedback: Scale to 0.98
```

#### Friend Profile Modal
```
Create a Snapchat friend profile:
- Modal: White background, 24px border-radius
- Centered Bitmoji: 120px
- Display name: 24px bold
- Username: 15px gray, prefixed with @
- Snapchat+ badge if applicable (gold gradient pill)
- Action buttons: 56px circles for Send Snap, Chat, Video Call
- Stats: Snap Score, mutual friends count
- Close button: X in top right
```

### CSS Variables Template

```css
:root {
  /* Brand */
  --snap-yellow: #FFFC00;
  --snap-black: #000000;
  --snap-white: #FFFFFF;
  
  /* Chat */
  --chat-blue: #0FADFF;
  --chat-gray: #F0F0F0;
  --snap-red: #E5395E;
  --snap-purple: #9B30FF;
  
  /* Backgrounds (Light) */
  --bg-primary: #FFFFFF;
  --bg-secondary: #F7F7F7;
  --bg-tertiary: #EFEFEF;
  
  /* Backgrounds (Dark) */
  --bg-primary-dark: #000000;
  --bg-secondary-dark: #1C1C1C;
  --bg-tertiary-dark: #2C2C2C;
  
  /* Text (Light) */
  --text-primary: #000000;
  --text-secondary: #6E6E6E;
  --text-tertiary: #999999;
  
  /* Text (Dark) */
  --text-primary-dark: #FFFFFF;
  --text-secondary-dark: #A0A0A0;
  --text-tertiary-dark: #666666;
  
  /* Semantic */
  --success: #00E676;
  --warning: #FFB300;
  --error: #FF3B30;
  --streak: #FF9500;
  
  /* Story Gradients */
  --story-unseen: linear-gradient(135deg, #FFFC00, #FF6600);
  --story-close: linear-gradient(135deg, #00E676, #00BFA5);
  --story-viewed: #D1D1D1;
  
  /* Typography */
  --font-family: 'Graphik', -apple-system, BlinkMacSystemFont, 'Avenir Next', sans-serif;
  
  /* Spacing */
  --space-4: 4px;
  --space-8: 8px;
  --space-12: 12px;
  --space-16: 16px;
  --space-24: 24px;
  --space-32: 32px;
  
  /* Radii */
  --radius-sm: 8px;
  --radius-md: 16px;
  --radius-lg: 24px;
  --radius-pill: 28px;
  --radius-round: 50%;
  
  /* Shadows */
  --shadow-sm: 0 1px 3px rgba(0,0,0,0.08);
  --shadow-md: 0 4px 12px rgba(0,0,0,0.12);
  --shadow-lg: 0 8px 24px rgba(0,0,0,0.15);
}
```

---

## Summary

Snapchat's design system creates a youthful, camera-first communication experience through:

1. **Signature Yellow (#FFFC00)** as the instantly recognizable brand anchor
2. **Camera-first philosophy** with the viewfinder as home screen
3. **Ephemeral visual language** using status colors (red/purple/blue) and hollow indicators
4. **Circular avatars and Bitmoji** for personal, playful identity
5. **Gradient story rings** creating visual urgency for unviewed content
6. **Gesture-driven navigation** (swipe between Map, Camera, Chat, Discover)
7. **Pill-shaped buttons** and generous border-radius (16-24px) for friendly feel
8. **Chat bubble system** with distinct sent (blue) and received (gray) styling
9. **Dark mode support** with pure black backgrounds

When implementing Snapchat-style interfaces, prioritize:
- Camera viewfinder as the central experience
- Swipe gestures over tab navigation
- Story rings with gradient borders for engagement
- Bitmoji integration for personality
- Ephemeral content indicators (viewed, delivered, screenshots)
- Mobile-first, thumb-friendly design
- Playful, Gen-Z appropriate tone and visual language
