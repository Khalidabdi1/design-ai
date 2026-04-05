# Twitch Design System

> Live streaming platform with gaming-first aesthetic. Twitch Purple (#9146FF) accent, dark immersive backgrounds, real-time engagement through chat, emotes, and community features.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Twitch embodies a **vibrant, energetic, gaming-centric** design philosophy. The interface is built for extended viewing sessions, featuring deep dark backgrounds that let colorful content pop. Every element supports the core experience: watching live content while engaging with community through chat.

### Mood & Feeling
- **Electric & Alive**: Purple accents and live indicators create constant energy
- **Community-Driven**: Chat, emotes, and badges emphasize social interaction
- **Immersive**: Dark theme keeps focus on video content and reduces eye strain
- **Gamified**: Bits, subscriptions, and achievements add playful progression elements
- **Real-Time**: Live indicators, viewer counts, and chat streams emphasize immediacy

### Design Density
**Medium density** optimized for dual-focus: video content and chat. The left rail navigation is compact, video player dominates, and chat is information-dense but scannable. Cards in browse sections provide visual richness without overwhelming.

### Visual Character
- Bold purple accents on dark backgrounds
- Rounded corners (8px standard) for approachable feel
- Glowing/pulsing live indicators
- Gradient backgrounds in promotional areas
- Dense chat with emotes as first-class elements
- Stream thumbnails with live overlays
- Badge systems for subscriber recognition

---

## 2. Color Palette & Roles

### Primary Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-twitch-purple` | `#9146FF` | Primary brand, buttons, links, accents |
| `--color-twitch-purple-hover` | `#772CE8` | Purple hover states |
| `--color-twitch-purple-active` | `#5C16C5` | Purple pressed/active states |
| `--color-twitch-purple-light` | `#BF94FF` | Light purple for secondary accents |
| `--color-twitch-purple-dark` | `#451093` | Deep purple backgrounds |

### Background Colors (Dark Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--color-background-base` | `#0e0e10` | Page background, deepest level |
| `--color-background-alt` | `#18181b` | Cards, panels, elevated surfaces |
| `--color-background-alt-2` | `#1f1f23` | Secondary panels, hover states |
| `--color-background-input` | `#3d3d40` | Input fields, search bars |
| `--color-background-overlay` | `rgba(0, 0, 0, 0.6)` | Video overlays, modals |
| `--color-background-interactable-hover` | `#26262c` | Hover states on cards |
| `--color-background-interactable-selected` | `#3d3d40` | Selected/active states |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-text-base` | `#efeff1` | Primary body text, headings |
| `--color-text-alt` | `#adadb8` | Secondary text, metadata |
| `--color-text-alt-2` | `#7c7c8a` | Tertiary text, timestamps |
| `--color-text-link` | `#bf94ff` | Hyperlinks (light purple) |
| `--color-text-overlay` | `#ffffff` | Text on overlays, video |
| `--color-text-live` | `#eb0400` | Live indicator text |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-live` | `#eb0400` | Live indicators, recording |
| `--color-success` | `#00f593` | Success states, online |
| `--color-warning` | `#ffca5f` | Warnings, cautions |
| `--color-error` | `#eb0400` | Errors, destructive actions |
| `--color-info` | `#1db3ff` | Informational highlights |

### Special Feature Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-bits-teal` | `#1db3ff` | Bits, cheering |
| `--color-bits-purple` | `#9146ff` | Bit badge tiers |
| `--color-sub-purple` | `#9146ff` | Subscriptions |
| `--color-prime-blue` | `#00c8af` | Prime Gaming |
| `--color-hype-train` | `#ff6905` | Hype train events |
| `--color-raid` | `#9146ff` | Raid notifications |

### Light Theme (Alternate)

| Token | Hex | Role |
|-------|-----|------|
| `--color-background-base-light` | `#f7f7f8` | Page background |
| `--color-background-alt-light` | `#ffffff` | Cards, panels |
| `--color-text-base-light` | `#0e0e10` | Primary text |
| `--color-text-alt-light` | `#53535f` | Secondary text |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary UI font */
--font-base: 'Roobert', 'Inter', 'Helvetica Neue', Helvetica, Arial, sans-serif;

/* Monospace for code, stats */
--font-mono: 'SF Mono', 'Consolas', monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Page Title (H1) | 32px | 700 | 40px | -0.02em | `--color-text-base` |
| Section Title (H2) | 24px | 600 | 32px | -0.01em | `--color-text-base` |
| Card Title (H3) | 18px | 600 | 24px | 0 | `--color-text-base` |
| Subsection (H4) | 16px | 600 | 20px | 0 | `--color-text-base` |
| Body Large | 16px | 400 | 24px | 0 | `--color-text-base` |
| Body Regular | 14px | 400 | 20px | 0 | `--color-text-base` |
| Body Small | 13px | 400 | 18px | 0 | `--color-text-alt` |
| Caption | 12px | 400 | 16px | 0 | `--color-text-alt-2` |
| Button Text | 13px | 600 | 18px | 0 | White or contextual |
| Chat Message | 13px | 400 | 18px | 0 | `--color-text-base` |
| Stream Title | 14px | 600 | 20px | 0 | `--color-text-base` |
| Viewer Count | 13px | 400 | 18px | 0 | `--color-text-alt` |
| Category Tag | 12px | 500 | 16px | 0 | `--color-text-alt` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, descriptions, chat |
| 500 | Medium | Secondary emphasis, tags |
| 600 | Semibold | Headings, buttons, usernames |
| 700 | Bold | Page titles, strong emphasis |

### Special Typography

| Element | Style | Usage |
|---------|-------|-------|
| Live Badge | 12px, 700, uppercase | "LIVE" indicator |
| Viewer Count | 13px with eye icon | Stream metrics |
| Username (Chat) | 13px, 600, name color | Chat usernames |
| Emote Text | 28px emoji size | Inline emotes |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Purple)
```css
.button-primary {
  background: #9146ff;
  color: #ffffff;
  font-size: 13px;
  font-weight: 600;
  padding: 8px 16px;
  height: 30px;
  border-radius: 4px;
  border: none;
  transition: background-color 100ms ease;
}

.button-primary:hover {
  background: #772ce8;
}

.button-primary:active {
  background: #5c16c5;
}

.button-primary:disabled {
  background: #3d3d40;
  color: #7c7c8a;
  cursor: not-allowed;
}
```

