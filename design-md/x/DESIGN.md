# X (Twitter) Design System

> A comprehensive design guide for X's current visual identity (2024-2026)

---

## 1. Visual Theme & Atmosphere

### Brand Philosophy
X embodies a **minimalist, content-first** design philosophy. The platform prioritizes rapid information consumption and real-time engagement through an interface that fades into the background, allowing content to take center stage.

### Core Aesthetic Principles
- **Dark-mode dominance**: Pure black backgrounds create an immersive, distraction-free experience
- **High contrast**: Sharp contrast between text and background for maximum readability
- **Monochromatic foundation**: Black, white, and blue form the entire visual language
- **Editorial clarity**: Clean typography and generous whitespace enable rapid scanning
- **Functional minimalism**: Every element serves a purpose; decorative elements are eliminated

### Emotional Tone
- **Professional yet accessible**: Serious enough for news, casual enough for memes
- **Fast and immediate**: Design suggests real-time, always-updating content
- **Global and neutral**: Culturally agnostic visual language
- **Bold simplicity**: The X logo represents transformation and confident rebrand

### Visual Personality
| Attribute | Expression |
|-----------|------------|
| Speed | Instant loading states, minimal animations |
| Authenticity | Raw, unfiltered content presentation |
| Connectivity | Threaded conversations, quoted posts |
| Accessibility | High contrast, clear hierarchy |

---

## 2. Color Palette & Roles

### Primary Colors

| Color | Hex | RGB | Role |
|-------|-----|-----|------|
| Black | `#000000` | rgb(0, 0, 0) | Primary background (dark mode) |
| White | `#FFFFFF` | rgb(255, 255, 255) | Primary text, light mode background |
| X Blue | `#1D9BF0` | rgb(29, 155, 240) | Links, highlights, interactive elements |

### Extended Palette

#### Neutral Grays
| Color | Hex | Usage |
|-------|-----|-------|
| Dark Gray | `#0F1419` | Text on light backgrounds |
| Medium Gray | `#536471` | Secondary text, timestamps |
| Light Gray | `#71767B` | Placeholder text, disabled states |
| Border Gray | `#2F3336` | Dividers, card borders (dark mode) |
| Hover Gray | `#1D1F23` | Hover states on dark backgrounds |
| Surface Gray | `#16181C` | Elevated surfaces, cards (dark mode) |

#### Semantic Colors
| Color | Hex | Usage |
|-------|-----|-------|
| Success Green | `#00BA7C` | Repost (retweet) icon active |
| Like Pink | `#F91880` | Like heart icon active |
| Warning Yellow | `#FFD400` | Gold/Premium indicators |
| Error Red | `#F4212E` | Errors, delete confirmations |
| Premium Gold | `#E2B719` | Verified organization badge |

### Color Application Rules

```
Background Layers (Dark Mode):
├── Base: #000000 (pure black)
├── Surface: #16181C (cards, modals)
├── Elevated: #1D1F23 (hover states)
└── Borders: #2F3336 (dividers)

Background Layers (Light Mode):
├── Base: #FFFFFF (pure white)
├── Surface: #F7F9F9 (cards, sidebars)
├── Elevated: #EFF3F4 (hover states)
└── Borders: #EFF3F4 (dividers)
```

### Light Mode Variant
| Element | Light Mode | Dark Mode |
|---------|------------|-----------|
| Background | `#FFFFFF` | `#000000` |
| Primary Text | `#0F1419` | `#E7E9EA` |
| Secondary Text | `#536471` | `#71767B` |
| Borders | `#EFF3F4` | `#2F3336` |
| Cards | `#F7F9F9` | `#16181C` |

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
| Display (trending) | 31px | 800 | 36px | -0.5px |
| Heading Large | 23px | 700 | 28px | 0 |
| Heading Medium | 20px | 700 | 24px | 0 |
| Body | 15px | 400 | 20px | 0 |
| Body Bold | 15px | 700 | 20px | 0 |
| Caption | 13px | 400 | 16px | 0 |
| Small | 12px | 400 | 16px | 0.2px |
| Tiny | 11px | 400 | 14px | 0.2px |

