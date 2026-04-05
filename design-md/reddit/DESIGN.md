# Reddit Design System

> Community-driven social platform with card-based content, threaded discussions, and the iconic orangered accent. Clean, scannable, and built for endless scrolling.

---

## 1. Visual Theme & Atmosphere

### Design Philosophy
Reddit's design balances **community identity** with **content accessibility**. The interface prioritizes readability and scanability, enabling users to browse massive amounts of user-generated content efficiently. Every element serves the core purpose: facilitating discussion and discovery.

### Mood & Character
| Attribute | Description |
|-----------|-------------|
| **Tone** | Casual, democratic, community-driven |
| **Energy** | Active, participatory, always-updating |
| **Personality** | Approachable (Snoo mascot), opinionated (voting system), tribal (subreddits) |
| **Visual density** | Medium-high; content-rich but organized into digestible cards |

### Brand Identity
- **Snoo**: The alien mascot appears throughout, customizable per subreddit
- **Orangered**: The iconic upvote color, synonymous with Reddit itself
- **Periwinkle**: The downvote color, creating the signature voting duality
- **Community badges**: Awards and flair create visual hierarchy and engagement

### Design Principles
1. **Content first**: Posts and comments are the heroes; UI stays out of the way
2. **Community identity**: Each subreddit can express its own personality
3. **Democratic design**: Upvotes/downvotes visually represent collective opinion
4. **Scanability**: Card layouts enable rapid browsing of diverse content
5. **Threading clarity**: Comment hierarchies must be instantly readable

---

## 2. Color Palette & Roles

### Light Mode

| Name | Hex | RGB | Role |
|------|-----|-----|------|
| **Orangered** | `#FF4500` | 255, 69, 0 | Primary brand, upvotes, CTAs |
| **Periwinkle** | `#7193FF` | 113, 147, 255 | Downvotes, secondary accent |
| **Reddit Blue** | `#0079D3` | 0, 121, 211 | Links, interactive elements |
| **Canvas** | `#DAE0E6` | 218, 224, 230 | Page background |
| **Card White** | `#FFFFFF` | 255, 255, 255 | Content cards, surfaces |
| **Text Primary** | `#1C1C1C` | 28, 28, 28 | Headlines, body text |
| **Text Secondary** | `#7C7C7C` | 124, 124, 124 | Metadata, timestamps |
| **Text Tertiary** | `#878A8C` | 135, 138, 140 | Placeholders, hints |
| **Border** | `#EDEFF1` | 237, 239, 241 | Card borders, dividers |
| **Online Green** | `#46D160` | 70, 209, 96 | Online indicators, success |
| **Gold** | `#FFD635` | 255, 214, 53 | Awards, premium features |
| **Silver** | `#C4C4C4` | 196, 196, 196 | Silver award |
| **Platinum** | `#A0E8FF` | 160, 232, 255 | Platinum award |

### Dark Mode

| Name | Hex | RGB | Role |
|------|-----|-----|------|
| **Orangered** | `#FF4500` | 255, 69, 0 | Primary brand, upvotes (unchanged) |
| **Periwinkle** | `#7193FF` | 113, 147, 255 | Downvotes (unchanged) |
| **Reddit Blue** | `#4FBCFF` | 79, 188, 255 | Links (brighter for dark bg) |
| **Canvas** | `#030303` | 3, 3, 3 | Page background |
| **Card Dark** | `#1A1A1B` | 26, 26, 27 | Content cards, surfaces |
| **Elevated Surface** | `#272729` | 39, 39, 41 | Modals, dropdowns, hovers |
| **Text Primary** | `#D7DADC` | 215, 218, 220 | Headlines, body text |
| **Text Secondary** | `#818384` | 129, 131, 132 | Metadata, timestamps |
| **Text Tertiary** | `#6B6C6D` | 107, 108, 109 | Placeholders, hints |
| **Border** | `#343536` | 52, 53, 54 | Card borders, dividers |
| **Online Green** | `#46D160` | 70, 209, 96 | Online indicators (unchanged) |

### Semantic Color Usage

