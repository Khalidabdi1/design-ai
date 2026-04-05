# Threads (Meta) Design System

> A comprehensive design guide for Threads' visual identity (2023-2026)

---

## 1. Visual Theme & Atmosphere

### Brand Philosophy
Threads embodies a **clean, text-first, conversational** design philosophy. As Meta's text-based companion to Instagram, the platform prioritizes authentic conversations and community building through an interface that feels familiar to Instagram users while establishing its own distinct identity focused on written content.

### Core Aesthetic Principles
- **Minimalist purity**: Stark contrast between content and background with minimal visual noise
- **Text-first hierarchy**: Typography takes center stage, images are secondary
- **Instagram DNA**: Shares design language with Instagram while being distinctly text-focused
- **Conversation threads**: Visual connections between replies create flowing discussions
- **Clean negative space**: Generous whitespace allows content to breathe
- **Binary color modes**: Pure white or pure black backgrounds define each mode

### Emotional Tone
- **Approachable and casual**: Less formal than Twitter/X, more conversational
- **Connected community**: Design emphasizes human connection over broadcast
- **Fresh and modern**: Contemporary aesthetic that feels current and inviting
- **Calm and focused**: Reduced visual noise for a more peaceful experience
- **Instagram-adjacent**: Comfortable for Instagram users transitioning

### Visual Personality
| Attribute | Expression |
|-----------|------------|
| Simplicity | Stripped-down UI, essential elements only |
| Connection | Threaded replies, avatar clusters, visual continuity |
| Authenticity | Profile-first design, real identities from Instagram |
| Clarity | High contrast, readable typography, clear hierarchy |
| Modernity | Contemporary sans-serif typography, smooth animations |

---

## 2. Color Palette & Roles

### Primary Colors

| Color | Hex | RGB | Role |
|-------|-----|-----|------|
| White | `#FFFFFF` | rgb(255, 255, 255) | Primary background (light mode) |
| Black | `#000000` | rgb(0, 0, 0) | Primary background (dark mode) |
| Pure Black Text | `#000000` | rgb(0, 0, 0) | Primary text (light mode) |
| Pure White Text | `#FFFFFF` | rgb(255, 255, 255) | Primary text (dark mode) |

### Instagram Gradient (Branding Only)

| Color | Hex | Usage |
|-------|-----|-------|
| Instagram Yellow | `#FEDA77` | Logo gradient start |
| Instagram Orange | `#F58529` | Logo gradient |
| Instagram Pink | `#DD2A7B` | Logo gradient |
| Instagram Purple | `#8134AF` | Logo gradient |
| Instagram Blue | `#515BD4` | Logo gradient end |

> **Note**: The Instagram gradient is used exclusively for the Threads @ logo and occasional branding elements. It is NOT used in the UI.

### Extended Palette

#### Neutral Grays (Light Mode)
| Color | Hex | Usage |
|-------|-----|-------|
| Primary Text | `#000000` | Headlines, body text |
| Secondary Text | `#999999` | Timestamps, metadata, handles |
| Tertiary Text | `#737373` | Subtitles, hints |
| Divider | `#E0E0E0` | Borders, separators |
| Hover Surface | `#F5F5F5` | Hover states on cards |
| Input Background | `#F0F0F0` | Search bars, input fields |

#### Neutral Grays (Dark Mode)
| Color | Hex | Usage |
|-------|-----|-------|
| Primary Text | `#FFFFFF` | Headlines, body text |
| Secondary Text | `#777777` | Timestamps, metadata, handles |
| Tertiary Text | `#A8A8A8` | Subtitles, hints |
| Divider | `#262626` | Borders, separators |
| Hover Surface | `#1A1A1A` | Hover states on cards |
| Input Background | `#262626` | Search bars, input fields |

#### Semantic Colors
| Color | Hex | Usage |
|-------|-----|-------|
| Like Red | `#FF3040` | Like heart active state |
| Error Red | `#ED4956` | Error messages, delete |
| Link Blue | `#0095F6` | Links, mentions (Instagram blue) |
| Success Green | `#00A400` | Success states |
| Verified Blue | `#0095F6` | Verified badge |

### Color Application Rules

