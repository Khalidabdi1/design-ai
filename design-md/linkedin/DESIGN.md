# LinkedIn Design System

## 1. Color Palette

### Primary Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| LinkedIn Blue | `#0A66C2` | `rgb(10, 102, 194)` | Primary brand color, CTAs, links, active states |
| Light Blue | `#70B5F9` | `rgb(112, 181, 249)` | Hover states, secondary accents, skill badges |
| Dark Blue | `#004182` | `rgb(0, 65, 130)` | Pressed states, emphasis, premium features |

### Neutral Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| Black | `#000000` | `rgb(0, 0, 0)` | Primary text (with opacity) |
| Black 90% | `#000000E6` | `rgba(0, 0, 0, 0.9)` | Primary body text |
| Black 60% | `#00000099` | `rgba(0, 0, 0, 0.6)` | Secondary text, timestamps |
| Black 40% | `#00000066` | `rgba(0, 0, 0, 0.4)` | Placeholder text, disabled states |
| White | `#FFFFFF` | `rgb(255, 255, 255)` | Backgrounds, cards, modals |
| Light Gray | `#F3F2EF` | `rgb(243, 242, 239)` | Page background, section dividers |
| Border Gray | `#E0DFDC` | `rgb(224, 223, 220)` | Card borders, dividers |

### Semantic Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| Success Green | `#057642` | `rgb(5, 118, 66)` | Success states, online indicators |
| Light Green | `#7FC15E` | `rgb(127, 193, 94)` | Open to work banner, growth indicators |
| Warning Orange | `#B24020` | `rgb(178, 64, 32)` | Error states, urgent notifications |
| Premium Gold | `#C37D16` | `rgb(195, 125, 22)` | LinkedIn Premium features |

### Gradient Definitions
```css
/* Premium Gold Gradient */
background: linear-gradient(135deg, #E7A33E 0%, #C37D16 50%, #8B5A0B 100%);

/* Professional Blue Gradient (Cards) */
background: linear-gradient(180deg, #0A66C2 0%, #004182 100%);

/* Hover State Gradient */
background: linear-gradient(180deg, rgba(10, 102, 194, 0.08) 0%, rgba(10, 102, 194, 0) 100%);
```

---

## 2. Typography

### Font Stack
```css
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;
```

### Type Scale
| Style | Size | Weight | Line Height | Letter Spacing | Usage |
|-------|------|--------|-------------|----------------|-------|
| Display Large | 32px | 600 | 40px | -0.5px | Profile names (hero) |
| Display Medium | 24px | 600 | 32px | -0.25px | Section headings |
| Heading Large | 20px | 600 | 28px | 0 | Card titles, job titles |
| Heading Medium | 18px | 600 | 24px | 0 | Subheadings |
| Heading Small | 16px | 600 | 22px | 0 | Component headers |
| Body Large | 16px | 400 | 24px | 0 | Post content |
| Body Medium | 14px | 400 | 20px | 0 | Primary body text |
| Body Small | 12px | 400 | 16px | 0.1px | Secondary text, metadata |
| Caption | 11px | 400 | 14px | 0.2px | Timestamps, helper text |
| Overline | 12px | 600 | 16px | 1px | Labels, categories |

### Font Weights
| Weight | Value | Usage |
|--------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Emphasized text, subtitles |
| Semibold | 600 | Headings, names, CTAs |
| Bold | 700 | Strong emphasis (rare) |

### Text Colors
| Type | Color | Opacity | Usage |
|------|-------|---------|-------|
| Primary | `#000000` | 90% | Headlines, body text |
| Secondary | `#000000` | 60% | Timestamps, secondary info |
| Tertiary | `#000000` | 40% | Placeholders, disabled |
| Link | `#0A66C2` | 100% | Clickable text, hashtags |
| Inverse | `#FFFFFF` | 100% | Text on dark backgrounds |

---

## 3. Spacing System

### Base Unit
Base unit: **4px**

### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `spacing-0` | 0px | No spacing |
| `spacing-1` | 4px | Tight inline spacing, icon gaps |
| `spacing-2` | 8px | Compact component padding |
| `spacing-3` | 12px | Standard inline spacing |
| `spacing-4` | 16px | Default component padding |
| `spacing-5` | 20px | Section margins |
| `spacing-6` | 24px | Card padding |
| `spacing-8` | 32px | Large section spacing |
| `spacing-10` | 40px | Major section breaks |
| `spacing-12` | 48px | Page-level spacing |
| `spacing-16` | 64px | Large gaps |