```
Upvote active:     #FF4500 (orangered)
Upvote inactive:   #D5D7D9 (light) / #818384 (dark)
Downvote active:   #7193FF (periwinkle)
Downvote inactive: #D5D7D9 (light) / #818384 (dark)
Link:              #0079D3 (light) / #4FBCFF (dark)
Link hover:        #0066B3 (light) / #6ECAFF (dark)
Error:             #FF0000
Warning:           #FFB000
Success:           #46D160
Moderator:         #46D160 (green shield)
Admin:             #FF4500 (red shield)
OP highlight:      #0079D3 (light) / #4FBCFF (dark)
Cake day:          #FF4500 (cake icon)
```

---

## 3. Typography Rules

### Font Stack

| Use | Family | Fallback |
|-----|--------|----------|
| **Headings** | IBM Plex Sans | -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif |
| **Body** | -apple-system, BlinkMacSystemFont | Segoe UI, Roboto, Helvetica Neue, sans-serif |
| **Code** | Source Code Pro | Menlo, Monaco, Consolas, monospace |
| **Brand/Logo** | Reddit Sans (custom) | IBM Plex Sans |

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| **Page title** | 24px | 700 | 28px | -0.02em |
| **Post title** | 18px | 500 | 22px | 0 |
| **Post title (compact)** | 14px | 500 | 18px | 0 |
| **Subreddit name** | 16px | 700 | 20px | 0 |
| **Body text** | 14px | 400 | 21px | 0 |
| **Comment text** | 14px | 400 | 21px | 0 |
| **Metadata** | 12px | 400 | 16px | 0 |
| **Button text** | 14px | 700 | 17px | 0.5px |
| **Nav item** | 14px | 500 | 18px | 0 |
| **Flair text** | 12px | 500 | 14px | 0 |
| **Tiny/caption** | 10px | 400 | 12px | 0.3px |

### Typography Rules
- **Post titles**: Medium weight (500), never exceed 2 lines in card view
- **Usernames**: Always prefixed with `u/`, linked, 12px
- **Subreddit names**: Always prefixed with `r/`, linked, bold
- **Timestamps**: Relative time preferred ("2h ago", "3d"), 12px, secondary color
- **Karma counts**: Abbreviated format (1.2k, 15.6k, 2.3m)
- **Code blocks**: Monospace, light gray background, 13px
- **Blockquotes**: Left border accent, indented

---

## 4. Component Stylings

### Buttons

#### Primary Button (Orangered)
```css
.btn-primary {
  background: #FF4500;
  color: #FFFFFF;
  font-weight: 700;
  font-size: 14px;
  padding: 8px 16px;
  border-radius: 9999px;  /* Full pill shape */
  border: none;
  min-width: 80px;
  min-height: 32px;
}
.btn-primary:hover {
  background: #E63E00;
}
.btn-primary:active {
  background: #CC3700;
}
.btn-primary:disabled {
  background: #FF4500;
  opacity: 0.5;
}
```

#### Secondary Button (Outlined)
```css
.btn-secondary {
  background: transparent;
  color: #0079D3;
  font-weight: 700;
  font-size: 14px;
  padding: 8px 16px;
  border-radius: 9999px;
  border: 1px solid #0079D3;
  min-height: 32px;
}
.btn-secondary:hover {
  background: rgba(0, 121, 211, 0.1);
}
/* Dark mode */
.dark .btn-secondary {
  color: #4FBCFF;
  border-color: #4FBCFF;
}
```

#### Icon Button
```css
.btn-icon {
  background: transparent;
  color: #878A8C;
  padding: 8px;
  border-radius: 4px;
  border: none;
}
.btn-icon:hover {
  background: rgba(0, 0, 0, 0.05);
  color: #1C1C1C;
}
/* Dark mode */
.dark .btn-icon:hover {
  background: rgba(255, 255, 255, 0.1);
  color: #D7DADC;
}
```

### Upvote/Downvote System