#### Secondary Button (Outlined)
```css
.button-secondary {
  background: transparent;
  color: #bf94ff;
  font-size: 13px;
  font-weight: 600;
  padding: 8px 16px;
  height: 30px;
  border-radius: 4px;
  border: 2px solid #9146ff;
}

.button-secondary:hover {
  background: rgba(145, 70, 255, 0.2);
}
```

#### Tertiary Button (Ghost)
```css
.button-tertiary {
  background: transparent;
  color: #efeff1;
  font-size: 13px;
  font-weight: 600;
  padding: 8px 16px;
  border: none;
}

.button-tertiary:hover {
  background: #26262c;
}
```

#### Follow Button
```css
.button-follow {
  background: #9146ff;
  color: #ffffff;
  font-size: 13px;
  font-weight: 600;
  padding: 8px 16px;
  border-radius: 4px;
  display: inline-flex;
  align-items: center;
  gap: 6px;
}

.button-follow .heart-icon {
  width: 16px;
  height: 16px;
}

.button-following {
  background: transparent;
  border: 2px solid #9146ff;
  color: #bf94ff;
}
```

#### Subscribe Button
```css
.button-subscribe {
  background: #9146ff;
  color: #ffffff;
  padding: 8px 16px;
  border-radius: 4px;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 6px;
}

.button-subscribe .star-icon {
  width: 16px;
  height: 16px;
}
```

### Inputs

#### Search Input
```css
.input-search {
  background: #3d3d40;
  border: 2px solid transparent;
  border-radius: 6px;
  color: #efeff1;
  font-size: 14px;
  padding: 8px 12px 8px 36px;
  width: 100%;
  height: 36px;
}

.input-search:focus {
  border-color: #9146ff;
  outline: none;
}

.input-search::placeholder {
  color: #7c7c8a;
}

.input-search-icon {
  position: absolute;
  left: 10px;
  top: 50%;
  transform: translateY(-50%);
  color: #7c7c8a;
  width: 16px;
  height: 16px;
}
```

#### Chat Input
```css
.chat-input {
  background: #3d3d40;
  border: 2px solid transparent;
  border-radius: 4px;
  color: #efeff1;
  font-size: 13px;
  padding: 10px 12px;
  width: 100%;
  min-height: 38px;
  resize: none;
}

.chat-input:focus {
  border-color: #9146ff;
  outline: none;
}

.chat-input::placeholder {
  color: #adadb8;
}
```