### Component Spacing
| Component | Padding | Margin | Gap |
|-----------|---------|--------|-----|
| Feed Card | 16px | 0 0 8px 0 | 12px |
| Profile Card | 24px | 0 0 8px 0 | 16px |
| Navigation | 0 16px | 0 | 24px |
| Modal | 24px | auto | 16px |
| Dropdown | 8px 0 | 4px 0 0 0 | 0 |
| Button | 6px 16px | 0 | 8px |
| Input | 12px 16px | 0 | 8px |
| Message Bubble | 12px 16px | 4px 0 | - |

### Layout Grid
```css
/* Desktop Feed Layout */
.feed-container {
  max-width: 1128px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 225px 1fr 300px;
  gap: 24px;
  padding: 24px;
}

/* Mobile Layout */
@media (max-width: 768px) {
  .feed-container {
    grid-template-columns: 1fr;
    padding: 0;
    gap: 8px;
  }
}
```

---

## 4. Border Radius

### Radius Scale
| Token | Value | Usage |
|-------|-------|-------|
| `radius-none` | 0px | Sharp edges, dividers |
| `radius-xs` | 2px | Tags, small badges |
| `radius-sm` | 4px | Buttons, inputs |
| `radius-md` | 8px | Cards, dropdowns |
| `radius-lg` | 12px | Modals, large cards |
| `radius-xl` | 16px | Featured content |
| `radius-full` | 9999px | Avatars, pills, circular buttons |

### Component Radius
| Component | Radius |
|-----------|--------|
| Profile Avatar (Large) | 50% (circular) |
| Profile Avatar (Small) | 50% (circular) |
| Company Logo | 4px |
| Feed Card | 8px |
| Modal | 8px |
| Button Primary | 24px (pill) |
| Button Secondary | 24px (pill) |
| Input Field | 4px |
| Dropdown | 8px |
| Message Bubble | 18px |
| Skill Badge | 4px |
| Notification Badge | 50% (circular) |
| Post Image | 8px |

---

## 5. Shadows and Elevation

### Shadow Scale
| Level | Shadow | Usage |
|-------|--------|-------|
| `elevation-0` | none | Flat elements |
| `elevation-1` | `0 0 0 1px rgba(0, 0, 0, 0.08)` | Cards at rest |
| `elevation-2` | `0 4px 12px rgba(0, 0, 0, 0.15)` | Cards on hover |
| `elevation-3` | `0 8px 24px rgba(0, 0, 0, 0.2)` | Dropdowns, tooltips |
| `elevation-4` | `0 12px 32px rgba(0, 0, 0, 0.25)` | Modals |
| `elevation-5` | `0 20px 48px rgba(0, 0, 0, 0.3)` | Full-screen overlays |

### Component Shadows
```css
/* Feed Card */
.feed-card {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
}

.feed-card:hover {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 4px 12px rgba(0, 0, 0, 0.12);
}

/* Dropdown Menu */
.dropdown {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 8px 24px rgba(0, 0, 0, 0.15);
}

/* Modal */
.modal {
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.2);
}

/* Navigation Header (Fixed) */
.navigation {
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.08);
}

/* Messaging Composer */
.message-composer {
  box-shadow: 0 -1px 3px rgba(0, 0, 0, 0.08);
}
```

### Focus States
```css
/* Default Focus Ring */
:focus-visible {
  outline: none;
  box-shadow: 0 0 0 2px #FFFFFF,
              0 0 0 4px #0A66C2;
}

/* Input Focus */
input:focus {
  border-color: #0A66C2;
  box-shadow: 0 0 0 2px rgba(10, 102, 194, 0.2);
}
```

---

## 6. Iconography

### Icon Sizes
| Size | Dimensions | Usage |
|------|------------|-------|
| Extra Small | 16px | Inline icons, badges |
| Small | 20px | Button icons, list items |
| Medium | 24px | Navigation, primary actions |
| Large | 32px | Empty states, featured |
| Extra Large | 48px | Illustrations, heroes |