```
Background Layers (Light Mode):
├── Base: #FFFFFF (pure white)
├── Surface: #F5F5F5 (cards, hover)
├── Elevated: #EBEBEB (active states)
└── Borders: #E0E0E0 (dividers)

Background Layers (Dark Mode):
├── Base: #000000 (pure black)
├── Surface: #1A1A1A (cards, hover)
├── Elevated: #262626 (active states)
└── Borders: #262626 (dividers)
```

### Mode-Specific Variants
| Element | Light Mode | Dark Mode |
|---------|------------|-----------|
| Background | `#FFFFFF` | `#000000` |
| Primary Text | `#000000` | `#FFFFFF` |
| Secondary Text | `#999999` | `#777777` |
| Dividers | `#E0E0E0` | `#262626` |
| Cards | `#FFFFFF` | `#000000` |
| Input Fields | `#F0F0F0` | `#262626` |

---

## 3. Typography Rules

### Font Stack

```css
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
```

### Fallback Hierarchy
1. **-apple-system** (iOS/macOS San Francisco)
2. **BlinkMacSystemFont** (macOS Chrome San Francisco)
3. **Segoe UI** (Windows)
4. **Roboto** (Android/Chrome OS)
5. **Helvetica, Arial** (Universal fallbacks)

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| Display | 24px | 700 | 28px | -0.5px |
| Heading Large | 20px | 600 | 24px | -0.3px |
| Heading Medium | 17px | 600 | 22px | 0 |
| Body Large | 16px | 400 | 22px | 0 |
| Body | 15px | 400 | 20px | 0 |
| Body Bold | 15px | 600 | 20px | 0 |
| Caption | 13px | 400 | 18px | 0 |
| Small | 12px | 400 | 16px | 0.1px |
| Tiny | 11px | 400 | 14px | 0.1px |

### Typography Usage

#### Thread/Post Content
```css
.thread-content {
  font-size: 15px;
  font-weight: 400;
  line-height: 21px;
  color: #000000; /* light mode */
  word-wrap: break-word;
  white-space: pre-wrap;
}
```

#### Display Name
```css
.display-name {
  font-size: 15px;
  font-weight: 600;
  line-height: 20px;
  color: #000000; /* light mode */
}
```

#### Username/Handle
```css
.username {
  font-size: 15px;
  font-weight: 400;
  line-height: 20px;
  color: #999999; /* light mode */
}
```

#### Timestamps
```css
.timestamp {
  font-size: 15px;
  font-weight: 400;
  color: #999999; /* light mode */
}
```

### Special Text Treatments

