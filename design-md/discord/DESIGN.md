# Discord Design System

> Community chat platform with gaming-focused aesthetic. Blurple accent (#5865F2), dark theme dominant, voice-first communication design.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Discord embraces a **gaming-centric, community-oriented** design philosophy. The interface feels like a cozy digital hangout—dark, immersive, and playful without being childish. Every element is designed to keep users engaged in conversations while minimizing eye strain during long sessions.

### Mood & Feeling
- **Immersive**: Deep dark backgrounds create focus on content and conversations
- **Playful yet mature**: Rounded corners and vibrant Blurple accent balanced with sophisticated layouts
- **Community-first**: Server icons, member lists, and voice channels emphasize group interaction
- **Always-on presence**: Status indicators, typing animations, and real-time updates everywhere

### Design Density
**Medium-high density** with intentional breathing room. Chat messages are compact but readable. Sidebars contain dense navigation (servers, channels, members) while the main content area remains focused on conversation flow.

### Visual Character
- Rounded corners throughout (gaming console influence)
- Smooth micro-animations for state changes
- Emoji and reactions as first-class UI elements
- Voice/video indicators integrated seamlessly
- Server icons as identity anchors (left rail)

---

## 2. Color Palette & Roles

### Primary Dark Theme

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#313338` | Main content area, chat background |
| `--background-secondary` | `#2b2d31` | Sidebars, channel lists, secondary panels |
| `--background-secondary-alt` | `#232428` | Hover states on secondary backgrounds |
| `--background-tertiary` | `#1e1f22` | Deepest background, server list, inputs |
| `--background-floating` | `#111214` | Modals, popouts, floating elements |
| `--background-modifier-hover` | `rgba(79, 84, 92, 0.16)` | Interactive hover states |
| `--background-modifier-active` | `rgba(79, 84, 92, 0.24)` | Active/pressed states |
| `--background-modifier-selected` | `rgba(79, 84, 92, 0.32)` | Selected items |

### Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--brand-500` (Blurple) | `#5865F2` | Primary accent, buttons, links, mentions |
| `--brand-560` | `#4752C4` | Blurple hover state |
| `--brand-600` | `#3C45A5` | Blurple pressed/active state |
| `--brand-260` | `#A5B3F0` | Light Blurple for hover text |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--text-normal` | `#dbdee1` | Primary body text, messages |
| `--text-muted` | `#949ba4` | Secondary text, timestamps, subtitles |
| `--text-link` | `#00a8fc` | Hyperlinks |
| `--header-primary` | `#f2f3f5` | Headers, usernames, important text |
| `--header-secondary` | `#b5bac1` | Subheaders, channel descriptions |
| `--text-positive` | `#23a55a` | Success states, online indicators |
| `--text-warning` | `#f0b232` | Warnings, idle status |
| `--text-danger` | `#f23f43` | Errors, do not disturb, destructive actions |

### Status Colors

| Token | Hex | Role |
|-------|-----|------|
| `--status-online` | `#23a55a` | Online presence indicator |
| `--status-idle` | `#f0b232` | Idle/Away status |
| `--status-dnd` | `#f23f43` | Do Not Disturb |
| `--status-offline` | `#80848e` | Offline/Invisible |
| `--status-streaming` | `#593695` | Streaming on Twitch/YouTube |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--green-360` | `#23a55a` | Success, confirmations, positive actions |
| `--yellow-300` | `#f0b232` | Warnings, cautions |
| `--red-400` | `#f23f43` | Errors, destructive actions, alerts |
| `--blue-345` | `#00a8fc` | Links, informational highlights |

### Light Theme (Alternate)

| Token | Hex | Role |
|-------|-----|------|
| `--background-primary` | `#ffffff` | Main content area |
| `--background-secondary` | `#f2f3f5` | Sidebars, secondary panels |
| `--background-tertiary` | `#e3e5e8` | Deepest sections, inputs |
| `--text-normal` | `#313338` | Primary body text |
| `--text-muted` | `#5c5e66` | Secondary text |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary app font (custom) */
--font-primary: 'gg sans', 'Noto Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;

/* Marketing/Display font */
--font-display: 'Poppins', 'gg sans', sans-serif;

/* Code blocks and monospace */
--font-code: 'Consolas', 'Monaco', 'Andale Mono', monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Server Name | 16px | 600 | 20px | 0 | `--header-primary` |
| Channel Category | 12px | 700 | 16px | 0.02em (uppercase) | `--channels-default` |
| Channel Name | 16px | 500 | 20px | 0 | `--channels-default` |
| Username (Chat) | 16px | 500 | 22px | 0 | Role color or `--header-primary` |
| Message Body | 16px | 400 | 22px | 0 | `--text-normal` |
| Timestamp | 12px | 500 | 22px | 0 | `--text-muted` |
| Modal Title | 20px | 600 | 24px | 0 | `--header-primary` |
| Button Text | 14px | 500 | 16px | 0 | White or contextual |
| Input Label | 12px | 700 | 16px | 0.02em (uppercase) | `--header-secondary` |
| Input Text | 16px | 400 | 20px | 0 | `--text-normal` |
| Tooltip | 14px | 500 | 18px | 0 | White |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 300 | Light | Rarely used, subtle text |
| 400 | Regular | Body text, messages, descriptions |
| 500 | Medium | Usernames, channel names, interactive elements |
| 600 | Semibold | Headers, server names, emphasis |
| 700 | Bold | Category labels, strong emphasis, uppercase labels |

### Marketing Typography (Poppins)

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Hero Headline | 56px | 700 | Landing page main headline |
| Section Title | 40px | 600 | Feature section headers |
| Subheadline | 24px | 500 | Supporting headlines |
| Body Large | 20px | 400 | Feature descriptions |
| Body Regular | 16px | 400 | Standard marketing copy |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Blurple)
```css
.button-primary {
  background: #5865F2;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 2px 16px;
  min-width: 60px;
  min-height: 38px;
  border-radius: 3px;
  border: none;
  transition: background-color 170ms ease;
}

.button-primary:hover {
  background: #4752C4;
}

.button-primary:active {
  background: #3C45A5;
}

.button-primary:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
```