### Icon Style Guidelines
- **Style**: Outlined icons for navigation, filled for active states
- **Stroke Width**: 1.5px - 2px consistent stroke
- **Corner Radius**: 1px rounded corners on paths
- **Color**: Inherit from parent, default `#000000` at 60% opacity
- **Active Color**: `#0A66C2` for selected/active states

### Core Navigation Icons
| Icon | Default State | Active State | Size |
|------|---------------|--------------|------|
| Home | Outline | Filled + Blue | 24px |
| Network | Outline | Filled + Blue | 24px |
| Jobs | Outline | Filled + Blue | 24px |
| Messaging | Outline | Filled + Blue | 24px |
| Notifications | Outline | Filled + Blue | 24px |
| Profile | Avatar | Blue ring | 24px |

### Action Icons
| Icon | Usage | Size |
|------|-------|------|
| Like (Thumbs up) | Post reactions | 20px |
| Comment | Post engagement | 20px |
| Repost | Share content | 20px |
| Send | Share via message | 20px |
| More (3 dots) | Overflow menu | 20px |
| Close (X) | Dismiss modals | 24px |
| Search | Search input | 20px |
| Edit (Pencil) | Edit actions | 20px |
| Settings (Gear) | Configuration | 24px |

### Reaction Icons
| Reaction | Color |
|----------|-------|
| Like | `#0A66C2` (Blue) |
| Celebrate | `#44712E` (Green) |
| Support | `#7A3E98` (Purple) |
| Love | `#DF704D` (Coral) |
| Insightful | `#E7A33E` (Gold) |
| Funny | `#7FC15E` (Light Green) |

---

## 7. Component Library

### Buttons

#### Primary Button
```css
.btn-primary {
  background-color: #0A66C2;
  color: #FFFFFF;
  border: none;
  border-radius: 24px;
  padding: 6px 16px;
  font-size: 16px;
  font-weight: 600;
  line-height: 24px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.btn-primary:hover {
  background-color: #004182;
}

.btn-primary:active {
  background-color: #00264D;
}

.btn-primary:disabled {
  background-color: rgba(0, 0, 0, 0.08);
  color: rgba(0, 0, 0, 0.4);
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.btn-secondary {
  background-color: transparent;
  color: #0A66C2;
  border: 1px solid #0A66C2;
  border-radius: 24px;
  padding: 5px 15px;
  font-size: 16px;
  font-weight: 600;
  line-height: 24px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.btn-secondary:hover {
  background-color: rgba(10, 102, 194, 0.08);
  border-color: #004182;
  color: #004182;
}
```

#### Tertiary Button (Text)
```css
.btn-tertiary {
  background-color: transparent;
  color: rgba(0, 0, 0, 0.6);
  border: none;
  padding: 6px 8px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
}

.btn-tertiary:hover {
  background-color: rgba(0, 0, 0, 0.08);
  border-radius: 4px;
  color: rgba(0, 0, 0, 0.9);
}
```

#### Connect Button (Special)
```css
.btn-connect {
  background-color: transparent;
  color: #0A66C2;
  border: 1px solid #0A66C2;
  border-radius: 24px;
  padding: 5px 15px;
  font-size: 16px;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 4px;
}

.btn-connect:hover {
  background-color: rgba(10, 102, 194, 0.08);
  border-width: 2px;
  padding: 4px 14px;
}
```

### Cards

#### Feed Post Card
```css
.feed-card {
  background: #FFFFFF;
  border-radius: 8px;
  border: 1px solid #E0DFDC;
  margin-bottom: 8px;
  overflow: hidden;
}

.feed-card-header {
  display: flex;
  padding: 12px 16px;
  gap: 8px;
}

.feed-card-avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  flex-shrink: 0;
}

.feed-card-author {
  flex: 1;
}

.feed-card-name {
  font-size: 14px;
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
  line-height: 20px;
}

.feed-card-headline {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
  line-height: 16px;
}

.feed-card-timestamp {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
}

.feed-card-content {
  padding: 0 16px 12px;
  font-size: 14px;
  line-height: 20px;
  color: rgba(0, 0, 0, 0.9);
}

.feed-card-actions {
  display: flex;
  border-top: 1px solid #E0DFDC;
  padding: 4px 8px;
}

.feed-card-action {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
  padding: 12px 8px;
  border-radius: 4px;
  color: rgba(0, 0, 0, 0.6);
  font-size: 14px;
  font-weight: 600;
}

.feed-card-action:hover {
  background-color: rgba(0, 0, 0, 0.08);
  color: rgba(0, 0, 0, 0.9);
}
```