### Cards

#### Stream Card (Browse)
```css
.stream-card {
  background: #18181b;
  border-radius: 8px;
  overflow: hidden;
  transition: transform 100ms ease;
}

.stream-card:hover {
  transform: translateY(-4px);
}

.stream-card-thumbnail {
  position: relative;
  aspect-ratio: 16 / 9;
  width: 100%;
}

.stream-card-thumbnail img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.stream-card-live-badge {
  position: absolute;
  top: 10px;
  left: 10px;
  background: #eb0400;
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 2px 6px;
  border-radius: 4px;
  text-transform: uppercase;
}

.stream-card-viewer-count {
  position: absolute;
  bottom: 10px;
  left: 10px;
  background: rgba(0, 0, 0, 0.6);
  color: #ffffff;
  font-size: 13px;
  padding: 2px 6px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  gap: 4px;
}

.stream-card-body {
  padding: 10px;
  display: flex;
  gap: 10px;
}

.stream-card-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  flex-shrink: 0;
}

.stream-card-info {
  flex: 1;
  min-width: 0;
}

.stream-card-title {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.stream-card-streamer {
  font-size: 13px;
  color: #adadb8;
  margin-top: 2px;
}

.stream-card-category {
  font-size: 13px;
  color: #adadb8;
  margin-top: 2px;
}

.stream-card-category:hover {
  color: #bf94ff;
}

.stream-card-tags {
  display: flex;
  gap: 6px;
  margin-top: 8px;
  flex-wrap: wrap;
}

.stream-card-tag {
  background: #3d3d40;
  color: #adadb8;
  font-size: 12px;
  padding: 2px 8px;
  border-radius: 9999px;
}
```

#### Category Card
```css
.category-card {
  position: relative;
  border-radius: 6px;
  overflow: hidden;
  transition: transform 100ms ease;
}

.category-card:hover {
  transform: scale(1.05);
}

.category-card-image {
  width: 100%;
  aspect-ratio: 3 / 4;
  object-fit: cover;
}

.category-card-info {
  padding: 8px 0;
}

.category-card-name {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
}

.category-card-viewers {
  font-size: 13px;
  color: #adadb8;
  margin-top: 2px;
}
```

#### Clip Card
```css
.clip-card {
  background: #18181b;
  border-radius: 6px;
  overflow: hidden;
}

.clip-card-thumbnail {
  position: relative;
  aspect-ratio: 16 / 9;
}

.clip-card-duration {
  position: absolute;
  bottom: 6px;
  right: 6px;
  background: rgba(0, 0, 0, 0.8);
  color: #ffffff;
  font-size: 12px;
  padding: 2px 4px;
  border-radius: 4px;
}

.clip-card-body {
  padding: 8px;
}

.clip-card-title {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
}

.clip-card-meta {
  font-size: 13px;
  color: #adadb8;
  margin-top: 4px;
}
```

### Navigation

#### Left Sidebar
```css
.sidebar {
  width: 50px;
  background: #1f1f23;
  height: 100vh;
  display: flex;
  flex-direction: column;
  padding: 10px 0;
}

.sidebar.expanded {
  width: 240px;
}

.sidebar-section {
  padding: 10px;
}

.sidebar-section-title {
  font-size: 13px;
  font-weight: 600;
  color: #adadb8;
  text-transform: uppercase;
  padding: 5px 10px;
  display: none;
}

.sidebar.expanded .sidebar-section-title {
  display: block;
}

.sidebar-channel {
  display: flex;
  align-items: center;
  padding: 5px 10px;
  border-radius: 4px;
  gap: 10px;
  cursor: pointer;
}

.sidebar-channel:hover {
  background: #26262c;
}

.sidebar-channel-avatar {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  position: relative;
}

.sidebar-channel-live-ring {
  position: absolute;
  inset: -3px;
  border: 2px solid #eb0400;
  border-radius: 50%;
}

.sidebar-channel-info {
  flex: 1;
  min-width: 0;
  display: none;
}

.sidebar.expanded .sidebar-channel-info {
  display: block;
}

.sidebar-channel-name {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
}

.sidebar-channel-game {
  font-size: 13px;
  color: #adadb8;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.sidebar-channel-viewers {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  color: #adadb8;
}

.sidebar-channel-viewers .live-dot {
  width: 8px;
  height: 8px;
  background: #eb0400;
  border-radius: 50%;
}
```