```css
.vote-button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 24px;
  height: 24px;
  padding: 4px;
  border-radius: 2px;
  color: #878A8C;
}

.vote-button:hover {
  background: rgba(0, 0, 0, 0.05);
}

.vote-button.upvote.active {
  color: #FF4500;
}

.vote-button.downvote.active {
  color: #7193FF;
}

.vote-count {
  font-size: 12px;
  font-weight: 700;
  min-width: 32px;
  text-align: center;
}

.vote-count.upvoted {
  color: #FF4500;
}

.vote-count.downvoted {
  color: #7193FF;
}
```

### Post Card

```css
.post-card {
  background: #FFFFFF;
  border: 1px solid #EDEFF1;
  border-radius: 4px;
  margin-bottom: 10px;
  overflow: hidden;
}

/* Dark mode */
.dark .post-card {
  background: #1A1A1B;
  border-color: #343536;
}

.post-card:hover {
  border-color: #898989;
}

.dark .post-card:hover {
  border-color: #818384;
}

/* Card layout */
.post-card-content {
  display: flex;
}

.post-vote-column {
  width: 40px;
  padding: 8px 4px;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #F8F9FA;
}

.dark .post-vote-column {
  background: #161617;
}

.post-main-content {
  flex: 1;
  padding: 8px;
}
```

### Comment Thread

```css
.comment {
  padding: 8px 0 8px 8px;
}

.comment-thread {
  margin-left: 8px;
  padding-left: 16px;
  border-left: 2px solid #EDEFF1;
}

.dark .comment-thread {
  border-left-color: #343536;
}

/* Thread collapse line - hover state */
.comment-thread:hover {
  border-left-color: #0079D3;
}

.dark .comment-thread:hover {
  border-left-color: #4FBCFF;
}

/* Collapsed comment */
.comment.collapsed {
  opacity: 0.6;
}

.comment-body {
  font-size: 14px;
  line-height: 21px;
  color: #1C1C1C;
}

.dark .comment-body {
  color: #D7DADC;
}
```

### Avatar & User Icons

```css
.avatar {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background: #EDEFF1;
  overflow: hidden;
}

.avatar-small {
  width: 24px;
  height: 24px;
}

.avatar-large {
  width: 80px;
  height: 80px;
}

/* Community icon */
.community-icon {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  border: 4px solid #FFFFFF;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.1);
}

.dark .community-icon {
  border-color: #1A1A1B;
}

/* Community banner avatar (profile overlap) */
.community-icon-banner {
  width: 80px;
  height: 80px;
  margin-top: -40px;
  border-width: 4px;
}
```

### Awards & Badges

```css
.award {
  display: inline-flex;
  align-items: center;
  gap: 2px;
  font-size: 12px;
  color: #878A8C;
}

.award-icon {
  width: 16px;
  height: 16px;
}

/* Award colors */
.award-gold {
  color: #FFD635;
}

.award-silver {
  color: #C4C4C4;
}

.award-platinum {
  color: #A0E8FF;
}

.award-helpful {
  color: #FF4500;
}

/* Flair badges */
.flair {
  display: inline-block;
  padding: 2px 6px;
  border-radius: 9999px;
  font-size: 12px;
  font-weight: 500;
  line-height: 14px;
}

.flair-user {
  background: #EDEFF1;
  color: #1C1C1C;
}

.dark .flair-user {
  background: #272729;
  color: #D7DADC;
}

/* Post flair with custom colors */
.flair-post {
  background: var(--flair-bg, #EDEFF1);
  color: var(--flair-color, #1C1C1C);
}

/* Moderator flair */
.flair-mod {
  background: #46D160;
  color: #FFFFFF;
}
```

### Input Fields

```css
.input {
  width: 100%;
  padding: 8px 12px;
  font-size: 14px;
  border: 1px solid #EDEFF1;
  border-radius: 4px;
  background: #F6F7F8;
  color: #1C1C1C;
}

.dark .input {
  background: #272729;
  border-color: #343536;
  color: #D7DADC;
}

.input:focus {
  outline: none;
  border-color: #0079D3;
  background: #FFFFFF;
}

.dark .input:focus {
  border-color: #4FBCFF;
  background: #1A1A1B;
}

/* Search bar */
.search-bar {
  background: #F6F7F8;
  border: 1px solid #EDEFF1;
  border-radius: 9999px;
  padding: 6px 16px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.search-bar:focus-within {
  border-color: #0079D3;
  background: #FFFFFF;
}

/* Create post prompt */
.create-post-input {
  background: #F6F7F8;
  border: 1px solid #EDEFF1;
  border-radius: 4px;
  padding: 8px 16px;
  width: 100%;
  cursor: pointer;
}

.create-post-input:hover {
  border-color: #0079D3;
  background: #FFFFFF;
}
```