#### Secondary Button (Gray)
```css
.button-secondary {
  background: #4e5058;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 2px 16px;
  min-height: 38px;
  border-radius: 3px;
}

.button-secondary:hover {
  background: #6d6f78;
}
```

#### Danger Button
```css
.button-danger {
  background: #f23f43;
  color: #ffffff;
}

.button-danger:hover {
  background: #da373c;
}
```

#### Link Button
```css
.button-link {
  background: transparent;
  color: #ffffff;
  padding: 2px 16px;
}

.button-link:hover {
  text-decoration: underline;
}
```

### Inputs

#### Text Input
```css
.input {
  background: #1e1f22;
  border: none;
  border-radius: 3px;
  color: #dbdee1;
  font-size: 16px;
  padding: 10px;
  width: 100%;
  height: 40px;
}

.input:focus {
  outline: none;
  /* No visible focus ring—Discord relies on context */
}

.input::placeholder {
  color: #87898c;
}
```

#### Text Area (Message Input)
```css
.textarea-message {
  background: #383a40;
  border-radius: 8px;
  color: #dbdee1;
  font-size: 16px;
  padding: 11px 16px;
  resize: none;
  min-height: 44px;
}
```

#### Input with Label
```css
.input-label {
  color: #b5bac1;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  margin-bottom: 8px;
}
```

### Cards

#### Server/Guild Card
```css
.card-server {
  background: #2b2d31;
  border-radius: 8px;
  padding: 16px;
  transition: background-color 150ms ease;
}

.card-server:hover {
  background: #35373c;
}
```

#### Embed Card (Link Preview)
```css
.embed {
  background: #2b2d31;
  border-left: 4px solid #5865F2; /* or custom color */
  border-radius: 4px;
  padding: 8px 16px 16px 12px;
  max-width: 520px;
}

.embed-title {
  color: #00a8fc;
  font-size: 16px;
  font-weight: 600;
}

.embed-description {
  color: #dbdee1;
  font-size: 14px;
  margin-top: 8px;
}
```