#### Profile Card (Sidebar)
```css
.profile-card {
  background: #FFFFFF;
  border-radius: 8px;
  border: 1px solid #E0DFDC;
  overflow: hidden;
}

.profile-card-banner {
  height: 56px;
  background: linear-gradient(135deg, #0A66C2 0%, #004182 100%);
}

.profile-card-avatar-container {
  display: flex;
  justify-content: center;
  margin-top: -40px;
}

.profile-card-avatar {
  width: 72px;
  height: 72px;
  border-radius: 50%;
  border: 2px solid #FFFFFF;
}

.profile-card-info {
  text-align: center;
  padding: 12px 16px;
}

.profile-card-name {
  font-size: 16px;
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
}

.profile-card-headline {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
  margin-top: 4px;
}
```

#### Job Listing Card
```css
.job-card {
  display: flex;
  padding: 16px;
  gap: 12px;
  border-bottom: 1px solid #E0DFDC;
  background: #FFFFFF;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.job-card:hover {
  background-color: #F3F2EF;
}

.job-card-logo {
  width: 56px;
  height: 56px;
  border-radius: 4px;
  flex-shrink: 0;
}

.job-card-content {
  flex: 1;
}

.job-card-title {
  font-size: 16px;
  font-weight: 600;
  color: #0A66C2;
  line-height: 24px;
}

.job-card-title:hover {
  text-decoration: underline;
}

.job-card-company {
  font-size: 14px;
  color: rgba(0, 0, 0, 0.9);
  line-height: 20px;
}

.job-card-meta {
  font-size: 14px;
  color: rgba(0, 0, 0, 0.6);
  line-height: 20px;
}

.job-card-insights {
  margin-top: 8px;
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
}
```

#### Connection Card
```css
.connection-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 24px 16px;
  background: #FFFFFF;
  border-radius: 8px;
  border: 1px solid #E0DFDC;
  text-align: center;
}

.connection-card-avatar {
  width: 104px;
  height: 104px;
  border-radius: 50%;
  margin-bottom: 12px;
}

.connection-card-name {
  font-size: 16px;
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
}

.connection-card-headline {
  font-size: 14px;
  color: rgba(0, 0, 0, 0.6);
  margin-top: 4px;
  max-height: 40px;
  overflow: hidden;
}

.connection-card-mutual {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
  margin-top: 8px;
}

.connection-card-actions {
  margin-top: 16px;
  display: flex;
  gap: 8px;
}
```

### Form Elements

#### Text Input
```css
.input-text {
  width: 100%;
  padding: 12px 16px;
  border: 1px solid rgba(0, 0, 0, 0.4);
  border-radius: 4px;
  font-size: 14px;
  line-height: 20px;
  color: rgba(0, 0, 0, 0.9);
  background: #FFFFFF;
  transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.input-text::placeholder {
  color: rgba(0, 0, 0, 0.4);
}

.input-text:hover {
  border-color: rgba(0, 0, 0, 0.6);
}

.input-text:focus {
  outline: none;
  border-color: #0A66C2;
  box-shadow: 0 0 0 2px rgba(10, 102, 194, 0.2);
}

.input-text:disabled {
  background: #F3F2EF;
  color: rgba(0, 0, 0, 0.4);
  cursor: not-allowed;
}
```

#### Search Input
```css
.search-input-container {
  position: relative;
  width: 100%;
  max-width: 280px;
}

.search-input {
  width: 100%;
  padding: 8px 16px 8px 40px;
  background: #EEF3F8;
  border: none;
  border-radius: 4px;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.9);
}

.search-input::placeholder {
  color: rgba(0, 0, 0, 0.6);
}

.search-input:focus {
  outline: none;
  background: #FFFFFF;
  box-shadow: 0 0 0 2px #0A66C2;
}

.search-icon {
  position: absolute;
  left: 12px;
  top: 50%;
  transform: translateY(-50%);
  color: rgba(0, 0, 0, 0.6);
}
```

### Navigation