#### Top Navigation
```css
.top-nav {
  height: 50px;
  background: #18181b;
  display: flex;
  align-items: center;
  padding: 0 20px;
  gap: 20px;
}

.top-nav-logo {
  width: 28px;
  height: 32px;
  color: #9146ff;
}

.top-nav-links {
  display: flex;
  gap: 16px;
}

.top-nav-link {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
  padding: 8px 12px;
  border-radius: 4px;
}

.top-nav-link:hover {
  color: #bf94ff;
}

.top-nav-link.active {
  color: #9146ff;
}

.top-nav-search {
  flex: 1;
  max-width: 400px;
  margin: 0 auto;
}

.top-nav-actions {
  display: flex;
  gap: 10px;
  align-items: center;
}

.top-nav-user-avatar {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  cursor: pointer;
}

.top-nav-icon-button {
  width: 30px;
  height: 30px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #efeff1;
  cursor: pointer;
}

.top-nav-icon-button:hover {
  background: #26262c;
}
```

### Chat Components

#### Chat Container
```css
.chat {
  width: 340px;
  height: 100%;
  background: #18181b;
  display: flex;
  flex-direction: column;
}

.chat-header {
  height: 50px;
  padding: 0 10px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid #3d3d40;
}

.chat-header-title {
  font-size: 14px;
  font-weight: 600;
  color: #efeff1;
}

.chat-messages {
  flex: 1;
  overflow-y: auto;
  padding: 10px;
}

.chat-input-container {
  padding: 10px;
  border-top: 1px solid #3d3d40;
}
```

#### Chat Message
```css
.chat-message {
  padding: 5px 0;
  font-size: 13px;
  line-height: 18px;
  word-wrap: break-word;
}

.chat-message-badges {
  display: inline;
  margin-right: 4px;
}

.chat-message-badge {
  width: 18px;
  height: 18px;
  vertical-align: middle;
  margin-right: 2px;
}

.chat-message-username {
  font-weight: 600;
  cursor: pointer;
}

.chat-message-username:hover {
  text-decoration: underline;
}

.chat-message-colon {
  color: #efeff1;
}

.chat-message-text {
  color: #efeff1;
}

.chat-message-emote {
  width: 28px;
  height: 28px;
  vertical-align: middle;
  margin: -4px 1px;
}

.chat-message-mention {
  background: rgba(145, 70, 255, 0.3);
  padding: 2px 4px;
  border-radius: 2px;
}
```

#### Subscriber Badge Tiers
```css
.badge-subscriber-1 { /* 1 month */ }
.badge-subscriber-3 { /* 3 months */ }
.badge-subscriber-6 { /* 6 months */ }
.badge-subscriber-12 { /* 1 year */ }
.badge-subscriber-24 { /* 2 years */ }

.badge-mod {
  /* Moderator badge - green sword */
  color: #00f593;
}

.badge-vip {
  /* VIP badge - pink diamond */
  color: #e005b9;
}

.badge-broadcaster {
  /* Broadcaster badge - camera */
  color: #eb0400;
}
```

### Live Indicators

#### Live Badge
```css
.live-badge {
  background: #eb0400;
  color: #ffffff;
  font-size: 12px;
  font-weight: 700;
  padding: 2px 6px;
  border-radius: 4px;
  text-transform: uppercase;
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.live-badge::before {
  content: '';
  width: 6px;
  height: 6px;
  background: #ffffff;
  border-radius: 50%;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}
```

#### Viewer Count
```css
.viewer-count {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  color: #adadb8;
}

.viewer-count-icon {
  width: 14px;
  height: 14px;
  color: #eb0400;
}
```

### Raid/Host UI

#### Raid Notification
```css
.raid-notification {
  background: linear-gradient(135deg, #451093 0%, #9146ff 100%);
  border-radius: 8px;
  padding: 20px;
  text-align: center;
  animation: slideIn 300ms ease-out;
}

.raid-notification-title {
  font-size: 24px;
  font-weight: 700;
  color: #ffffff;
  margin-bottom: 8px;
}

.raid-notification-avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  border: 3px solid #ffffff;
  margin: 16px auto;
}

.raid-notification-name {
  font-size: 18px;
  font-weight: 600;
  color: #ffffff;
}

.raid-notification-viewers {
  font-size: 14px;
  color: rgba(255, 255, 255, 0.8);
  margin-top: 4px;
}

.raid-notification-actions {
  display: flex;
  gap: 12px;
  justify-content: center;
  margin-top: 16px;
}
```