#### User Card (Profile Popout)
```css
.user-card {
  background: #232428;
  border-radius: 8px;
  width: 340px;
  overflow: hidden;
}

.user-card-banner {
  height: 60px;
  background: #5865F2; /* or banner image */
}

.user-card-avatar {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  border: 6px solid #232428;
  margin-top: -40px;
  margin-left: 16px;
}
```

### Messages

#### Message Container
```css
.message {
  padding: 2px 48px 2px 72px;
  position: relative;
  min-height: 44px;
}

.message:hover {
  background: rgba(79, 84, 92, 0.16);
}

.message-avatar {
  position: absolute;
  left: 16px;
  width: 40px;
  height: 40px;
  border-radius: 50%;
}

.message-username {
  color: #f2f3f5; /* or role color */
  font-size: 16px;
  font-weight: 500;
}

.message-timestamp {
  color: #949ba4;
  font-size: 12px;
  margin-left: 8px;
}

.message-content {
  color: #dbdee1;
  font-size: 16px;
  line-height: 22px;
}
```

#### Reaction Pill
```css
.reaction {
  background: #2b2d31;
  border-radius: 8px;
  padding: 4px 6px;
  display: inline-flex;
  align-items: center;
  gap: 6px;
  cursor: pointer;
  border: 1px solid transparent;
}

.reaction:hover {
  border-color: rgba(255, 255, 255, 0.1);
}

.reaction.reacted {
  background: rgba(88, 101, 242, 0.3);
  border-color: #5865F2;
}

.reaction-count {
  color: #dbdee1;
  font-size: 14px;
  font-weight: 500;
}
```

### Navigation

#### Server Icon (Pill List)
```css
.server-icon {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  transition: border-radius 200ms ease;
  background: #313338;
  display: flex;
  align-items: center;
  justify-content: center;
}

.server-icon:hover,
.server-icon.active {
  border-radius: 16px;
}

.server-icon.active::before {
  /* Left pill indicator */
  content: '';
  position: absolute;
  left: 0;
  width: 4px;
  height: 40px;
  background: #f2f3f5;
  border-radius: 0 4px 4px 0;
}
```

#### Channel Item
```css
.channel {
  padding: 6px 8px;
  margin: 1px 8px;
  border-radius: 4px;
  color: #949ba4;
  display: flex;
  align-items: center;
  gap: 6px;
}

.channel:hover {
  background: rgba(79, 84, 92, 0.32);
  color: #dbdee1;
}

.channel.active {
  background: rgba(79, 84, 92, 0.48);
  color: #f2f3f5;
}

.channel-icon {
  width: 20px;
  height: 20px;
  color: inherit;
}
```

#### Voice Channel
```css
.voice-channel {
  /* Same as channel but with voice indicators */
}

.voice-channel-users {
  margin-left: 24px;
  padding: 4px 0;
}

.voice-user {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 4px 8px;
  border-radius: 4px;
}

.voice-user-avatar {
  width: 20px;
  height: 20px;
  border-radius: 50%;
}

.voice-user-speaking {
  box-shadow: 0 0 0 2px #23a55a;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.85);
}

.modal {
  background: #313338;
  border-radius: 4px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.15),
              0 4px 8px rgba(0, 0, 0, 0.2);
  max-width: 440px;
  width: 100%;
}

.modal-header {
  padding: 16px;
  text-align: center;
}

.modal-title {
  color: #f2f3f5;
  font-size: 20px;
  font-weight: 600;
}

.modal-body {
  padding: 0 16px 20px;
}

.modal-footer {
  background: #2b2d31;
  padding: 16px;
  display: flex;
  justify-content: flex-end;
  gap: 8px;
}
```

### Tooltips

```css
.tooltip {
  background: #111214;
  color: #dbdee1;
  font-size: 14px;
  font-weight: 500;
  padding: 8px 12px;
  border-radius: 4px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.24);
  max-width: 190px;
}

.tooltip-arrow {
  fill: #111214;
}
```

### Context Menus

```css
.context-menu {
  background: #111214;
  border-radius: 4px;
  padding: 6px 8px;
  min-width: 188px;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.24);
}

.context-menu-item {
  padding: 6px 8px;
  border-radius: 2px;
  color: #b5bac1;
  font-size: 14px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.context-menu-item:hover {
  background: #5865F2;
  color: #ffffff;
}

.context-menu-item.danger {
  color: #f23f43;
}

.context-menu-item.danger:hover {
  background: #f23f43;
  color: #ffffff;
}

.context-menu-separator {
  height: 1px;
  background: #3f4147;
  margin: 4px 0;
}
```