#### Top Navigation Bar
```css
.nav-header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 52px;
  background: #FFFFFF;
  border-bottom: 1px solid #E0DFDC;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 16px;
  z-index: 100;
}

.nav-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  max-width: 1128px;
}

.nav-logo {
  width: 34px;
  height: 34px;
}

.nav-items {
  display: flex;
  align-items: center;
  gap: 8px;
}

.nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0 12px;
  min-width: 60px;
  color: rgba(0, 0, 0, 0.6);
  text-decoration: none;
  font-size: 12px;
  font-weight: 400;
}

.nav-item:hover {
  color: rgba(0, 0, 0, 0.9);
}

.nav-item.active {
  color: rgba(0, 0, 0, 0.9);
  border-bottom: 2px solid rgba(0, 0, 0, 0.9);
}

.nav-icon {
  width: 24px;
  height: 24px;
  margin-bottom: 2px;
}
```

### Messaging

#### Message Thread Item
```css
.message-thread {
  display: flex;
  padding: 12px 16px;
  gap: 8px;
  cursor: pointer;
  transition: background-color 0.15s ease;
}

.message-thread:hover {
  background-color: rgba(0, 0, 0, 0.08);
}

.message-thread.active {
  background-color: #E8F4FD;
}

.message-thread.unread .message-preview {
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
}

.message-avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  flex-shrink: 0;
  position: relative;
}

.message-avatar.online::after {
  content: '';
  position: absolute;
  bottom: 2px;
  right: 2px;
  width: 10px;
  height: 10px;
  background: #057642;
  border: 2px solid #FFFFFF;
  border-radius: 50%;
}

.message-content {
  flex: 1;
  min-width: 0;
}

.message-name {
  font-size: 14px;
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
}

.message-preview {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.message-time {
  font-size: 12px;
  color: rgba(0, 0, 0, 0.6);
  flex-shrink: 0;
}
```

#### Message Bubble
```css
.message-bubble {
  max-width: 70%;
  padding: 12px 16px;
  border-radius: 18px;
  font-size: 14px;
  line-height: 20px;
  word-wrap: break-word;
}

.message-bubble.sent {
  background: #0A66C2;
  color: #FFFFFF;
  border-bottom-right-radius: 4px;
  margin-left: auto;
}

.message-bubble.received {
  background: #F3F2EF;
  color: rgba(0, 0, 0, 0.9);
  border-bottom-left-radius: 4px;
}
```

### Notification Badge
```css
.notification-badge {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-width: 18px;
  height: 18px;
  padding: 0 6px;
  background: #C83636;
  color: #FFFFFF;
  font-size: 12px;
  font-weight: 600;
  border-radius: 9px;
  position: absolute;
  top: -4px;
  right: -4px;
}
```

### Modal
```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.75);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}

.modal {
  background: #FFFFFF;
  border-radius: 8px;
  width: 100%;
  max-width: 552px;
  max-height: 90vh;
  overflow: hidden;
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.2);
}

.modal-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 24px;
  border-bottom: 1px solid #E0DFDC;
}

.modal-title {
  font-size: 20px;
  font-weight: 600;
  color: rgba(0, 0, 0, 0.9);
}

.modal-close {
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  cursor: pointer;
  color: rgba(0, 0, 0, 0.6);
}

.modal-close:hover {
  background: rgba(0, 0, 0, 0.08);
}

.modal-body {
  padding: 16px 24px;
  overflow-y: auto;
  max-height: calc(90vh - 140px);
}

.modal-footer {
  display: flex;
  justify-content: flex-end;
  gap: 8px;
  padding: 16px 24px;
  border-top: 1px solid #E0DFDC;
}
```

---

## 8. Animation & Motion

### Timing Functions
```css
/* Standard easing */
--ease-standard: cubic-bezier(0.4, 0, 0.2, 1);

/* Deceleration (entering) */
--ease-decelerate: cubic-bezier(0, 0, 0.2, 1);

/* Acceleration (exiting) */
--ease-accelerate: cubic-bezier(0.4, 0, 1, 1);

/* Sharp/Emphasized */
--ease-sharp: cubic-bezier(0.4, 0, 0.6, 1);
```

### Duration Scale
| Token | Duration | Usage |
|-------|----------|-------|
| `duration-instant` | 100ms | Hover states, color changes |
| `duration-fast` | 150ms | Button presses, micro-interactions |
| `duration-normal` | 200ms | Standard transitions |
| `duration-slow` | 300ms | Expanding panels, modals entering |
| `duration-slower` | 400ms | Complex animations |
| `duration-slowest` | 500ms | Page transitions |