### Navigation

```css
/* Top nav bar */
.navbar {
  height: 48px;
  background: #FFFFFF;
  border-bottom: 1px solid #EDEFF1;
  display: flex;
  align-items: center;
  padding: 0 20px;
  position: sticky;
  top: 0;
  z-index: 100;
}

.dark .navbar {
  background: #1A1A1B;
  border-bottom-color: #343536;
}

/* Subreddit tabs */
.subreddit-tabs {
  display: flex;
  gap: 8px;
  padding: 12px 16px;
  border-bottom: 1px solid #EDEFF1;
  background: #FFFFFF;
}

.dark .subreddit-tabs {
  background: #1A1A1B;
  border-bottom-color: #343536;
}

.tab {
  padding: 8px 12px;
  border-radius: 9999px;
  font-size: 14px;
  font-weight: 700;
  color: #878A8C;
  cursor: pointer;
}

.tab:hover {
  background: rgba(0, 0, 0, 0.05);
}

.tab.active {
  background: rgba(0, 121, 211, 0.1);
  color: #0079D3;
}

.dark .tab.active {
  background: rgba(79, 188, 255, 0.1);
  color: #4FBCFF;
}
```

### Dropdown & Menus

```css
.dropdown {
  background: #FFFFFF;
  border: 1px solid #EDEFF1;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  min-width: 200px;
  overflow: hidden;
}

.dark .dropdown {
  background: #1A1A1B;
  border-color: #343536;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}

.dropdown-item {
  padding: 12px 16px;
  font-size: 14px;
  color: #1C1C1C;
  cursor: pointer;
}

.dark .dropdown-item {
  color: #D7DADC;
}

.dropdown-item:hover {
  background: #F6F7F8;
}

.dark .dropdown-item:hover {
  background: #272729;
}

.dropdown-divider {
  height: 1px;
  background: #EDEFF1;
  margin: 4px 0;
}

.dark .dropdown-divider {
  background: #343536;
}
```

### Modal

```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.4);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}

.modal {
  background: #FFFFFF;
  border-radius: 4px;
  max-width: 538px;
  width: 100%;
  max-height: 90vh;
  overflow: hidden;
}

.dark .modal {
  background: #1A1A1B;
}

.modal-header {
  padding: 16px;
  border-bottom: 1px solid #EDEFF1;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.dark .modal-header {
  border-bottom-color: #343536;
}

.modal-body {
  padding: 16px;
  overflow-y: auto;
}

.modal-footer {
  padding: 16px;
  border-top: 1px solid #EDEFF1;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
}

.dark .modal-footer {
  border-top-color: #343536;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-0` | 0px | Reset |
| `--space-1` | 4px | Tight inline spacing |
| `--space-2` | 8px | Icon padding, compact gaps |
| `--space-3` | 12px | Card inner padding |
| `--space-4` | 16px | Standard component padding |
| `--space-5` | 20px | Section padding |
| `--space-6` | 24px | Card gaps, medium spacing |
| `--space-7` | 32px | Large gaps |
| `--space-8` | 40px | Section dividers |
| `--space-9` | 48px | Header height |
| `--space-10` | 64px | Major section breaks |

### Grid System

```css
/* Classic Reddit layout */
.reddit-layout {
  display: grid;
  grid-template-columns: 1fr minmax(auto, 640px) 312px 1fr;
  gap: 24px;
  max-width: 1280px;
  margin: 0 auto;
  padding: 20px 24px;
}

/* Feed takes center, sidebar on right */
.feed-column {
  grid-column: 2;
}

.sidebar-column {
  grid-column: 3;
}

/* Full-width mode (comments page) */
.reddit-layout-fullwidth {
  grid-template-columns: 1fr minmax(auto, 740px) 312px 1fr;
}
```