### Bits & Subscriptions

#### Bits Cheer
```css
.bits-cheer {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  animation: bounce 500ms ease;
}

.bits-cheer-emote {
  width: 28px;
  height: 28px;
}

.bits-cheer-amount {
  font-weight: 700;
}

.bits-cheer-1 { color: #979797; } /* Gray: 1-99 */
.bits-cheer-100 { color: #9146ff; } /* Purple: 100-999 */
.bits-cheer-1000 { color: #1db3ff; } /* Blue: 1,000-4,999 */
.bits-cheer-5000 { color: #00f593; } /* Green: 5,000-9,999 */
.bits-cheer-10000 { color: #f43021; } /* Red: 10,000+ */

@keyframes bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-4px); }
}
```

#### Subscription Event
```css
.sub-event {
  background: linear-gradient(135deg, #9146ff 0%, #451093 100%);
  border-radius: 4px;
  padding: 12px;
  margin: 8px 0;
}

.sub-event-icon {
  width: 20px;
  height: 20px;
  color: #ffffff;
}

.sub-event-text {
  color: #ffffff;
  font-size: 13px;
}

.sub-event-username {
  font-weight: 700;
}

.sub-event-months {
  opacity: 0.9;
}
```

### Tooltips

```css
.tooltip {
  background: #0e0e10;
  color: #efeff1;
  font-size: 13px;
  padding: 8px 12px;
  border-radius: 4px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.4);
  max-width: 250px;
}

.tooltip-arrow {
  fill: #0e0e10;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.7);
}

.modal {
  background: #18181b;
  border-radius: 8px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.6);
  max-width: 460px;
  width: 100%;
}

.modal-header {
  padding: 20px;
  border-bottom: 1px solid #3d3d40;
}

.modal-title {
  font-size: 18px;
  font-weight: 600;
  color: #efeff1;
}

.modal-close {
  position: absolute;
  top: 10px;
  right: 10px;
  width: 30px;
  height: 30px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.modal-close:hover {
  background: #26262c;
}

.modal-body {
  padding: 20px;
}

.modal-footer {
  padding: 20px;
  border-top: 1px solid #3d3d40;
  display: flex;
  justify-content: flex-end;
  gap: 10px;
}
```

### Hype Train

```css
.hype-train {
  background: linear-gradient(90deg, #ff6905 0%, #eb0400 100%);
  padding: 10px 16px;
  display: flex;
  align-items: center;
  gap: 16px;
}

.hype-train-icon {
  width: 32px;
  height: 32px;
  animation: shake 500ms infinite;
}

.hype-train-level {
  font-size: 18px;
  font-weight: 700;
  color: #ffffff;
}

.hype-train-progress {
  flex: 1;
  height: 8px;
  background: rgba(255, 255, 255, 0.3);
  border-radius: 4px;
  overflow: hidden;
}

.hype-train-progress-bar {
  height: 100%;
  background: #ffffff;
  border-radius: 4px;
  transition: width 300ms ease;
}

.hype-train-time {
  font-size: 14px;
  font-weight: 600;
  color: #ffffff;
}

@keyframes shake {
  0%, 100% { transform: translateX(0); }
  25% { transform: translateX(-2px) rotate(-2deg); }
  75% { transform: translateX(2px) rotate(2deg); }
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-05` | 4px | Tight gaps, badge margins |
| `--space-1` | 8px | Component padding |
| `--space-2` | 10px | Standard gaps |
| `--space-3` | 16px | Section gaps |
| `--space-4` | 20px | Card padding, modal padding |
| `--space-5` | 24px | Large section breaks |
| `--space-6` | 32px | Page margins |

### Core Layout Structure (Stream View)