### Typography Usage

#### Post Content
```css
.post-content {
  font-size: 15px;
  font-weight: 400;
  line-height: 20px;
  color: #E7E9EA; /* dark mode */
  word-wrap: break-word;
  white-space: pre-wrap;
}
```

#### Display Name
```css
.display-name {
  font-size: 15px;
  font-weight: 700;
  line-height: 20px;
  color: #E7E9EA;
}
```

#### Username/Handle
```css
.username {
  font-size: 15px;
  font-weight: 400;
  line-height: 20px;
  color: #71767B;
}
```

#### Timestamps
```css
.timestamp {
  font-size: 15px;
  font-weight: 400;
  color: #71767B;
}
```

### Special Text Treatments

#### Links & Mentions
- Color: `#1D9BF0` (X Blue)
- No underline by default
- Underline on hover
- Mentions (@) and hashtags (#) follow same styling

#### Quoted/Embedded Text
- Background: `#16181C` (dark mode)
- Border radius: 16px
- Padding: 12px
- Full width within post

---

## 4. Component Stylings

### Buttons

#### Primary Button (Blue)
```css
.btn-primary {
  background-color: #1D9BF0;
  color: #FFFFFF;
  font-size: 15px;
  font-weight: 700;
  padding: 0 16px;
  height: 36px;
  border-radius: 9999px;
  border: none;
  cursor: pointer;
  transition: background-color 0.2s;
}

.btn-primary:hover {
  background-color: #1A8CD8;
}

.btn-primary:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.btn-secondary {
  background-color: transparent;
  color: #E7E9EA;
  font-size: 15px;
  font-weight: 700;
  padding: 0 16px;
  height: 36px;
  border-radius: 9999px;
  border: 1px solid #536471;
  cursor: pointer;
  transition: background-color 0.2s, border-color 0.2s;
}

.btn-secondary:hover {
  background-color: rgba(239, 243, 244, 0.1);
  border-color: #E7E9EA;
}
```

#### Large Post Button
```css
.btn-post {
  background-color: #1D9BF0;
  color: #FFFFFF;
  font-size: 17px;
  font-weight: 700;
  padding: 0 32px;
  height: 52px;
  border-radius: 9999px;
  width: 100%; /* sidebar context */
}
```

### Post Card

```css
.post-card {
  background-color: transparent;
  border-bottom: 1px solid #2F3336;
  padding: 12px 16px;
  display: flex;
  gap: 12px;
  cursor: pointer;
  transition: background-color 0.2s;
}

.post-card:hover {
  background-color: rgba(255, 255, 255, 0.03);
}
```

### Avatar

```css
.avatar {
  width: 40px;
  height: 40px;
  border-radius: 9999px;
  object-fit: cover;
  flex-shrink: 0;
}

.avatar-large {
  width: 48px;
  height: 48px;
}

.avatar-profile {
  width: 134px;
  height: 134px;
  border: 4px solid #000000;
}
```

### Action Icons

```css
.action-icon {
  width: 34.75px;
  height: 34.75px;
  border-radius: 9999px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: background-color 0.2s, color 0.2s;
}

/* Reply */
.action-reply:hover {
  background-color: rgba(29, 155, 240, 0.1);
  color: #1D9BF0;
}

/* Repost */
.action-repost:hover {
  background-color: rgba(0, 186, 124, 0.1);
  color: #00BA7C;
}

/* Like */
.action-like:hover {
  background-color: rgba(249, 24, 128, 0.1);
  color: #F91880;
}

/* Bookmark */
.action-bookmark:hover {
  background-color: rgba(29, 155, 240, 0.1);
  color: #1D9BF0;
}

/* Share */
.action-share:hover {
  background-color: rgba(29, 155, 240, 0.1);
  color: #1D9BF0;
}
```

### Input Fields

```css
.input-field {
  background-color: transparent;
  border: 1px solid #333639;
  border-radius: 4px;
  padding: 12px;
  font-size: 17px;
  color: #E7E9EA;
  width: 100%;
  outline: none;
}

.input-field:focus {
  border-color: #1D9BF0;
  box-shadow: 0 0 0 1px #1D9BF0;
}

.input-field::placeholder {
  color: #71767B;
}
```

### Search Box

```css
.search-box {
  background-color: #202327;
  border: 1px solid transparent;
  border-radius: 9999px;
  padding: 12px 16px 12px 44px;
  font-size: 15px;
  color: #E7E9EA;
  width: 100%;
}

.search-box:focus {
  background-color: #000000;
  border-color: #1D9BF0;
}
```

### Modal/Dialog

```css
.modal-overlay {
  background-color: rgba(91, 112, 131, 0.4);
  position: fixed;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal-content {
  background-color: #000000;
  border-radius: 16px;
  max-width: 600px;
  max-height: 90vh;
  overflow-y: auto;
  box-shadow: 0 0 0 1px rgba(255, 255, 255, 0.15);
}
```

### Tabs

```css
.tab-item {
  padding: 16px;
  font-size: 15px;
  font-weight: 500;
  color: #71767B;
  border-bottom: 2px solid transparent;
  cursor: pointer;
  transition: background-color 0.2s;
}

.tab-item:hover {
  background-color: rgba(231, 233, 234, 0.1);
}

.tab-item.active {
  color: #E7E9EA;
  font-weight: 700;
  border-bottom-color: #1D9BF0;
}
```

### Verified Badge

```css
.verified-badge {
  width: 18px;
  height: 18px;
  margin-left: 2px;
  fill: #1D9BF0; /* Blue checkmark */
}

.verified-badge-gold {
  fill: #E2B719; /* Organizations */
}

.verified-badge-gray {
  fill: #829AAB; /* Government/Multilateral */
}
```

### Tooltips

```css
.tooltip {
  background-color: #5B7083;
  color: #FFFFFF;
  font-size: 12px;
  padding: 4px 8px;
  border-radius: 4px;
  max-width: 200px;
}
```

---

## 5. Layout Principles

### Three-Column Layout

```
┌─────────────────────────────────────────────────────────────┐
│                      Viewport (100%)                        │
├──────────┬─────────────────────────────┬───────────────────┤
│  Sidebar │        Main Feed            │   Right Sidebar   │
│  (275px) │        (600px)              │   (350px)         │
│          │                             │                   │
│  [Logo]  │  ┌─────────────────────┐   │  [Search]         │
│  [Nav]   │  │ What's happening?   │   │  [Trends]         │
│  [Post]  │  └─────────────────────┘   │  [Who to Follow]  │
│          │  ┌─────────────────────┐   │  [Premium]        │
│          │  │ Post Card           │   │                   │
│          │  │ ────────────────    │   │                   │
│          │  │ Post Card           │   │                   │
│          │  │ ────────────────    │   │                   │
│          │  │ Post Card           │   │                   │
│          │  └─────────────────────┘   │                   │
│          │                             │                   │
│  [User]  │                             │  [Footer Links]   │
└──────────┴─────────────────────────────┴───────────────────┘
```

### Grid Specifications

| Column | Width | Max Width | Min Width |
|--------|-------|-----------|-----------|
| Left Sidebar | 275px | 275px | 68px (collapsed) |
| Main Feed | 600px | 600px | 600px |
| Right Sidebar | 350px | 350px | 0 (hidden) |
| Total Content | 1225px | 1400px | 600px |

### Spacing System

```
Base Unit: 4px

Spacing Scale:
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
| Post card | 12px 16px |
| Navigation item | 12px |
| Section gap | 16px |
| Modal padding | 16px |
| Card internal | 12px |
| Icon spacing | 4px |

### Content Width Constraints

```css
.main-content {
  max-width: 600px;
  width: 100%;
  border-left: 1px solid #2F3336;
  border-right: 1px solid #2F3336;
  min-height: 100vh;
}

.sidebar-right {
  width: 350px;
  padding: 12px 24px;
}

.sidebar-left {
  width: 275px;
  padding: 0 8px;
  position: fixed;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
```

### Navigation Structure

```css
.nav-item {
  display: flex;
  align-items: center;
  gap: 20px;
  padding: 12px;
  border-radius: 9999px;
  font-size: 20px;
  font-weight: 400;
  color: #E7E9EA;
  transition: background-color 0.2s;
}

.nav-item:hover {
  background-color: rgba(231, 233, 234, 0.1);
}

.nav-item.active {
  font-weight: 700;
}
```

---

## 6. Depth & Elevation

### Elevation Levels

X uses a **flat design approach** with minimal shadows. Depth is communicated through:
1. **Background color changes** rather than shadows
2. **Border treatments** for separation
3. **Overlay opacity** for modals

### Surface Hierarchy (Dark Mode)

| Level | Background | Use Case |
|-------|------------|----------|
| 0 - Base | `#000000` | Main background |
| 1 - Surface | `#16181C` | Cards, widgets, sidebars |
| 2 - Elevated | `#1D1F23` | Hover states, dropdowns |
| 3 - Overlay | `rgba(91, 112, 131, 0.4)` | Modal backdrops |

### Shadow Usage

```css
/* Minimal shadow use - primarily for floating elements */
.dropdown-menu {
  background-color: #000000;
  border-radius: 12px;
  box-shadow: 
    0 0 0 1px rgba(255, 255, 255, 0.15),
    0 0 15px rgba(255, 255, 255, 0.1);
}

/* Image lightbox */
.media-viewer {
  background-color: rgba(0, 0, 0, 0.9);
}

/* Sticky header */
.header-blur {
  background-color: rgba(0, 0, 0, 0.65);
  backdrop-filter: blur(12px);
}
```

### Z-Index Scale

```
Navigation:     100
Sticky Header:  200
Dropdowns:      300
Tooltips:       400
Modal Overlay:  500
Modal Content:  600
Toast/Alerts:   700
```

### Border Treatments

```css
/* Primary dividers */
.divider {
  border-bottom: 1px solid #2F3336;
}

/* Card borders */
.card-border {
  border: 1px solid #2F3336;
}

/* Focus rings */
.focus-ring {
  box-shadow: 0 0 0 2px #1D9BF0;
}

/* Subtle glow on dropdowns */
.dropdown-glow {
  box-shadow: 0 0 0 1px rgba(255, 255, 255, 0.15);
}
```

### Animation & Transitions

```css
/* Standard transition */
.transition-default {
  transition: all 0.2s ease-out;
}

/* Button hover */
.transition-button {
  transition: background-color 0.2s ease;
}

/* Modal entrance */
@keyframes modal-enter {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Like animation */
@keyframes like-burst {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}
```

---

## 7. Do's and Don'ts

### DO's

#### Colors
- Use pure black (`#000000`) as the primary background in dark mode
- Apply X Blue (`#1D9BF0`) sparingly for interactive elements and links
- Maintain high contrast ratios (minimum 4.5:1 for text)
- Use semantic colors consistently (green for repost, pink for like)

#### Typography
- Stick to the system font stack for performance and native feel
- Use 15px as the base font size for body text
- Apply bold weight (700) for display names and emphasis
- Keep line height at 20px for comfortable reading

#### Components
- Use 9999px border-radius for all pill-shaped elements (buttons, avatars, tags)
- Keep action buttons icon-only with count beside them
- Provide clear hover states with subtle background color changes
- Use full-width layouts within the 600px content area

#### Layout
- Center the three-column layout on wide screens
- Fix the left sidebar for persistent navigation
- Use infinite scroll for timeline content
- Maintain consistent 12-16px padding on cards

#### Interactions
- Show loading states with subtle skeleton screens
- Provide immediate visual feedback on interactions
- Keep animations under 200ms for snappy feel
- Support keyboard navigation throughout

### DON'TS

#### Colors
- Don't use true gray backgrounds (avoid `#808080` mid-grays)
- Don't apply gradients anywhere in the UI
- Don't use colored backgrounds for cards or sections
- Don't deviate from the monochromatic + blue palette

#### Typography
- Don't use decorative or custom fonts
- Don't go below 11px for any text
- Don't use all-caps except for specific labels
- Don't center-align body text

#### Components
- Don't use shadows for elevation (use background colors instead)
- Don't add borders to buttons
- Don't use square corners on interactive elements
- Don't create custom icon styles (use consistent line icons)

#### Layout
- Don't exceed 600px for main content width
- Don't use multi-column layouts within the feed
- Don't implement horizontal scrolling for content
- Don't hide primary navigation

#### Interactions
- Don't use bounce or elastic animations
- Don't implement long-press as primary interaction (desktop)
- Don't auto-play videos with sound
- Don't use modals for simple confirmations

### Common Mistakes to Avoid

| Mistake | Correct Approach |
|---------|------------------|
| Adding card shadows | Use border-bottom dividers |
| Rounded corners at 8px | Use 16px for cards, 9999px for pills |
| Blue backgrounds | Keep blue for text/icons only |
| Dense information | Generous whitespace, clear hierarchy |
| Custom loading spinners | Use shimmer/skeleton patterns |

---

## 8. Responsive Behavior

### Breakpoint System

| Breakpoint | Width | Layout Changes |
|------------|-------|----------------|
| Desktop XL | ≥1400px | Full three-column, expanded nav labels |
| Desktop | 1100-1399px | Three-column, full nav |
| Tablet | 1005-1099px | Two-column, collapsed nav icons |
| Mobile L | 688-1004px | Single column with bottom nav |
| Mobile | <688px | Single column, compact UI |

### Desktop (≥1100px)
```
┌──────────────────────────────────────────────────┐
│ [Sidebar 275px] [Feed 600px] [Right Bar 350px]   │
│ - Full nav with labels                           │
│ - All three columns visible                      │
│ - Trending sidebar shown                         │
└──────────────────────────────────────────────────┘
```

### Tablet (1005-1099px)
```
┌──────────────────────────────────────────────────┐
│ [Sidebar 68px] [Feed 600px] [Right Bar 350px]    │
│ - Icons only navigation                          │
│ - X logo only (no wordmark)                      │
│ - Three columns, narrow sidebar                  │
└──────────────────────────────────────────────────┘
```

### Mobile Large (688-1004px)
```
┌──────────────────────────────────────────────────┐
│ [Sidebar 68px] [Feed 600px]                      │
│ - Right sidebar hidden                           │
│ - Icon navigation only                           │
│ - Trends moved to Explore tab                    │
└──────────────────────────────────────────────────┘
```

### Mobile (<688px)
```
┌─────────────────────────┐
│ [Header with menu]      │
│ [Feed full width]       │
│ [Bottom navigation]     │
│                         │
│ - Tab bar at bottom     │
│ - Hamburger menu        │
│ - FAB for compose       │
└─────────────────────────┘
```

### Mobile-Specific Components

#### Bottom Navigation Bar
```css
.bottom-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 53px;
  background-color: #000000;
  border-top: 1px solid #2F3336;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
```

#### Floating Compose Button
```css
.fab-compose {
  position: fixed;
  bottom: 80px;
  right: 16px;
  width: 56px;
  height: 56px;
  border-radius: 9999px;
  background-color: #1D9BF0;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
  display: flex;
  align-items: center;
  justify-content: center;
}
```

#### Mobile Header
```css
.mobile-header {
  position: sticky;
  top: 0;
  height: 53px;
  background-color: rgba(0, 0, 0, 0.65);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid #2F3336;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 16px;
}
```

### Touch Optimizations
- Minimum touch target: 44x44px
- Swipe gestures for navigation between tabs
- Pull-to-refresh on timeline
- Long-press for additional options menu
- Swipe actions on posts (experimental)

### Image Responsiveness
```css
.media-container {
  max-width: 100%;
  border-radius: 16px;
  overflow: hidden;
}

.media-container img {
  width: 100%;
  height: auto;
  max-height: 510px;
  object-fit: cover;
}
```

---

## 9. Agent Prompt Guide

### System Prompt for X-Style UI Generation

```
You are an AI assistant specialized in generating user interfaces that match X's (formerly Twitter) design system. Follow these specifications precisely:

VISUAL FOUNDATION:
- Use pure black (#000000) as primary background
- White (#E7E9EA) for primary text
- X Blue (#1D9BF0) for interactive elements and links only
- Gray (#71767B) for secondary text and placeholders
- Border gray (#2F3336) for all dividers

TYPOGRAPHY:
- System font stack: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto
- Base size: 15px
- Line height: 20px
- Bold (700) for names and emphasis
- Regular (400) for body content

COMPONENT PATTERNS:
- Buttons: Pill-shaped (border-radius: 9999px)
- Cards: Subtle borders, no shadows
- Avatars: Perfect circles (border-radius: 9999px)
- Icons: Line style, 18-24px
- Inputs: Minimal borders, blue focus states

LAYOUT RULES:
- Max content width: 600px
- Card padding: 12px 16px
- Consistent 4px spacing grid
- Border-based elevation only

INTERACTION STATES:
- Hover: Subtle background (#1D1F23)
- Active: Slightly darker
- Focus: Blue ring (#1D9BF0)
- Disabled: 50% opacity
```

### Component Generation Prompts

#### Generate a Post Card
```
Create a post card component with:
- 40px circular avatar on the left
- Display name (bold) and @username (gray) on same line
- Timestamp with "· Xh" format
- Body text at 15px
- Action bar with reply, repost, like, bookmark, share icons
- Hover state with subtle gray background
- Bottom border divider
```

#### Generate a Profile Header
```
Create a profile header with:
- Banner image (200px height, full width)
- Circular avatar (134px) overlapping banner
- Display name with verified badge
- @username in gray
- Bio text (15px)
- Following/Followers counts
- Follow/Following button (pill-shaped)
```

#### Generate Navigation Sidebar
```
Create a navigation sidebar with:
- X logo at top (28px)
- Vertical nav items with icons (24px) and labels
- Items: Home, Explore, Notifications, Messages, Grok, Lists, Bookmarks, Communities, Premium, Verified Orgs, Profile, More
- Full-width Post button at bottom
- User profile summary at very bottom
- Pill-shaped hover states
```

### Color Usage Quick Reference

```
When to use X Blue (#1D9BF0):
- Links and mentions
- Primary buttons
- Focus states
- Selected tab indicators
- Follow button

When to use Pure Black (#000000):
- Page backgrounds
- Modal backgrounds
- Input backgrounds (focused)

When to use Gray (#71767B):
- Timestamps
- Usernames (@handles)
- Placeholder text
- Secondary information
- Disabled states

When to use White (#E7E9EA):
- Display names
- Post content
- Button text
- Headlines
- Active icons
```

### Semantic Action Colors

```
Reply action: #1D9BF0 (blue)
Repost action: #00BA7C (green)
Like action: #F91880 (pink)
Bookmark action: #1D9BF0 (blue)
Share action: #1D9BF0 (blue)
Delete/Error: #F4212E (red)
```

### Common UI Patterns

```
Loading States:
- Use skeleton screens with #2F3336 animated bars
- Pulse animation at 1.5s intervals
- Match exact content layout

Empty States:
- Large icon (48px) centered
- Bold headline
- Gray descriptive text
- Optional blue CTA button

Error States:
- Red accent (#F4212E) for alerts
- Keep messaging concise
- Provide retry actions

Success States:
- Minimal celebration
- Quick toast notifications
- Auto-dismiss after 3s
```

---

## Quick Reference Card

| Element | Value |
|---------|-------|
| Primary Background | `#000000` |
| Primary Text | `#E7E9EA` |
| Accent Blue | `#1D9BF0` |
| Secondary Text | `#71767B` |
| Borders | `#2F3336` |
| Font Family | System fonts |
| Base Font Size | 15px |
| Button Radius | 9999px |
| Card Radius | 16px |
| Content Width | 600px |
| Avatar Size | 40px |
| Icon Size | 18-24px |
| Spacing Unit | 4px |

---

*Last updated: 2024-2026 Design System*
*Based on X (formerly Twitter) web and mobile applications*