### Standard Transitions
```css
/* Button hover */
.btn {
  transition: background-color 150ms var(--ease-standard),
              border-color 150ms var(--ease-standard),
              color 150ms var(--ease-standard);
}

/* Card hover */
.card {
  transition: box-shadow 200ms var(--ease-standard),
              transform 200ms var(--ease-standard);
}

.card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

/* Link underline */
.link {
  transition: color 100ms var(--ease-standard);
}

/* Dropdown */
.dropdown {
  transition: opacity 200ms var(--ease-decelerate),
              transform 200ms var(--ease-decelerate);
}
```

### Animation Keyframes
```css
/* Fade In */
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Slide In From Bottom */
@keyframes slideInUp {
  from {
    opacity: 0;
    transform: translateY(16px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Modal Enter */
@keyframes modalEnter {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Notification Pulse */
@keyframes pulse {
  0%, 100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
}

/* Skeleton Loading */
@keyframes shimmer {
  0% {
    background-position: -200% 0;
  }
  100% {
    background-position: 200% 0;
  }
}

.skeleton {
  background: linear-gradient(
    90deg,
    #F3F2EF 0%,
    #E8E8E8 50%,
    #F3F2EF 100%
  );
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}

/* Typing Indicator */
@keyframes typingBounce {
  0%, 60%, 100% {
    transform: translateY(0);
  }
  30% {
    transform: translateY(-4px);
  }
}

.typing-dot {
  animation: typingBounce 1.4s infinite;
}

.typing-dot:nth-child(2) {
  animation-delay: 0.2s;
}

.typing-dot:nth-child(3) {
  animation-delay: 0.4s;
}
```

### Component Animations
```css
/* Post Reaction */
.reaction-btn.active {
  animation: pulse 300ms var(--ease-standard);
}

/* New notification */
.notification-badge.new {
  animation: pulse 600ms var(--ease-standard) infinite;
}

/* Feed post appearing */
.feed-card {
  animation: slideInUp 300ms var(--ease-decelerate);
}

/* Modal */
.modal {
  animation: modalEnter 300ms var(--ease-decelerate);
}

/* Toast notification */
.toast {
  animation: slideInUp 300ms var(--ease-decelerate);
}
```

---

## 9. Responsive Breakpoints

### Breakpoint Scale
| Name | Min Width | Max Width | Usage |
|------|-----------|-----------|-------|
| Mobile Small | 0px | 479px | Small phones |
| Mobile | 480px | 767px | Standard phones |
| Tablet | 768px | 1023px | Tablets, small laptops |
| Desktop | 1024px | 1279px | Standard desktops |
| Desktop Large | 1280px | 1535px | Large desktops |
| Desktop XL | 1536px+ | - | Ultra-wide monitors |

### Media Query Mixins
```css
/* Mobile First Approach */
@media (min-width: 768px) { /* Tablet and up */ }
@media (min-width: 1024px) { /* Desktop and up */ }
@media (min-width: 1280px) { /* Large desktop and up */ }

/* Desktop First Approach */
@media (max-width: 1023px) { /* Tablet and below */ }
@media (max-width: 767px) { /* Mobile only */ }
```

### Responsive Layout Patterns

#### Feed Layout
```css
/* Mobile */
.feed-layout {
  display: flex;
  flex-direction: column;
  gap: 0;
}

.feed-sidebar-left,
.feed-sidebar-right {
  display: none;
}

/* Tablet */
@media (min-width: 768px) {
  .feed-layout {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 24px;
    padding: 24px;
    max-width: 1024px;
    margin: 0 auto;
  }
  
  .feed-sidebar-left {
    display: block;
  }
}

/* Desktop */
@media (min-width: 1024px) {
  .feed-layout {
    grid-template-columns: 225px 1fr 300px;
    max-width: 1128px;
  }
  
  .feed-sidebar-right {
    display: block;
  }
}
```

#### Navigation Responsive
```css
/* Mobile Navigation */
.nav-mobile {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: space-around;
  background: #FFFFFF;
  border-top: 1px solid #E0DFDC;
  padding: 8px 0;
  z-index: 100;
}

.nav-desktop {
  display: none;
}

/* Desktop Navigation */
@media (min-width: 768px) {
  .nav-mobile {
    display: none;
  }
  
  .nav-desktop {
    display: flex;
  }
}
```