```
┌─────────────────────────────────────────────────────────────────┐
│  Top Navigation Bar (50px)                                       │
├─────┬───────────────────────────────────────────────┬───────────┤
│     │                                               │           │
│     │            Video Player                       │   Chat    │
│ Left│           (16:9 aspect)                       │  Panel    │
│Sidebar                                              │  (340px)  │
│(50px│                                               │           │
│ or  │───────────────────────────────────────────────│           │
│240px│   Stream Info Bar                             │           │
│)    │   (Channel, Title, Category, Follow/Sub)      │           │
│     │───────────────────────────────────────────────│           │
│     │   About / Chat Rules / Schedule Panels        │           │
│     │                                               │           │
└─────┴───────────────────────────────────────────────┴───────────┘
```

### Core Layout Structure (Browse View)

```
┌─────────────────────────────────────────────────────────────────┐
│  Top Navigation Bar (50px)                                       │
├─────┬───────────────────────────────────────────────────────────┤
│     │   Category / Filter Bar                                    │
│ Left│───────────────────────────────────────────────────────────│
│Sidebar  Stream Cards Grid                                        │
│(50px│   ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐             │
│ or  │   │        │ │        │ │        │ │        │             │
│240px│   │  Card  │ │  Card  │ │  Card  │ │  Card  │             │
│)    │   │        │ │        │ │        │ │        │             │
│     │   └────────┘ └────────┘ └────────┘ └────────┘             │
│     │   ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐             │
│     │   │  Card  │ │  Card  │ │  Card  │ │  Card  │             │
│     │   └────────┘ └────────┘ └────────┘ └────────┘             │
└─────┴───────────────────────────────────────────────────────────┘
```

### Panel Widths

| Panel | Width | Notes |
|-------|-------|-------|
| Left Sidebar (Collapsed) | 50px | Shows avatars only |
| Left Sidebar (Expanded) | 240px | Shows full channel info |
| Chat Panel | 340px | Fixed, collapsible |
| Video Player | Flexible | Maintains 16:9 aspect |
| Top Navigation | 50px height | Fixed |

### Grid System

```css
/* Browse page card grid */
.stream-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  padding: 20px;
}

/* Category grid (taller cards) */
.category-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 16px;
}
```

### Whitespace Philosophy
- **Immersive video**: Minimize chrome around video player
- **Dense but scannable**: Cards provide rich info without overwhelming
- **Breathing room in chat**: Messages have consistent spacing for readability
- **Compact sidebar**: Efficient space use for followed channels

### Content Width
- Stream page info: Max 1200px
- Browse cards: Minimum 300px per card
- Chat width: Fixed 340px
- Modal content: 460px typical

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Base surfaces |
| Level 1 | `0 1px 2px rgba(0,0,0,0.3)` | Cards, subtle lift |
| Level 2 | `0 4px 8px rgba(0,0,0,0.4)` | Dropdowns, popovers |
| Level 3 | `0 8px 16px rgba(0,0,0,0.5)` | Modals, dialogs |
| Level 4 | `0 16px 32px rgba(0,0,0,0.6)` | Full overlays |

### Surface Hierarchy