#### Links & Mentions
- Color: `#0095F6` (Instagram Blue)
- No underline by default
- Underline on hover
- Mentions (@) and hashtags (#) use same color

#### Thread Indicators
- "Show replies" link: `#999999`
- Reply count: `#999999`
- "View thread" text: `#999999`

---

## 4. Component Stylings

### Buttons

#### Primary Button
```css
.btn-primary {
  background-color: #000000; /* light mode */
  color: #FFFFFF;
  font-size: 15px;
  font-weight: 600;
  padding: 8px 16px;
  height: 36px;
  border-radius: 10px;
  border: none;
  cursor: pointer;
  transition: opacity 0.2s;
}

.btn-primary:hover {
  opacity: 0.8;
}

.btn-primary:disabled {
  opacity: 0.3;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.btn-secondary {
  background-color: transparent;
  color: #000000; /* light mode */
  font-size: 15px;
  font-weight: 600;
  padding: 8px 16px;
  height: 36px;
  border-radius: 10px;
  border: 1px solid #E0E0E0;
  cursor: pointer;
  transition: background-color 0.2s;
}

.btn-secondary:hover {
  background-color: #F5F5F5;
}
```

#### Follow Button
```css
.btn-follow {
  background-color: #000000; /* light mode */
  color: #FFFFFF;
  font-size: 14px;
  font-weight: 600;
  padding: 6px 20px;
  min-width: 100px;
  height: 34px;
  border-radius: 10px;
  border: none;
}

.btn-following {
  background-color: transparent;
  color: #000000;
  border: 1px solid #DBDBDB;
}
```

### Thread/Post Card

```css
.thread-card {
  background-color: transparent;
  border-bottom: 1px solid #E0E0E0;
  padding: 12px 16px;
  display: flex;
  gap: 12px;
  cursor: pointer;
  transition: background-color 0.15s;
}

.thread-card:hover {
  background-color: #FAFAFA;
}
```

### Avatar

```css
.avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  object-fit: cover;
  flex-shrink: 0;
}

.avatar-large {
  width: 48px;
  height: 48px;
}

.avatar-profile {
  width: 84px;
  height: 84px;
  border: 2px solid #FFFFFF;
}
```

### Avatar with Gradient Ring (Story/Active)
```css
.avatar-ring {
  background: linear-gradient(45deg, #FEDA77, #F58529, #DD2A7B, #8134AF, #515BD4);
  padding: 3px;
  border-radius: 50%;
}

.avatar-ring .avatar {
  border: 3px solid #FFFFFF;
}
```

### Thread Line (Reply Connector)
```css
.thread-line {
  width: 2px;
  background-color: #E0E0E0;
  margin: 4px auto;
  flex-grow: 1;
  min-height: 20px;
}

/* Dark mode */
.thread-line-dark {
  background-color: #333333;
}
```

### Action Icons

```css
.action-icon {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: background-color 0.15s;
  color: #000000; /* light mode */
}

.action-icon:hover {
  background-color: #F0F0F0;
}

/* Like */
.action-like.active {
  color: #FF3040;
}

.action-like.active svg {
  fill: #FF3040;
}

/* Reply */
.action-reply:hover {
  color: #0095F6;
}

/* Repost */
.action-repost.active {
  color: #00A400;
}

/* Share */
.action-share:hover {
  background-color: #F0F0F0;
}
```

### Input Fields

```css
.input-field {
  background-color: #F0F0F0;
  border: none;
  border-radius: 12px;
  padding: 12px 16px;
  font-size: 16px;
  color: #000000;
  width: 100%;
  outline: none;
}

.input-field:focus {
  background-color: #EBEBEB;
}

.input-field::placeholder {
  color: #999999;
}
```

### Search Box

```css
.search-box {
  background-color: #F0F0F0;
  border: none;
  border-radius: 10px;
  padding: 10px 16px 10px 40px;
  font-size: 15px;
  color: #000000;
  width: 100%;
}

.search-box:focus {
  background-color: #EBEBEB;
}
```

### Modal/Dialog

```css
.modal-overlay {
  background-color: rgba(0, 0, 0, 0.65);
  position: fixed;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal-content {
  background-color: #FFFFFF;
  border-radius: 16px;
  max-width: 500px;
  max-height: 85vh;
  overflow-y: auto;
  width: 100%;
  margin: 20px;
}

/* Dark mode */
.modal-content-dark {
  background-color: #262626;
}
```

### Tabs

```css
.tab-item {
  padding: 16px 20px;
  font-size: 15px;
  font-weight: 600;
  color: #999999;
  border-bottom: 1px solid transparent;
  cursor: pointer;
  transition: color 0.15s;
  flex: 1;
  text-align: center;
}

.tab-item:hover {
  color: #000000;
}

.tab-item.active {
  color: #000000;
  border-bottom-color: #000000;
}
```

### Verified Badge
```css
.verified-badge {
  width: 14px;
  height: 14px;
  margin-left: 4px;
  display: inline-flex;
  align-items: center;
}

.verified-badge svg {
  fill: #0095F6;
}
```

### Reply Avatars Cluster (Stacked)
```css
.avatar-cluster {
  display: flex;
  margin-left: -8px;
}

.avatar-cluster .avatar {
  width: 20px;
  height: 20px;
  border: 2px solid #FFFFFF;
  margin-left: -6px;
}

.avatar-cluster .avatar:first-child {
  margin-left: 0;
}
```

---

## 5. Layout Principles

### Single-Column Layout (Mobile-First)

```
┌─────────────────────────────────────────────────────────┐
│                    Viewport (100%)                       │
├─────────────────────────────────────────────────────────┤
│                     Header Bar                           │
│  [Menu]          Threads Logo            [User Avatar]   │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  ┌─────────────────────────────────────────────────┐    │
│  │  [Avatar] Display Name · Timestamp              │    │
│  │  │        @username                             │    │
│  │  │                                              │    │
│  │  │  Thread content text goes here...            │    │
│  │  │                                              │    │
│  │  │  [Like] [Reply] [Repost] [Share]            │    │
│  │  │                                              │    │
│  │  ├──(thread line)───────────────────────────   │    │
│  │  │                                              │    │
│  │  │  [Avatar] Reply author                       │    │
│  │  │  Reply content...                            │    │
│  └─────────────────────────────────────────────────┘    │
│                                                          │
│  ─────────────────────────────────────────────────────  │
│                                                          │
│  ┌─────────────────────────────────────────────────┐    │
│  │  [Next Thread Card]                              │    │
│  └─────────────────────────────────────────────────┘    │
│                                                          │
├─────────────────────────────────────────────────────────┤
│                   Bottom Navigation                      │
│   [Home]  [Search]  [+Post]  [Activity]  [Profile]     │
└─────────────────────────────────────────────────────────┘
```

### Desktop Layout (Two-Column for Web)

```
┌───────────────────────────────────────────────────────────────┐
│                       Viewport (100%)                          │
├─────────────┬─────────────────────────────────┬───────────────┤
│  Sidebar    │         Main Feed               │   Right Side  │
│  (240px)    │         (640px)                 │   (Optional)  │
│             │                                 │               │
│  [Logo]     │   [Thread Cards]                │  [Suggested]  │
│  [Nav]      │   [+ New Thread]                │  [Trending]   │
│             │   [Threaded Replies]            │               │
│             │                                 │               │
│             │                                 │               │
│             │                                 │               │
│  [Profile]  │                                 │               │
└─────────────┴─────────────────────────────────┴───────────────┘
```

### Grid Specifications

| Element | Width | Notes |
|---------|-------|-------|
| Content Max Width | 640px | Main feed area |
| Left Sidebar | 240px | Desktop navigation |
| Right Sidebar | 320px | Optional, suggestions |
| Thread Card | 100% | Full width of content |
| Avatar Column | 48px | Including thread line space |
| Content Column | Flexible | Remainder of card width |

### Spacing System

```
Base Unit: 4px

Spacing Scale:
├── 2xs: 2px
├── xs: 4px
├── sm: 8px
├── md: 12px
├── lg: 16px
├── xl: 20px
├── 2xl: 24px
├── 3xl: 32px
└── 4xl: 48px
```

### Component Spacing

| Context | Padding/Margin |
|---------|----------------|
| Thread card | 12px 16px |
| Between action icons | 4px |
| Avatar to content | 12px |
| Thread line margin | 4px auto |
| Section divider | 0 (1px border) |
| Modal padding | 16px |
| Navigation item | 12px |

### Content Width Constraints

```css
.main-feed {
  max-width: 640px;
  width: 100%;
  margin: 0 auto;
}

.thread-content {
  max-width: 100%;
  overflow-wrap: break-word;
}

.media-container {
  max-width: 100%;
  border-radius: 12px;
  overflow: hidden;
  margin-top: 12px;
}
```

### Thread Reply Layout

```css
.thread-reply-container {
  display: flex;
  gap: 12px;
}

.thread-avatar-column {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 36px;
}

.thread-line {
  width: 2px;
  flex-grow: 1;
  background-color: #E0E0E0;
  margin: 4px 0;
}
```

---

## 6. Depth & Elevation

### Elevation Philosophy

Threads uses a **flat design approach** with virtually no shadows. Depth is communicated through:
1. **High contrast** between elements and backgrounds
2. **Border treatments** for separation
3. **Thread lines** for visual continuity
4. **Overlay opacity** for modals

### Surface Hierarchy (Light Mode)

| Level | Background | Use Case |
|-------|------------|----------|
| 0 - Base | `#FFFFFF` | Main background |
| 1 - Hover | `#FAFAFA` | Card hover states |
| 2 - Surface | `#F0F0F0` | Input fields, search |
| 3 - Active | `#EBEBEB` | Pressed states |
| 4 - Overlay | `rgba(0, 0, 0, 0.65)` | Modal backdrops |

### Surface Hierarchy (Dark Mode)

| Level | Background | Use Case |
|-------|------------|----------|
| 0 - Base | `#000000` | Main background |
| 1 - Hover | `#1A1A1A` | Card hover states |
| 2 - Surface | `#262626` | Input fields, modals |
| 3 - Active | `#363636` | Pressed states |
| 4 - Overlay | `rgba(0, 0, 0, 0.85)` | Modal backdrops |

### Shadow Usage

```css
/* Minimal shadow - primarily for floating elements (rare) */
.floating-button {
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.15);
}

/* Modal shadow */
.modal-content {
  box-shadow: 0 4px 24px rgba(0, 0, 0, 0.2);
}

/* Bottom sheet */
.bottom-sheet {
  box-shadow: 0 -4px 20px rgba(0, 0, 0, 0.15);
}
```

### Z-Index Scale

```
Base Content:      0
Thread Lines:      1
Sticky Header:     100
Bottom Navigation: 100
Dropdowns:         200
Tooltips:          300
Modal Overlay:     400
Modal Content:     500
Toast/Alerts:      600
```

### Border Treatments

```css
/* Primary dividers */
.divider {
  border-bottom: 1px solid #E0E0E0;
}

/* Dark mode dividers */
.divider-dark {
  border-bottom: 1px solid #262626;
}

/* Thread line */
.thread-connector {
  width: 2px;
  background-color: #E0E0E0;
}

/* Input focus - no visible ring, subtle background change */
.input:focus {
  background-color: #EBEBEB;
  outline: none;
}
```

### Animation & Transitions

```css
/* Standard transition */
.transition-default {
  transition: all 0.15s ease-out;
}

/* Hover effects */
.transition-hover {
  transition: background-color 0.15s ease;
}

/* Like animation */
@keyframes like-pop {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}

/* Modal entrance */
@keyframes modal-slide-up {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Fade in */
@keyframes fade-in {
  from { opacity: 0; }
  to { opacity: 1; }
}
```

---

## 7. Do's and Don'ts

### DO's

#### Colors
- Use pure white (`#FFFFFF`) or pure black (`#000000`) as backgrounds
- Keep the UI monochromatic (black, white, grays)
- Use Instagram blue (`#0095F6`) sparingly for links only
- Reserve the Instagram gradient exclusively for the Threads logo
- Maintain high contrast for readability

#### Typography
- Use system fonts for optimal performance and native feel
- Keep body text at 15px for comfortable reading
- Use semi-bold (600) for display names and emphasis
- Maintain consistent line heights (20-22px for body)

#### Components
- Use subtle border-radius (10-12px) for interactive elements
- Create visual thread continuity with connector lines
- Keep avatars circular with clean edges
- Provide clear but subtle hover states

#### Layout
- Center content with max-width constraints (640px)
- Use single-column layout for focus
- Maintain generous padding (12-16px)
- Keep thread replies visually connected

#### Interactions
- Show immediate feedback on actions
- Use subtle background color changes for hover
- Animate likes with a simple scale effect
- Keep transitions fast (150ms)

### DON'TS

#### Colors
- Don't use the Instagram gradient in the UI
- Don't add colored backgrounds to cards
- Don't use blue for anything except links
- Don't create custom color schemes
- Don't use mid-gray backgrounds

#### Typography
- Don't use custom or decorative fonts
- Don't go below 12px for any text
- Don't use all-caps styling
- Don't vary font weights dramatically
- Don't center-align body text

#### Components
- Don't use drop shadows on cards
- Don't add borders to thread cards
- Don't use pill-shaped buttons (use rounded rectangles)
- Don't break thread line continuity
- Don't overcomplicate action icons

#### Layout
- Don't exceed 640px content width
- Don't add multiple columns in the main feed
- Don't hide the thread line connectors
- Don't create dense layouts
- Don't use horizontal scrolling

#### Interactions
- Don't use complex animations
- Don't delay feedback more than 200ms
- Don't auto-play media with sound
- Don't use bounce effects
- Don't obscure content with overlays unnecessarily

### Common Mistakes to Avoid

| Mistake | Correct Approach |
|---------|------------------|
| Adding card shadows | Use border-bottom dividers only |
| Using gradient buttons | Use solid black/white buttons |
| Small avatars (< 36px) | Keep avatars 36-48px minimum |
| Breaking thread lines | Maintain continuous visual connection |
| Complex loading states | Use simple skeleton patterns |
| Colored action icons (default) | Icons are black/gray until active |

---

## 8. Responsive Behavior

### Breakpoint System

| Breakpoint | Width | Layout Changes |
|------------|-------|----------------|
| Desktop XL | ≥1200px | Three-column with right sidebar |
| Desktop | 1024-1199px | Two-column, sidebar + feed |
| Tablet | 768-1023px | Single column, collapsed nav |
| Mobile L | 428-767px | Single column, bottom nav |
| Mobile | <428px | Single column, compact spacing |

### Desktop (≥1024px)
```
┌──────────────────────────────────────────────────────┐
│ [Sidebar 240px]      [Feed 640px]      [Right 320px] │
│ - Full nav labels    - Full content    - Suggestions │
│ - Logo               - Threads         - Trending    │
│ - Profile link       - Thread lines    - Footer      │
└──────────────────────────────────────────────────────┘
```

### Tablet (768-1023px)
```
┌──────────────────────────────────────────────────────┐
│ [Header with logo]                                    │
│ [Feed - full width with max-width 640px centered]    │
│ [Bottom navigation bar]                               │
└──────────────────────────────────────────────────────┘
```

### Mobile (<768px)
```
┌─────────────────────────────┐
│ [Header: Menu | Logo | User] │
│                              │
│ [Thread Card]                │
│ [Thread Line]                │
│ [Reply Card]                 │
│ [───────────]                │
│ [Thread Card]                │
│                              │
│ [Bottom Nav Bar]             │
│ Home Search + Activity Profile│
└─────────────────────────────┘
```

### Mobile-Specific Components

#### Bottom Navigation Bar
```css
.bottom-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 50px;
  background-color: #FFFFFF;
  border-top: 1px solid #E0E0E0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-bottom: env(safe-area-inset-bottom);
}

/* Dark mode */
.bottom-nav-dark {
  background-color: #000000;
  border-top-color: #262626;
}
```

#### Floating Compose Button
```css
.fab-compose {
  position: fixed;
  bottom: 70px;
  right: 16px;
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background-color: #000000;
  color: #FFFFFF;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.2);
}

/* Note: Mobile primarily uses center nav button */
```

#### Mobile Header
```css
.mobile-header {
  position: sticky;
  top: 0;
  height: 48px;
  background-color: #FFFFFF;
  border-bottom: 1px solid #E0E0E0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 16px;
  z-index: 100;
}

.mobile-header-dark {
  background-color: #000000;
  border-bottom-color: #262626;
}
```

### Touch Optimizations
- Minimum touch target: 44x44px
- Swipe gestures for thread navigation
- Pull-to-refresh on feed
- Long-press for additional options
- Haptic feedback on actions (iOS)

### Image Responsiveness
```css
.media-container {
  width: 100%;
  border-radius: 12px;
  overflow: hidden;
  margin-top: 12px;
}

.media-container img {
  width: 100%;
  height: auto;
  max-height: 500px;
  object-fit: cover;
}

.media-container video {
  width: 100%;
  max-height: 600px;
}
```

### Safe Area Handling
```css
.bottom-nav {
  padding-bottom: env(safe-area-inset-bottom);
}

.content-area {
  padding-bottom: calc(50px + env(safe-area-inset-bottom));
}
```

---

## 9. Agent Prompt Guide

### System Prompt for Threads-Style UI Generation

```
You are an AI assistant specialized in generating user interfaces that match Threads' (Meta) design system. Follow these specifications precisely:

VISUAL FOUNDATION:
- Use pure white (#FFFFFF) for light mode background
- Use pure black (#000000) for dark mode background
- Primary text matches background inverse (black on white, white on black)
- Gray (#999999 light, #777777 dark) for secondary text
- Instagram blue (#0095F6) ONLY for links and mentions
- NO gradient usage except the Threads @ logo

TYPOGRAPHY:
- System font stack: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto
- Base size: 15px
- Line height: 20-22px
- Semi-bold (600) for names and emphasis
- Regular (400) for body content

COMPONENT PATTERNS:
- Buttons: Rounded rectangles (border-radius: 10px)
- Cards: No borders, border-bottom dividers only
- Avatars: Perfect circles, 36-48px
- Thread lines: 2px vertical connectors in gray
- Icons: Line style, 20-24px
- Inputs: Filled gray backgrounds, no borders

LAYOUT RULES:
- Max content width: 640px
- Single-column, text-first design
- Thread cards with avatar column + content column
- Visual thread connections between replies
- Card padding: 12px 16px

INTERACTION STATES:
- Hover: Subtle background (#FAFAFA light, #1A1A1A dark)
- Active icons: Red for like, green for repost
- Focus: Background color change (no rings)
- Disabled: 30% opacity
```

### Component Generation Prompts

#### Generate a Thread Card
```
Create a thread card component with:
- 36px circular avatar on the left
- Display name (semi-bold) with optional verified badge
- @username (gray) next to name
- Timestamp with "· Xh" format
- Body text at 15px with max content width
- Action bar with Like, Reply, Repost, Share icons
- Subtle hover state (#FAFAFA background)
- Border-bottom divider (#E0E0E0)
```

#### Generate a Threaded Reply Chain
```
Create a thread with replies showing:
- Main thread card (full)
- Vertical thread line (2px gray) connecting to replies
- Reply cards with smaller context
- Avatar cluster (3 stacked 20px avatars) for multiple replies
- "View more replies" link in gray
- Continuous visual flow from parent to children
```

#### Generate a Profile Header
```
Create a profile header with:
- Large circular avatar (84px)
- Display name with verified badge if applicable
- @username in gray below
- Bio text (15px, max 3 lines)
- Follower count with "followers" label
- Follow/Following button (rounded rectangle)
- Tabs: Threads | Replies
```

#### Generate Bottom Navigation
```
Create a bottom navigation bar with:
- 5 equally spaced icons
- Home (filled/outline toggle)
- Search (magnifying glass)
- Compose (plus in circle - center, larger)
- Activity (heart)
- Profile (user avatar circle)
- Active state: filled icon
- 50px height with safe area padding
```

### Color Usage Quick Reference

```
When to use Black (#000000):
- Light mode: Primary text, buttons, icons
- Dark mode: Background
- Display names
- Active nav icons

When to use White (#FFFFFF):
- Light mode: Background
- Dark mode: Primary text, icons
- Button text on dark buttons

When to use Gray (#999999 / #777777):
- Timestamps
- @usernames
- Secondary text
- Inactive icons
- Thread lines
- Placeholders

When to use Instagram Blue (#0095F6):
- Links
- Mentions (@)
- Hashtags (#)
- Verified badges
- NOTHING else

When to use Red (#FF3040):
- Active like state only
```

### Thread-Specific Patterns

```
Thread Line Structure:
├── Avatar (36px)
├── Thread Line (2px, gray, vertical)
└── Reply Avatar (36px)

Reply Clustering:
- 1 reply: Show single avatar
- 2-3 replies: Stack avatars with -6px overlap
- 4+ replies: Show 3 stacked + count

Action Icon States:
- Default: Gray outline (#999999)
- Hover: Slightly darker
- Active Like: Filled red (#FF3040)
- Active Repost: Filled green (#00A400)
```

### Common UI Patterns

```
Loading States:
- Skeleton screens with #E0E0E0 (light) or #262626 (dark)
- Pulse animation at 1.5s intervals
- Match exact thread card layout

Empty States:
- Simple illustration (optional)
- Bold headline centered
- Gray descriptive text
- Action button if applicable

Error States:
- Red text (#ED4956)
- Concise message
- Retry option

Success States:
- Minimal, inline feedback
- Quick toast (auto-dismiss 2s)
- Subtle animation
```

---

## Quick Reference Card

| Element | Value |
|---------|-------|
| Primary Background (Light) | `#FFFFFF` |
| Primary Background (Dark) | `#000000` |
| Primary Text (Light) | `#000000` |
| Primary Text (Dark) | `#FFFFFF` |
| Secondary Text (Light) | `#999999` |
| Secondary Text (Dark) | `#777777` |
| Link Blue | `#0095F6` |
| Like Red | `#FF3040` |
| Dividers (Light) | `#E0E0E0` |
| Dividers (Dark) | `#262626` |
| Font Family | System fonts |
| Base Font Size | 15px |
| Button Radius | 10px |
| Card Radius | N/A (flat) |
| Content Width | 640px |
| Avatar Size | 36-48px |
| Thread Line Width | 2px |
| Icon Size | 20-24px |
| Spacing Unit | 4px |
| Bottom Nav Height | 50px |

---

*Last updated: 2023-2026 Design System*
*Based on Threads (Meta) web and mobile applications*