#### Card Grid Responsive
```css
/* Connection Cards Grid */
.connection-grid {
  display: grid;
  gap: 8px;
  grid-template-columns: 1fr;
}

@media (min-width: 480px) {
  .connection-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 768px) {
  .connection-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
  }
}

@media (min-width: 1024px) {
  .connection-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}
```

#### Typography Responsive
```css
/* Base mobile sizes */
.display-large {
  font-size: 24px;
  line-height: 32px;
}

.heading-large {
  font-size: 18px;
  line-height: 24px;
}

/* Desktop sizes */
@media (min-width: 768px) {
  .display-large {
    font-size: 32px;
    line-height: 40px;
  }
  
  .heading-large {
    font-size: 20px;
    line-height: 28px;
  }
}
```

### Touch Targets
```css
/* Minimum touch target for mobile */
.touch-target {
  min-width: 44px;
  min-height: 44px;
}

/* Larger touch targets on mobile */
@media (max-width: 767px) {
  .btn {
    min-height: 48px;
    padding: 12px 24px;
  }
  
  .nav-item {
    min-width: 64px;
    padding: 12px 8px;
  }
}
```

### Container Widths
```css
.container {
  width: 100%;
  margin: 0 auto;
  padding: 0 16px;
}

@media (min-width: 768px) {
  .container {
    padding: 0 24px;
    max-width: 720px;
  }
}

@media (min-width: 1024px) {
  .container {
    max-width: 1024px;
  }
}

@media (min-width: 1280px) {
  .container {
    max-width: 1128px;
  }
}
```

---

## Design Tokens Summary

```css
:root {
  /* Colors */
  --color-primary: #0A66C2;
  --color-primary-light: #70B5F9;
  --color-primary-dark: #004182;
  --color-background: #F3F2EF;
  --color-surface: #FFFFFF;
  --color-border: #E0DFDC;
  --color-text-primary: rgba(0, 0, 0, 0.9);
  --color-text-secondary: rgba(0, 0, 0, 0.6);
  --color-text-disabled: rgba(0, 0, 0, 0.4);
  --color-success: #057642;
  --color-error: #B24020;
  --color-premium: #C37D16;
  
  /* Typography */
  --font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;
  --font-size-xs: 11px;
  --font-size-sm: 12px;
  --font-size-md: 14px;
  --font-size-lg: 16px;
  --font-size-xl: 18px;
  --font-size-2xl: 20px;
  --font-size-3xl: 24px;
  --font-size-4xl: 32px;
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;
  
  /* Spacing */
  --spacing-1: 4px;
  --spacing-2: 8px;
  --spacing-3: 12px;
  --spacing-4: 16px;
  --spacing-5: 20px;
  --spacing-6: 24px;
  --spacing-8: 32px;
  --spacing-10: 40px;
  --spacing-12: 48px;
  
  /* Border Radius */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-pill: 24px;
  --radius-full: 9999px;
  
  /* Shadows */
  --shadow-card: 0 0 0 1px rgba(0, 0, 0, 0.08);
  --shadow-card-hover: 0 0 0 1px rgba(0, 0, 0, 0.08), 0 4px 12px rgba(0, 0, 0, 0.12);
  --shadow-dropdown: 0 0 0 1px rgba(0, 0, 0, 0.08), 0 8px 24px rgba(0, 0, 0, 0.15);
  --shadow-modal: 0 12px 32px rgba(0, 0, 0, 0.2);
  
  /* Transitions */
  --transition-fast: 150ms cubic-bezier(0.4, 0, 0.2, 1);
  --transition-normal: 200ms cubic-bezier(0.4, 0, 0.2, 1);
  --transition-slow: 300ms cubic-bezier(0.4, 0, 0.2, 1);
  
  /* Z-Index */
  --z-dropdown: 100;
  --z-sticky: 200;
  --z-fixed: 300;
  --z-modal-backdrop: 400;
  --z-modal: 500;
  --z-tooltip: 600;
}
```

---

*This design system reflects LinkedIn's professional, corporate aesthetic focused on career networking, job discovery, and professional content sharing.*