```
┌─────────────────────────────────────────────────────┐
│ Overlay (Modals)                 rgba(0,0,0,0.7)    │
├─────────────────────────────────────────────────────┤
│ Popover/Tooltip                  #0e0e10            │
├─────────────────────────────────────────────────────┤
│ Sidebar/Chat                     #18181b            │
├─────────────────────────────────────────────────────┤
│ Cards/Elevated                   #1f1f23            │
├─────────────────────────────────────────────────────┤
│ Page Background                  #0e0e10            │
└─────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, video |
| Sidebar | 100 | Left sidebar |
| Chat | 100 | Chat panel |
| Sticky | 200 | Top navigation |
| Dropdown | 1000 | Menus, autocomplete |
| Popout | 1001 | User cards, emote picker |
| Modal | 1002 | Modals, dialogs |
| Toast | 1003 | Notifications |
| Tooltip | 1004 | Tooltips |

### Overlay Treatment
- Modal backdrop: `rgba(0, 0, 0, 0.7)`
- Video controls overlay: `linear-gradient(transparent, rgba(0,0,0,0.8))`
- Thumbnail overlays: `rgba(0, 0, 0, 0.6)` for badges

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use Twitch Purple (#9146FF) as primary accent | Brand recognition, calls-to-action |
| Maintain dark backgrounds (#0e0e10, #18181b) | Eye comfort, video focus |
| Include live indicators with pulsing animation | Real-time urgency |
| Use rounded corners (8px cards, 4px buttons) | Approachable, modern feel |
| Show viewer counts prominently | Social proof, discovery |
| Display badges and emotes inline | Community identity |
| Provide dense chat with clear message separation | Scannable real-time content |
| Use gradient backgrounds for celebrations | Hype train, raids, subs |
| Include hover previews on thumbnails | Quick stream preview |
| Support emote autocomplete in chat | Efficient emote usage |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never use pure white backgrounds in dark mode | Jarring contrast, off-brand |
| Avoid hiding the chat panel by default | Chat is core to experience |
| Don't overcomplicate stream card info | Quick scanning is key |
| Never omit live status indicators | Users need to know what's live |
| Avoid slow loading thumbnails | Fast browsing is expected |
| Don't use small emotes (<20px) | Emotes must be recognizable |
| Never hide viewer counts | Key discovery metric |
| Avoid generic avatar placeholders | Each user should feel unique |
| Don't use purple on purple text | Contrast accessibility issues |
| Never autoplay audio without consent | Respect user control |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use energetic, community-focused language | Overly corporate tone |
| Celebrate subscription milestones | Downplay community contributions |
| Make raid/host events feel special | Treat them as routine |
| Provide clear follow/subscribe CTAs | Hide engagement options |
| Show streamer personality in UI | Make all channels look identical |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Desktop Large | >1440px | Full layout with expanded sidebar |
| Desktop | 1200px - 1440px | Standard layout |
| Desktop Small | 1024px - 1199px | Collapsed sidebar |
| Tablet | 768px - 1023px | Chat toggleable, single column browse |
| Mobile | <768px | Theater mode, drawer chat |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Left Sidebar | Fixed rail | Hidden, swipe drawer |
| Chat Panel | Fixed right | Full-screen drawer |
| Video Player | In-page | Full-width, theater mode |
| Browse Grid | Multi-column | Single or two column |
| Navigation | Full top bar | Simplified + bottom nav |
| Stream Cards | Card grid | Vertical list |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Follow Button | 44px height | Easy tap |
| Chat Send | 44px × 44px | Thumb-friendly |
| Stream Card | Full width tap | Entire card tappable |
| Navigation Icons | 44px × 44px | Comfortable touch |
| Emote Buttons | 36px × 36px | Frequent interaction |

### Theater Mode
- Video expands to fill viewport
- Chat overlays or hides
- Minimal UI chrome
- Quick toggle to exit

### Video Player Responsive
```css
.video-player {
  aspect-ratio: 16 / 9;
  max-height: calc(100vh - 50px); /* Minus nav */
}

@media (max-width: 768px) {
  .video-player {
    width: 100%;
    max-height: 40vh;
  }
}
```

### Image Handling
- Stream thumbnails: 16:9 aspect, lazy load
- Category art: 3:4 aspect (box art style)
- Avatars: 30-40px for compact, 64px for profiles
- Emotes: Multiple sizes (1x, 2x, 3x for density)

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
Primary Background: #0e0e10
Secondary Background: #18181b
Tertiary Background: #1f1f23
Input Background: #3d3d40

Twitch Purple: #9146ff
Purple Hover: #772ce8
Purple Active: #5c16c5
Purple Light: #bf94ff

Live Red: #eb0400
Success Green: #00f593
Warning Yellow: #ffca5f
Info Blue: #1db3ff

Text Primary: #efeff1
Text Secondary: #adadb8
Text Tertiary: #7c7c8a
Text Link: #bf94ff

Border Radius Cards: 8px
Border Radius Buttons: 4px
Border Radius Tags: 9999px (pill)
Border Radius Avatar: 50%

Font Primary: 'Roobert', 'Inter', system-ui
Font Size Body: 14px
Font Size Chat: 13px
Font Weight Bold: 700
Font Weight Semibold: 600
```

### Example Prompts

#### Stream Card Component
```
Create a stream card using Twitch's design system:
- Card background: #18181b with 8px border-radius
- Thumbnail: 16:9 aspect ratio with hover preview
- LIVE badge: Position top-left, #eb0400 background, white text, 12px bold uppercase
- Viewer count: Bottom-left overlay, semi-transparent black, white text with eye icon
- Avatar: 40px circle below thumbnail
- Stream title: 14px semibold #efeff1, single line with ellipsis
- Streamer name: 13px #adadb8, link hover to #bf94ff
- Category: 13px #adadb8, clickable
- Tags: Pill-shaped, #3d3d40 background, 12px text
- Hover: Translate Y -4px for lift effect
```