### Card Spacing

```css
.post-card {
  margin-bottom: 10px;
}

.post-card-padding {
  padding: 8px;
}

.comment-padding {
  padding: 8px 0 8px 8px;
}

/* Thread indentation */
.thread-indent {
  margin-left: 8px;
  padding-left: 16px;
}
```

### Container Widths

| Context | Width | Notes |
|---------|-------|-------|
| **Feed container** | 640px | Max width for post cards |
| **Sidebar** | 312px | Fixed width |
| **Modal** | 538px | Standard modal |
| **Full page max** | 1280px | Outer container limit |
| **Compact card** | 100% | Card view uses full feed width |

### Whitespace Philosophy
- **Breathing room**: Cards have clear separation, never touching
- **Scanability**: Consistent vertical rhythm for quick browsing
- **Hierarchy**: More space above major sections, less between related items
- **Information density**: Balance between readability and content amount

---

## 6. Depth & Elevation

### Shadow System

| Level | Value | Usage |
|-------|-------|-------|
| **Flat** | none | Default cards, inline elements |
| **Hover** | `0 2px 4px rgba(0, 0, 0, 0.08)` | Card hover, button hover |
| **Dropdown** | `0 2px 4px rgba(0, 0, 0, 0.12)` | Menus, popovers |
| **Modal** | `0 4px 12px rgba(0, 0, 0, 0.15)` | Modal dialogs |
| **Sticky** | `0 2px 8px rgba(0, 0, 0, 0.08)` | Sticky headers |

### Dark Mode Shadows

```css
/* Shadows are more subtle in dark mode */
.dark .shadow-hover {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
}

.dark .shadow-dropdown {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}

.dark .shadow-modal {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.6);
}
```

### Surface Hierarchy

| Surface | Light | Dark | Usage |
|---------|-------|------|-------|
| **Page** | `#DAE0E6` | `#030303` | Background canvas |
| **Card** | `#FFFFFF` | `#1A1A1B` | Post cards, widgets |
| **Elevated** | `#FFFFFF` | `#272729` | Dropdowns, modals, hovers |
| **Inset** | `#F6F7F8` | `#161617` | Vote column, input backgrounds |
| **Overlay** | `rgba(0,0,0,0.4)` | `rgba(0,0,0,0.7)` | Modal backdrop |

### Z-Index Scale

| Layer | Value | Usage |
|-------|-------|-------|
| **Base** | 0 | Standard content |
| **Raised** | 10 | Sticky elements on scroll |
| **Dropdown** | 50 | Dropdown menus |
| **Sticky nav** | 100 | Top navigation bar |
| **Modal** | 1000 | Modal dialogs |
| **Toast** | 1100 | Toast notifications |
| **Tooltip** | 1200 | Tooltips |

---

## 7. Do's and Don'ts

### Do's