### Status Indicators

```css
.status-indicator {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  border: 3px solid #1e1f22; /* matches avatar container bg */
}

.status-online { background: #23a55a; }
.status-idle { background: #f0b232; }
.status-dnd { background: #f23f43; }
.status-offline { background: #80848e; }

.status-streaming {
  background: #593695;
  border-radius: 3px;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-4` | 4px | Tight gaps, icon padding |
| `--spacing-8` | 8px | Standard element gaps |
| `--spacing-12` | 12px | Section gaps |
| `--spacing-16` | 16px | Card padding, modal padding |
| `--spacing-20` | 20px | Large section breaks |
| `--spacing-24` | 24px | Panel padding |

### Core Layout Structure

```
┌─────────────────────────────────────────────────────────────┐
│ ┌──────┬─────────┬──────────────────────────┬────────────┐ │
│ │      │         │                          │            │ │
│ │Server│ Channel │      Chat Messages       │  Member    │ │
│ │ List │  List   │                          │   List     │ │
│ │      │         │                          │            │ │
│ │ 72px │  240px  │       Flexible           │   240px    │ │
│ │      │         │                          │  (toggle)  │ │
│ │      │         │──────────────────────────│            │ │
│ │      │         │     Message Input        │            │ │
│ └──────┴─────────┴──────────────────────────┴────────────┘ │
└─────────────────────────────────────────────────────────────┘
```

### Panel Widths

| Panel | Width | Notes |
|-------|-------|-------|
| Server List | 72px | Fixed, vertically scrolling |
| Channel Sidebar | 240px | Fixed, contains channels + voice |
| Chat Area | Flexible | Min 480px, centered max-width for readability |
| Member Sidebar | 240px | Collapsible, shows online members |
| User Panel (Bottom) | 52px height | Shows current user status |

### Grid System
Discord uses a **flex-based layout** rather than traditional grid. Panels are fixed-width sidebars with a flexible center content area.

### Whitespace Philosophy
- **Compact but not cramped**: Messages have minimal vertical padding to show conversation flow
- **Visual grouping**: Related messages from same user collapse (no repeated avatar)
- **Breathing room in sidebars**: Channel categories have clear separation

### Content Width
- Messages max-width: Soft limit around 900px for readability
- Embeds max-width: 520px
- Modal content: 440px typical, 600px for settings

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Base surfaces |
| Level 1 | `0 1px 0 rgba(0,0,0,0.2)` | Dividers, subtle lift |
| Level 2 | `0 4px 8px rgba(0,0,0,0.2)` | Cards, dropdowns |
| Level 3 | `0 8px 16px rgba(0,0,0,0.24)` | Modals, popovers, tooltips |
| Level 4 | `0 16px 24px rgba(0,0,0,0.3)` | Full-screen overlays |

### Surface Hierarchy