#### Chat Message Component
```
Design a chat message following Twitch conventions:
- Container: Padding 5px 0, font-size 13px, line-height 18px
- Badges: Inline 18px icons (sub, mod, VIP) before username
- Username: Semibold weight, custom color from user settings
- Colon separator: White color
- Message text: #efeff1, word-wrap for long messages
- Emotes: 28px inline images with vertical-align middle
- Mentions: Purple highlight background with 2px padding
- Timestamps: On hover, 12px #7c7c8a
```

#### Live Indicator
```
Create a live badge for Twitch:
- Background: #eb0400 (Twitch red)
- Text: White, 12px, 700 weight, uppercase "LIVE"
- Padding: 2px 6px
- Border-radius: 4px
- Optional: Pulsing dot animation before text
- Use for: Stream thumbnails, sidebar channels, player overlay
```

#### Raid Notification
```
Design a raid notification overlay:
- Background: Gradient from #451093 to #9146ff
- Container: 8px border-radius, centered, animated slide-in
- Title: "RAID!" 24px bold white
- Raider avatar: 64px circle with white 3px border
- Raider name: 18px semibold white
- Viewer count: 14px white 80% opacity
- Actions: Two buttons (Shoutout purple, Close ghost)
- Animation: Confetti or particle effects optional
```

#### Subscribe Button States
```
Create subscribe button variations:
- Default: #9146ff background, white text, star icon
- Subscribed: Outlined purple border, light purple text, checkmark icon
- Gifting: "Gift a Sub" with gift icon
- Hover: #772ce8 (darker purple)
- Size: 30px height, 13px semibold text
```

### CSS Variables Template

```css
:root {
  /* Backgrounds */
  --color-background-base: #0e0e10;
  --color-background-alt: #18181b;
  --color-background-alt-2: #1f1f23;
  --color-background-input: #3d3d40;
  --color-background-overlay: rgba(0, 0, 0, 0.6);
  
  /* Brand */
  --color-twitch-purple: #9146ff;
  --color-twitch-purple-hover: #772ce8;
  --color-twitch-purple-active: #5c16c5;
  --color-twitch-purple-light: #bf94ff;
  
  /* Text */
  --color-text-base: #efeff1;
  --color-text-alt: #adadb8;
  --color-text-alt-2: #7c7c8a;
  --color-text-link: #bf94ff;
  
  /* Semantic */
  --color-live: #eb0400;
  --color-success: #00f593;
  --color-warning: #ffca5f;
  --color-error: #eb0400;
  --color-info: #1db3ff;
  
  /* Special */
  --color-hype-train: #ff6905;
  --color-prime: #00c8af;
  
  /* Typography */
  --font-base: 'Roobert', 'Inter', 'Helvetica Neue', sans-serif;
  --font-size-body: 14px;
  --font-size-chat: 13px;
  --font-size-small: 12px;
  
  /* Spacing */
  --space-1: 8px;
  --space-2: 10px;
  --space-3: 16px;
  --space-4: 20px;
  
  /* Radii */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-round: 50%;
  --radius-pill: 9999px;
  
  /* Sizes */
  --sidebar-collapsed: 50px;
  --sidebar-expanded: 240px;
  --chat-width: 340px;
  --nav-height: 50px;
}
```

---

## Summary

Twitch's design system creates an immersive, community-driven live streaming experience through:

1. **Deep dark theme** with layered backgrounds (#0e0e10 base, #18181b panels)
2. **Signature Twitch Purple (#9146FF)** for brand recognition and CTAs
3. **Vibrant live indicators** using red (#eb0400) with pulsing animations
4. **Dense but scannable layouts** optimized for video + chat dual focus
5. **Rich community features** through badges, emotes, and celebration events
6. **Responsive video player** that maintains 16:9 with flexible layout
7. **Real-time engagement patterns** for chat, raids, subs, and bits

When implementing Twitch-style interfaces, prioritize:
- Dark mode as primary with purple accents
- Live status visibility at all times
- Fast, responsive thumbnail previews
- Chat as a first-class UI component
- Celebration moments for community events
- Efficient space use for following channels
- Smooth animations for state changes (100-300ms)