| Category | Guideline |
|----------|-----------|
| **Color** | Use orangered (#FF4500) exclusively for upvotes, primary CTAs, and brand moments |
| **Color** | Maintain high contrast between text and background (4.5:1 minimum) |
| **Typography** | Abbreviate large numbers (1.2k, 15.6k, 2.3m) for karma and counts |
| **Typography** | Use relative timestamps ("2h ago") not absolute dates |
| **Components** | Keep buttons fully rounded (pill shape) for primary actions |
| **Components** | Preserve vote button spacing in the left column of cards |
| **Layout** | Maintain the 640px max-width for readable post content |
| **Layout** | Use thread lines to visually connect nested comments |
| **Branding** | Allow Snoo to be customizable per community |
| **Interaction** | Animate vote color changes smoothly |

### Don'ts

| Category | Anti-pattern |
|----------|-------------|
| **Color** | Never use orangered for negative actions (delete, error) |
| **Color** | Don't use periwinkle blue for anything except downvotes |
| **Typography** | Avoid full timestamps in feeds; save them for detail views |
| **Typography** | Don't make post titles smaller than 14px even in compact mode |
| **Components** | Never hide the voting UI; it's core to Reddit's identity |
| **Components** | Don't break comment thread indentation visually |
| **Layout** | Avoid full-width cards; maintain readable line lengths |
| **Layout** | Don't let sidebar width compress below 300px |
| **Branding** | Never use a non-circular shape for avatars/community icons |
| **Interaction** | Don't remove hover states; users expect interactivity feedback |

### Accessibility Requirements
- All interactive elements must have visible focus states
- Vote buttons must have aria-labels ("Upvote", "Downvote")
- Color alone should not convey information (use icons alongside)
- Minimum touch target: 44x44px on mobile
- Support reduced motion preferences for animations

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| **Desktop XL** | ≥1280px | Full layout with sidebar |
| **Desktop** | 960–1279px | Full layout, narrower margins |
| **Tablet** | 768–959px | Sidebar collapses to dropdown or hidden |
| **Mobile** | 640–767px | Single column, bottom nav |
| **Mobile S** | <640px | Compact cards, minimal chrome |

### Responsive Grid Changes

```css
/* Desktop: Full 3-column */
@media (min-width: 960px) {
  .reddit-layout {
    grid-template-columns: 1fr 640px 312px 1fr;
  }
}

/* Tablet: No sidebar */
@media (max-width: 959px) {
  .reddit-layout {
    grid-template-columns: 1fr minmax(auto, 640px) 1fr;
  }
  
  .sidebar-column {
    display: none;
  }
}

/* Mobile: Single column */
@media (max-width: 767px) {
  .reddit-layout {
    grid-template-columns: 1fr;
    padding: 0;
    gap: 0;
  }
  
  .post-card {
    border-radius: 0;
    border-left: none;
    border-right: none;
    margin-bottom: 8px;
  }
}
```

### Touch Adaptations

| Element | Desktop | Mobile |
|---------|---------|--------|
| **Vote buttons** | 24x24px | 44x44px tap target |
| **Action buttons** | Icon only | Icon + larger tap area |
| **Comment collapse** | Click thread line | Tap collapse button |
| **Navigation** | Top bar | Bottom tab bar |
| **Create post** | Inline prompt | FAB or bottom bar button |

### Mobile-Specific Components

```css
/* Bottom navigation (mobile) */
.bottom-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 56px;
  background: #FFFFFF;
  border-top: 1px solid #EDEFF1;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-bottom: env(safe-area-inset-bottom);
}

.dark .bottom-nav {
  background: #1A1A1B;
  border-top-color: #343536;
}

/* Mobile card adjustments */
@media (max-width: 767px) {
  .post-vote-column {
    width: 32px;
    padding: 4px;
  }
  
  .vote-button {
    width: 32px;
    height: 32px;
  }
}
```

### Content Collapsing Strategy
1. **960px**: Sidebar disappears, community info moves to expandable header
2. **768px**: Header simplifies, some nav items move to hamburger menu
3. **640px**: Cards go full-bleed, compact view enabled by default
4. **480px**: Further simplify card metadata, stack action buttons

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
Brand Color:       #FF4500 (Orangered)
Secondary:         #7193FF (Periwinkle/downvote)
Link Color:        #0079D3 (light) / #4FBCFF (dark)
Background Light:  #DAE0E6
Background Dark:   #030303
Card Light:        #FFFFFF
Card Dark:         #1A1A1B
Text Light:        #1C1C1C
Text Dark:         #D7DADC
Border Light:      #EDEFF1
Border Dark:       #343536
Success/Online:    #46D160
Gold Award:        #FFD635

Font Primary:      IBM Plex Sans, system-ui
Font Body:         -apple-system, system fonts
Border Radius:     4px (cards), 9999px (pills/avatars)
Card Gap:          10px
Thread Indent:     24px (8px margin + 16px padding)
Feed Width:        640px max
Sidebar Width:     312px
```

### Component Prompt Templates

#### Post Card
```
Create a Reddit-style post card with:
- Left vote column (40px) with upvote/downvote arrows and score
- Vote column has #F8F9FA background (light) or #161617 (dark)
- Main content area with 8px padding
- Subreddit name (r/name), poster (u/name), timestamp in metadata row
- Post title in 18px medium weight
- Optional thumbnail or media preview
- Action bar: comments count, share, save, award, more
- 4px border-radius, 1px #EDEFF1 border
- Hover: border color changes to #898989
```

#### Comment Thread
```
Create a Reddit comment with:
- Avatar (24px circle) + username (12px, link color) + flair + timestamp
- Comment body in 14px/21px line height
- Action row: upvote/score/downvote, reply, share, award, more
- Nested replies indented with 2px left border (#EDEFF1)
- Thread indent: 8px margin-left + 16px padding-left
- Thread line hover turns #0079D3
- Collapse UI: clicking thread line collapses children
```

#### Upvote/Downvote UI
```
Create Reddit voting arrows:
- Upvote: arrow icon, #878A8C default, #FF4500 when active
- Downvote: arrow icon, #878A8C default, #7193FF when active
- Score between arrows in 12px bold
- Score color matches active vote direction
- Vertical layout with 4px gap
- Subtle background on hover (rgba(0,0,0,0.05))
- Smooth color transition on click
```

#### Community Sidebar Widget
```
Create a subreddit info widget:
- Community icon (80px circle) overlapping banner
- Community name (r/name) in 16px bold
- Member count + online count with green dot
- Description text
- Join button (full-width, orangered, pill shape)
- Create Post button (secondary, outlined)
- Rules section collapsible
- Moderators section at bottom
- White card, 4px radius, 1px border
```

### Full Page Prompt

```
Create a Reddit homepage feed with:

HEADER:
- 48px sticky nav bar
- Reddit logo (Snoo + wordmark) left
- Search bar center (pill shape, #F6F7F8 bg)
- User actions right: create post, notifications, chat, profile avatar

LAYOUT:
- Canvas background #DAE0E6
- Center column 640px max for post cards
- Right sidebar 312px for widgets
- 24px gap between columns

FEED:
- Sort tabs at top: Hot, New, Top, Rising (pill buttons)
- Post cards stacked with 10px gap
- Each card has vote column + content area
- Infinite scroll pattern

SIDEBAR WIDGETS:
- Community Info (if on subreddit)
- Premium promo card
- Popular communities list
- Reddit Links/policies footer

Support both light mode (default) and dark mode toggle.
```

### Animation Guidelines

```css
/* Standard transitions */
--transition-fast: 150ms ease;
--transition-normal: 200ms ease;
--transition-slow: 300ms ease-out;

/* Vote color change */
.vote-button {
  transition: color var(--transition-fast);
}

/* Card hover */
.post-card {
  transition: border-color var(--transition-fast);
}

/* Dropdown open */
.dropdown {
  animation: fadeIn var(--transition-normal);
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(-4px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Comment collapse */
.comment-collapse {
  transition: height var(--transition-normal),
              opacity var(--transition-fast);
}
```

### Dark Mode Implementation

```css
/* Apply dark mode via class on root or body */
.dark {
  --bg-canvas: #030303;
  --bg-card: #1A1A1B;
  --bg-elevated: #272729;
  --bg-inset: #161617;
  --text-primary: #D7DADC;
  --text-secondary: #818384;
  --text-tertiary: #6B6C6D;
  --border-color: #343536;
  --link-color: #4FBCFF;
}

/* Light mode (default) */
:root {
  --bg-canvas: #DAE0E6;
  --bg-card: #FFFFFF;
  --bg-elevated: #FFFFFF;
  --bg-inset: #F6F7F8;
  --text-primary: #1C1C1C;
  --text-secondary: #7C7C7C;
  --text-tertiary: #878A8C;
  --border-color: #EDEFF1;
  --link-color: #0079D3;
}

/* Brand colors stay constant */
:root {
  --orangered: #FF4500;
  --periwinkle: #7193FF;
  --online-green: #46D160;
  --gold: #FFD635;
}
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024 | Initial Reddit design system documentation |

---

*This DESIGN.md captures Reddit's visual design system for AI agents to generate consistent, on-brand UI components. The orangered accent, card-based layout, threading system, and democratic voting UI are signature elements that define the Reddit experience.*