```
┌─────────────────────────────────────────────────────────┐
│ Floating (Modals, Popouts)         #111214              │
├─────────────────────────────────────────────────────────┤
│ Tertiary (Server list, Inputs)     #1e1f22              │
├─────────────────────────────────────────────────────────┤
│ Secondary (Sidebars, Panels)       #2b2d31              │
├─────────────────────────────────────────────────────────┤
│ Primary (Chat, Main Content)       #313338              │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, messages |
| Sticky | 100 | Channel header, pinned elements |
| Dropdown | 1000 | Context menus, autocomplete |
| Popout | 1001 | User cards, emoji picker |
| Modal | 1002 | Modals, dialogs |
| Toast | 1003 | Notifications, toasts |
| Tooltip | 1004 | Tooltips (always on top) |

### Overlay Treatment
- Modal backdrop: `rgba(0, 0, 0, 0.85)` - heavy dim for focus
- Popout: No backdrop, positioned relative to trigger
- Click outside to dismiss for all floating elements

---

## 7. Do's and Don'ts

### ✅ Do's

| Guideline | Rationale |
|-----------|-----------|
| Use Blurple (#5865F2) as the primary accent | Brand recognition, interactive elements |
| Maintain dark backgrounds for all surfaces | Eye comfort for extended use, gaming context |
| Show user presence with status indicators | Community awareness, real-time feel |
| Use rounded corners (8px cards, 3-4px buttons) | Friendly, approachable, gaming aesthetic |
| Group messages from the same user | Reduce visual noise, show conversation flow |
| Display role colors for usernames | Community identity, server hierarchy |
| Include micro-animations for state changes | Smooth, polished interaction feedback |
| Use uppercase + letter-spacing for labels | Clear hierarchy, form guidance |
| Provide keyboard shortcuts | Power user efficiency |
| Show typing indicators | Real-time communication feel |

### ❌ Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never use pure white backgrounds | Jarring contrast, off-brand |
| Avoid sharp corners (0px radius) | Feels harsh, not Discord aesthetic |
| Don't use thin/light font weights for UI | Readability issues on dark backgrounds |
| Never omit status indicators for users | Loses presence awareness |
| Avoid blue links that match Blurple | Links should be cyan `#00a8fc` to differentiate |
| Don't overcrowd the message input | Keep it clean, one primary action |
| Avoid modals for simple confirmations | Use inline or toast patterns when possible |
| Don't hide the server list on desktop | Core navigation should remain visible |
| Never use generic avatar placeholders | Each user gets a unique default avatar |
| Avoid slow animations (>300ms) | Feels sluggish, gaming users expect speed |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use conversational, friendly tone | Overly formal or corporate language |
| Provide clear action labels ("Send", "Cancel") | Vague labels ("Submit", "OK") |
| Show error states inline with context | Generic error modals |
| Use emoji naturally in UI copy | Excessive emoji that feels forced |
| Confirm destructive actions | Delete without warning |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Desktop Large | >1200px | Full layout with member sidebar visible |
| Desktop | 940px - 1200px | Member sidebar collapsed by default |
| Tablet | 768px - 939px | Unified sidebar, swipe to reveal |
| Mobile | <768px | Single-panel view, bottom navigation |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Server List | Left rail, always visible | Swipe-in drawer from left |
| Channel List | Fixed sidebar | Full-screen when active |
| Member List | Right sidebar, toggleable | Swipe-in drawer from right |
| Message Input | Fixed bottom of chat | Fixed bottom, expands for multiline |
| Voice Controls | In-chat overlay | Bottom sheet |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Server Icon | 48px × 48px | Optimized for thumb |
| Channel Item | Full width × 36px | Easy tap targets |
| Message Actions | 32px × 32px | Shown on long-press |
| Buttons | 44px height minimum | Comfortable touch |

### Collapsing Strategy
1. **Member sidebar** collapses first (toggle-able)
2. **Channel sidebar** becomes overlay at tablet
3. **Server list** becomes swipe drawer at mobile
4. **Bottom navigation** appears on mobile for server/mentions/search

### Image Handling
- Avatars: 32-128px sizes with `border-radius: 50%`
- Server Icons: 48px default, supports GIF for Nitro servers
- Message images: Thumbnail with max 400px width, click to expand
- Embeds: Maintain aspect ratio, max-width 520px

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
Primary Background: #313338
Secondary Background: #2b2d31
Tertiary Background: #1e1f22
Floating Background: #111214

Blurple (Accent): #5865F2
Blurple Hover: #4752C4
Blurple Active: #3C45A5

Text Primary: #dbdee1
Text Muted: #949ba4
Text Link: #00a8fc
Headers: #f2f3f5

Status Online: #23a55a
Status Idle: #f0b232
Status DND: #f23f43
Status Offline: #80848e

Border Radius Cards: 8px
Border Radius Buttons: 3px
Border Radius Small: 4px
Border Radius Avatar: 50% (or 16px when active)

Font Primary: 'gg sans', system-ui
Font Display: 'Poppins', sans-serif
Font Code: 'Consolas', monospace
```

### Example Prompts

#### Server Discovery Card
```
Create a server discovery card using Discord's design system:
- Card background: #2b2d31 with 8px border-radius
- Server icon: 48px with dynamic border-radius (50% → 16px on hover)
- Server name: 16px semibold #f2f3f5
- Member count: 14px #949ba4
- Online indicator: 10px circle #23a55a
- Join button: Blurple #5865F2, 3px radius, "Join" text
- Hover state: Background lightens to #35373c
```

#### Message Component
```
Design a chat message following Discord conventions:
- Container: Horizontal padding 48px left (for avatar), 16px right
- Avatar: 40px circle positioned absolute left
- Username: 16px medium weight, color from role or #f2f3f5
- Timestamp: 12px #949ba4, appears on hover or after username
- Message body: 16px regular #dbdee1, line-height 22px
- Hover background: rgba(79, 84, 92, 0.16)
- Reactions: Pill-shaped, 8px radius, #2b2d31 background
```

#### Voice Channel UI
```
Create a voice channel component:
- Channel row: Same as text channel with speaker icon
- Connected users: Nested 24px left, show 20px avatars
- Speaking indicator: 2px #23a55a ring around avatar
- Mute/Deafen icons: 16px, #949ba4 when off, #f23f43 when active
- Screen share indicator: Green badge
- User limit: "1/10" in #949ba4 text
```

#### Modal Dialog
```
Design a confirmation modal for Discord:
- Overlay: rgba(0, 0, 0, 0.85)
- Modal: #313338 background, 4px border-radius
- Width: 440px
- Header: Centered, 20px semibold #f2f3f5
- Body: 16px #dbdee1 description
- Footer: #2b2d31 background, 16px padding
- Cancel button: Secondary gray #4e5058
- Confirm button: Blurple #5865F2 (or #f23f43 for destructive)
```

#### User Profile Popout
```
Create a user profile card:
- Card: 340px wide, #232428 background, 8px radius
- Banner: 60px tall, solid #5865F2 or custom image
- Avatar: 80px circle with 6px border matching card bg
- Position avatar: -40px margin-top, overlapping banner
- Username: 20px semibold #f2f3f5
- Status: 14px #949ba4
- Divider: 1px #3f4147
- Sections: Bio, Roles, Note with 12px uppercase labels
```

### CSS Variables Template

```css
:root {
  /* Backgrounds */
  --background-primary: #313338;
  --background-secondary: #2b2d31;
  --background-tertiary: #1e1f22;
  --background-floating: #111214;
  
  /* Brand */
  --brand-500: #5865F2;
  --brand-560: #4752C4;
  --brand-600: #3C45A5;
  
  /* Text */
  --text-normal: #dbdee1;
  --text-muted: #949ba4;
  --text-link: #00a8fc;
  --header-primary: #f2f3f5;
  --header-secondary: #b5bac1;
  
  /* Status */
  --green-360: #23a55a;
  --yellow-300: #f0b232;
  --red-400: #f23f43;
  
  /* Interactive */
  --background-modifier-hover: rgba(79, 84, 92, 0.16);
  --background-modifier-active: rgba(79, 84, 92, 0.24);
  --background-modifier-selected: rgba(79, 84, 92, 0.32);
  
  /* Typography */
  --font-primary: 'gg sans', 'Noto Sans', Helvetica, Arial, sans-serif;
  --font-display: 'Poppins', sans-serif;
  
  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  
  /* Radii */
  --radius-sm: 3px;
  --radius-md: 4px;
  --radius-lg: 8px;
  --radius-round: 50%;
}
```

---

## Summary

Discord's design system creates an immersive, gaming-centric communication experience through:

1. **Deep dark theme** with carefully layered backgrounds (#313338 → #1e1f22 → #111214)
2. **Signature Blurple (#5865F2)** accent that's instantly recognizable
3. **Rounded, friendly shapes** with 8px card radius and pill-shaped elements
4. **Real-time presence indicators** making the interface feel alive
5. **Compact but readable typography** using gg sans at 16px baseline
6. **Three-column layout** with flexible center content and fixed sidebars
7. **Community-first patterns** like server icons, role colors, and voice indicators

When implementing Discord-style interfaces, prioritize:
- Dark mode as the primary experience
- Smooth micro-animations for state changes
- Status indicators and presence awareness
- Consistent use of Blurple for interactive elements
- Comfortable density that supports long sessions
