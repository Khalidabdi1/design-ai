# Mastodon Design System

> Decentralized, open-source social network with privacy-first design. Mastodon Purple (#6364FF) accent, dark immersive theme, multi-column TweetDeck-style interface, federation-aware UI patterns.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Mastodon embraces a **privacy-conscious, community-driven** design philosophy. The interface feels like a thoughtfully crafted space that respects user autonomy—dark, focused, and intentionally free from dark patterns. Every element is designed to promote healthy social interaction while giving users control over their experience.

### Mood & Feeling
- **Open & Transparent**: The open-source ethos extends to design—no hidden features, clear navigation
- **Calm & Focused**: Dark backgrounds reduce eye strain and create a distraction-free reading experience
- **Community-First**: Instance branding, federation indicators, and local/federated timelines emphasize decentralization
- **Privacy-Respectful**: Content warnings, granular visibility controls, and clear data handling

### Design Density
**Medium-high density** with intentional information hierarchy. The multi-column layout allows power users to monitor multiple timelines simultaneously while maintaining readability. Single-column mode provides a cleaner experience for focused browsing.

### Visual Character
- Clean, functional design without unnecessary decoration
- Subtle rounded corners for approachability
- Clear visual hierarchy through background layering
- Federation indicators (instance badges, remote user markers)
- Content warning system as first-class UI element
- Boost and favorite actions clearly distinguished
- Accessible, screen-reader friendly patterns

---

## 2. Color Palette & Roles

### Primary Dark Theme

| Token | Hex | Role |
|-------|-----|------|
| `--background-base` | `#191b22` | Deepest background, app container |
| `--background-elevated` | `#282c37` | Cards, panels, columns |
| `--background-input` | `#1f232b` | Form inputs, text areas |
| `--background-hover` | `#313543` | Interactive hover states |
| `--background-active` | `#393f4f` | Active/selected states |
| `--background-overlay` | `rgba(0, 0, 0, 0.7)` | Modal backdrops |

### Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--mastodon-purple` | `#6364FF` | Primary brand, buttons, links, accents |
| `--mastodon-purple-hover` | `#7477FF` | Hover state for purple elements |
| `--mastodon-purple-active` | `#5253E0` | Active/pressed purple |
| `--mastodon-purple-muted` | `rgba(99, 100, 255, 0.2)` | Subtle purple backgrounds |
| `--mastodon-purple-dark` | `#4E4FCC` | Dark purple for emphasis |

### Text Colors

| Token | Hex | Role |
|-------|-----|------|
| `--text-primary` | `#ffffff` | Primary headings, important text |
| `--text-secondary` | `#9baec8` | Body text, content |
| `--text-tertiary` | `#606984` | Muted text, timestamps, metadata |
| `--text-link` | `#6364FF` | Hyperlinks |
| `--text-link-hover` | `#858AFA` | Link hover state |
| `--text-inverse` | `#282c37` | Text on light/purple backgrounds |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--color-success` | `#79bd9a` | Success states, confirmations |
| `--color-warning` | `#ca8f04` | Warnings, cautions |
| `--color-error` | `#df405a` | Errors, destructive actions |
| `--color-info` | `#6364FF` | Informational highlights |
| `--color-boost` | `#2b90d9` | Boost (retweet) action |
| `--color-favorite` | `#ca8f04` | Favorite (star) action |
| `--color-bookmark` | `#6364FF` | Bookmark action |

### Federation Indicators

| Token | Hex | Role |
|-------|-----|------|
| `--federation-local` | `#79bd9a` | Local instance content |
| `--federation-remote` | `#6364FF` | Federated/remote content |
| `--instance-badge-bg` | `#393f4f` | Instance name badge background |

### Light Theme (Alternate)

| Token | Hex | Role |
|-------|-----|------|
| `--background-base` | `#f2f5f7` | App container |
| `--background-elevated` | `#ffffff` | Cards, panels |
| `--background-input` | `#f0f3f5` | Form inputs |
| `--text-primary` | `#282c37` | Primary text |
| `--text-secondary` | `#444b5d` | Body text |
| `--text-tertiary` | `#9baec8` | Muted text |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary system font stack */
--font-primary: 'mastodon-font-sans-serif', system-ui, -apple-system, 
                BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, 
                Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', 
                sans-serif;

/* Monospace for code and technical content */
--font-mono: 'mastodon-font-monospace', ui-monospace, 'Cascadia Mono', 
             'Segoe UI Mono', 'Liberation Mono', Menlo, Monaco, Consolas, 
             monospace;

/* Display font for marketing/landing pages */
--font-display: 'Poppins', var(--font-primary);
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Display Headline | 28px | 700 | 36px | -0.02em | `--text-primary` |
| Column Header | 16px | 700 | 24px | 0 | `--text-primary` |
| Post Author | 15px | 700 | 20px | 0 | `--text-primary` |
| Post Handle | 15px | 400 | 20px | 0 | `--text-tertiary` |
| Post Content | 15px | 400 | 22px | 0 | `--text-secondary` |
| Timestamp | 14px | 400 | 20px | 0 | `--text-tertiary` |
| Button Text | 14px | 600 | 18px | 0.02em | White or contextual |
| Form Label | 14px | 500 | 20px | 0 | `--text-secondary` |
| Input Text | 15px | 400 | 22px | 0 | `--text-primary` |
| Small Text | 13px | 400 | 18px | 0 | `--text-tertiary` |
| Counter Badge | 12px | 600 | 14px | 0 | `--text-primary` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, posts, descriptions |
| 500 | Medium | Form labels, subtle emphasis |
| 600 | Semibold | Buttons, links, interactive elements |
| 700 | Bold | Headings, usernames, strong emphasis |

### Post Content Typography

```css
/* Post text with proper wrapping and overflow */
.post-content {
  font-size: 15px;
  line-height: 22px;
  color: #9baec8;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

/* Hashtags and mentions */
.hashtag,
.mention {
  color: #6364FF;
  text-decoration: none;
}

.hashtag:hover,
.mention:hover {
  text-decoration: underline;
}

/* Content warnings */
.content-warning {
  font-size: 15px;
  font-weight: 500;
  color: #ffffff;
}
```

---

## 4. Component Stylings

### Buttons

#### Primary Button (Purple)
```css
.button-primary {
  background: #6364FF;
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  padding: 10px 18px;
  border-radius: 4px;
  border: none;
  cursor: pointer;
  transition: background-color 100ms ease-in-out;
}

.button-primary:hover {
  background: #7477FF;
}

.button-primary:active {
  background: #5253E0;
}

.button-primary:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
```

#### Secondary Button (Outlined)
```css
.button-secondary {
  background: transparent;
  color: #6364FF;
  font-size: 14px;
  font-weight: 600;
  padding: 9px 17px;
  border-radius: 4px;
  border: 1px solid #6364FF;
  cursor: pointer;
}

.button-secondary:hover {
  background: rgba(99, 100, 255, 0.1);
}
```

#### Danger Button
```css
.button-danger {
  background: #df405a;
  color: #ffffff;
}

.button-danger:hover {
  background: #e85e73;
}
```

#### Icon Button (Actions)
```css
.button-icon {
  background: transparent;
  color: #606984;
  padding: 8px;
  border-radius: 4px;
  border: none;
  cursor: pointer;
  transition: all 100ms ease-in-out;
}

.button-icon:hover {
  color: #6364FF;
  background: rgba(99, 100, 255, 0.1);
}

/* Boost action */
.button-icon.boost:hover,
.button-icon.boost.active {
  color: #2b90d9;
}

/* Favorite action */
.button-icon.favorite:hover,
.button-icon.favorite.active {
  color: #ca8f04;
}
```

### Inputs

#### Text Input
```css
.input {
  background: #1f232b;
  border: 1px solid #393f4f;
  border-radius: 4px;
  color: #ffffff;
  font-size: 15px;
  padding: 10px 12px;
  width: 100%;
  transition: border-color 100ms ease-in-out;
}

.input:focus {
  outline: none;
  border-color: #6364FF;
}

.input::placeholder {
  color: #606984;
}
```

#### Compose Text Area
```css
.compose-textarea {
  background: #282c37;
  border: none;
  border-radius: 4px;
  color: #ffffff;
  font-size: 15px;
  line-height: 22px;
  padding: 12px;
  resize: none;
  min-height: 100px;
}

.compose-textarea::placeholder {
  color: #606984;
}

.compose-textarea:focus {
  outline: none;
}
```

#### Search Input
```css
.search-input {
  background: #1f232b;
  border: 1px solid transparent;
  border-radius: 8px;
  color: #ffffff;
  font-size: 14px;
  padding: 10px 12px 10px 40px;
  width: 100%;
}

.search-input:focus {
  border-color: #6364FF;
  background: #282c37;
}
```

### Cards

#### Toot/Post Card
```css
.toot-card {
  background: #282c37;
  border-bottom: 1px solid #393f4f;
  padding: 14px 16px;
}

.toot-card:hover {
  background: #2c313d;
}

.toot-avatar {
  width: 46px;
  height: 46px;
  border-radius: 4px;
  margin-right: 10px;
}

.toot-header {
  display: flex;
  align-items: baseline;
  gap: 4px;
}

.toot-author {
  color: #ffffff;
  font-weight: 700;
  font-size: 15px;
}

.toot-handle {
  color: #606984;
  font-size: 15px;
}

.toot-timestamp {
  color: #606984;
  font-size: 14px;
}

.toot-content {
  color: #9baec8;
  font-size: 15px;
  line-height: 22px;
  margin-top: 8px;
}
```

#### Content Warning Card
```css
.content-warning {
  background: #393f4f;
  border-radius: 4px;
  padding: 12px;
  margin-top: 8px;
}

.content-warning-label {
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  margin-bottom: 8px;
}

.content-warning-toggle {
  background: #282c37;
  color: #9baec8;
  border: none;
  border-radius: 4px;
  padding: 6px 12px;
  font-size: 13px;
  cursor: pointer;
}

.content-warning-toggle:hover {
  background: #313543;
}
```

#### Account Card
```css
.account-card {
  background: #282c37;
  border-radius: 8px;
  padding: 16px;
}

.account-card-header {
  background: linear-gradient(135deg, #6364FF 0%, #8385FF 100%);
  height: 80px;
  border-radius: 8px 8px 0 0;
  margin: -16px -16px 16px -16px;
}

.account-card-avatar {
  width: 80px;
  height: 80px;
  border-radius: 4px;
  border: 4px solid #282c37;
  margin-top: -40px;
}

.account-card-name {
  color: #ffffff;
  font-size: 16px;
  font-weight: 700;
}

.account-card-handle {
  color: #606984;
  font-size: 14px;
}
```

#### Media Attachment
```css
.media-attachment {
  border-radius: 8px;
  overflow: hidden;
  margin-top: 10px;
}

.media-attachment img,
.media-attachment video {
  width: 100%;
  height: auto;
  display: block;
}

.media-sensitive-overlay {
  background: #191b22;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #9baec8;
}
```

### Action Bar

```css
.action-bar {
  display: flex;
  justify-content: space-between;
  margin-top: 12px;
  max-width: 400px;
}

.action-button {
  display: flex;
  align-items: center;
  gap: 6px;
  background: transparent;
  border: none;
  color: #606984;
  font-size: 14px;
  padding: 4px 8px;
  border-radius: 4px;
  cursor: pointer;
  transition: all 100ms ease-in-out;
}

.action-button:hover {
  background: rgba(99, 100, 255, 0.1);
}

.action-button.reply:hover { color: #6364FF; }
.action-button.boost:hover,
.action-button.boost.active { color: #2b90d9; }
.action-button.favorite:hover,
.action-button.favorite.active { color: #ca8f04; }
.action-button.bookmark:hover,
.action-button.bookmark.active { color: #6364FF; }
.action-button.share:hover { color: #6364FF; }
```

### Navigation

#### Column Header
```css
.column-header {
  background: #282c37;
  border-bottom: 1px solid #393f4f;
  padding: 15px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.column-header-title {
  color: #ffffff;
  font-size: 16px;
  font-weight: 700;
}

.column-header-icon {
  color: #9baec8;
}
```

#### Tab Navigation
```css
.tabs {
  display: flex;
  border-bottom: 1px solid #393f4f;
}

.tab {
  flex: 1;
  padding: 14px;
  color: #606984;
  font-size: 14px;
  font-weight: 600;
  text-align: center;
  border-bottom: 2px solid transparent;
  cursor: pointer;
  transition: all 100ms ease-in-out;
}

.tab:hover {
  color: #9baec8;
  background: rgba(99, 100, 255, 0.05);
}

.tab.active {
  color: #6364FF;
  border-bottom-color: #6364FF;
}
```

#### Sidebar Navigation
```css
.nav-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 16px;
  color: #9baec8;
  font-size: 15px;
  font-weight: 500;
  border-radius: 8px;
  cursor: pointer;
  transition: all 100ms ease-in-out;
}

.nav-item:hover {
  background: #282c37;
  color: #ffffff;
}

.nav-item.active {
  background: rgba(99, 100, 255, 0.15);
  color: #6364FF;
}

.nav-item-icon {
  width: 22px;
  height: 22px;
}

.nav-item-badge {
  background: #6364FF;
  color: #ffffff;
  font-size: 12px;
  font-weight: 600;
  padding: 2px 8px;
  border-radius: 10px;
  margin-left: auto;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.7);
  position: fixed;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal {
  background: #282c37;
  border-radius: 8px;
  max-width: 480px;
  width: 100%;
  max-height: 90vh;
  overflow-y: auto;
}

.modal-header {
  padding: 16px;
  border-bottom: 1px solid #393f4f;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.modal-title {
  color: #ffffff;
  font-size: 16px;
  font-weight: 700;
}

.modal-close {
  color: #606984;
  background: transparent;
  border: none;
  cursor: pointer;
}

.modal-body {
  padding: 16px;
}

.modal-footer {
  padding: 16px;
  border-top: 1px solid #393f4f;
  display: flex;
  justify-content: flex-end;
  gap: 8px;
}
```

### Toasts/Notifications

```css
.toast {
  background: #282c37;
  border-radius: 8px;
  padding: 14px 16px;
  display: flex;
  align-items: center;
  gap: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
}

.toast-success {
  border-left: 4px solid #79bd9a;
}

.toast-error {
  border-left: 4px solid #df405a;
}

.toast-message {
  color: #9baec8;
  font-size: 14px;
}
```

### Instance Badge

```css
.instance-badge {
  background: #393f4f;
  color: #9baec8;
  font-size: 12px;
  padding: 2px 6px;
  border-radius: 3px;
  display: inline-block;
}

.instance-badge.local {
  background: rgba(121, 189, 154, 0.2);
  color: #79bd9a;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-2` | 2px | Micro gaps, inline spacing |
| `--spacing-4` | 4px | Tight element gaps |
| `--spacing-8` | 8px | Standard element gaps |
| `--spacing-10` | 10px | Small component padding |
| `--spacing-14` | 14px | Card padding |
| `--spacing-16` | 16px | Standard padding |
| `--spacing-20` | 20px | Section spacing |
| `--spacing-24` | 24px | Large section breaks |

### Multi-Column Layout (Advanced Web)

```
┌────────────────────────────────────────────────────────────────────────┐
│ ┌────────┬───────────┬───────────┬───────────┬───────────┬──────────┐ │
│ │        │           │           │           │           │          │ │
│ │  Nav   │   Home    │ Notifi-   │  Local    │ Federated │ Getting  │ │
│ │        │  Timeline │  cations  │  Timeline │  Timeline │  Started │ │
│ │        │           │           │           │           │          │ │
│ │  60px  │   350px   │   350px   │   350px   │   350px   │  285px   │ │
│ │        │           │           │           │           │          │ │
│ └────────┴───────────┴───────────┴───────────┴───────────┴──────────┘ │
└────────────────────────────────────────────────────────────────────────┘
```

### Single-Column Layout (Simple Web/Mobile)

```
┌─────────────────────────────────────────────┐
│ ┌─────────────────────────────────────────┐ │
│ │              Navigation                 │ │
│ ├─────────────────────────────────────────┤ │
│ │              Compose                    │ │
│ ├─────────────────────────────────────────┤ │
│ │                                         │ │
│ │              Timeline                   │ │
│ │                                         │ │
│ │           max-width: 600px              │ │
│ │                                         │ │
│ │                                         │ │
│ ├─────────────────────────────────────────┤ │
│ │    Search / Trends / Suggestions        │ │
│ └─────────────────────────────────────────┘ │
└─────────────────────────────────────────────┘
```

### Column Widths

| Panel | Width | Notes |
|-------|-------|-------|
| Navigation Rail | 60px | Icon-only navigation |
| Standard Column | 350px | Timeline, notifications |
| Compose Panel | 285px | Getting started, compose |
| Single-Column Content | 600px max | Mobile/simple view |
| Profile Header | Full width | Responsive within container |

### Grid System
Mastodon uses a **flex-based multi-column layout** for the advanced web interface. Columns are fixed-width and horizontally scrollable. Single-column mode centers content with max-width constraints.

### Whitespace Philosophy
- **Breathing room in posts**: Adequate padding between posts for readability
- **Compact action bars**: Action buttons are tightly spaced to save vertical space
- **Clear column separation**: Visual distinction through background color
- **Consistent internal padding**: 14-16px within cards and containers

---

## 6. Depth & Elevation

### Shadow System

| Level | Shadow | Usage |
|-------|--------|-------|
| Level 0 | None | Base surfaces, columns |
| Level 1 | `0 1px 2px rgba(0, 0, 0, 0.2)` | Subtle lift, dropdown triggers |
| Level 2 | `0 4px 8px rgba(0, 0, 0, 0.3)` | Dropdowns, popovers |
| Level 3 | `0 8px 16px rgba(0, 0, 0, 0.4)` | Modals, dialogs |
| Level 4 | `0 16px 32px rgba(0, 0, 0, 0.5)` | Large overlays |

### Surface Hierarchy

```
┌─────────────────────────────────────────────────────────┐
│ Modal/Floating                         #282c37 + shadow │
├─────────────────────────────────────────────────────────┤
│ Columns/Panels                         #282c37          │
├─────────────────────────────────────────────────────────┤
│ Hover/Interactive                      #313543          │
├─────────────────────────────────────────────────────────┤
│ Base/App Background                    #191b22          │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Columns, content |
| Sticky Headers | 100 | Column headers |
| Dropdown | 1000 | Menus, autocomplete |
| Popout | 1001 | User cards, popovers |
| Modal | 1002 | Dialogs, modals |
| Toast | 1003 | Notifications |
| Tooltip | 1004 | Tooltips |
| Compose Overlay | 1005 | Full-screen compose |

### Border Treatments

```css
/* Standard border */
border: 1px solid #393f4f;

/* Subtle separator */
border-bottom: 1px solid #393f4f;

/* Focus ring */
outline: 2px solid #6364FF;
outline-offset: 2px;

/* Boost indicator */
border-left: 4px solid #2b90d9;

/* Content warning */
border-radius: 4px;
background: #393f4f;
```

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use Mastodon Purple (#6364FF) as primary accent | Brand recognition, consistency |
| Maintain dark backgrounds as default | Eye comfort, immersive reading |
| Show federation context (instance badges) | Users should know where content originates |
| Implement content warnings properly | Core feature of Mastodon culture |
| Display clear boost vs. favorite distinction | Different actions have different meanings |
| Use accessible color contrast (4.5:1 minimum) | Open-source projects prioritize accessibility |
| Support keyboard navigation throughout | Power users and accessibility |
| Show character count in compose | Mastodon has character limits |
| Indicate sensitive media clearly | User safety and consent |
| Allow instance-level customization | Decentralization means branding flexibility |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never auto-expand content warnings | Defeats the purpose of CW system |
| Avoid algorithmic feed manipulation UI | Mastodon is chronological by design |
| Don't hide federation indicators | Transparency about content origin |
| Never auto-play media without consent | Respect user preferences |
| Avoid dark patterns for engagement | Against Mastodon's ethical design values |
| Don't use "retweet"/"like" terminology | Use Mastodon terms: boost, favorite |
| Never collect unnecessary analytics | Privacy-first platform |
| Avoid engagement metric prominence | Social media wellness, not vanity metrics |
| Don't make ads UI patterns | Mastodon is ad-free by design |
| Never use infinite scroll without pause | Encourage intentional usage |

### Content & Tone Guidelines

| Do | Don't |
|----|-------|
| Use inclusive, welcoming language | Corporate or aggressive marketing tone |
| Explain federation concepts clearly | Assume users understand decentralization |
| Provide clear moderation controls | Hide safety features |
| Show timestamps in human-readable format | Unix timestamps or confusing formats |
| Translate instance rules clearly | Use technical/legal jargon |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Desktop XL | >1400px | Multiple columns visible |
| Desktop | 1024px - 1400px | 3-4 columns with scroll |
| Tablet | 768px - 1023px | Single column, sidebar toggle |
| Mobile | <768px | Single column, bottom navigation |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Navigation | Left sidebar rail | Bottom tab bar |
| Columns | Horizontal scroll | Single column |
| Compose | Inline in column | Full-screen modal |
| Search | Header search | Dedicated tab |
| Profile | Card + tabs | Stacked sections |
| Actions | Icon + count | Icon only |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Action Buttons | 44px × 44px | Reply, boost, favorite, etc. |
| Navigation Items | 48px × 48px | Bottom nav tabs |
| Avatar | 46px × 46px | Tappable profile link |
| Follow Button | 44px height | Comfortable touch |
| Menu Items | 44px height | Dropdown items |

### Responsive Typography

| Element | Desktop | Mobile |
|---------|---------|--------|
| Post Content | 15px | 16px |
| Display Name | 15px | 16px |
| Timestamps | 14px | 13px |
| Action Labels | Visible | Hidden (icons only) |

### Image Handling

| Context | Behavior |
|---------|----------|
| Avatar | 46px default, 80px in profile |
| Header Image | 400px height max, responsive width |
| Media Attachment | Max-height 300px, maintain aspect ratio |
| Sensitive Media | Blurred overlay until revealed |
| Emoji | 22px inline, 36px in picker |

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Backgrounds
Background Base: #191b22
Background Elevated: #282c37
Background Input: #1f232b
Background Hover: #313543
Background Active: #393f4f

# Brand
Mastodon Purple: #6364FF
Mastodon Purple Hover: #7477FF
Mastodon Purple Active: #5253E0

# Text
Text Primary: #ffffff
Text Secondary: #9baec8
Text Tertiary: #606984
Text Link: #6364FF

# Actions
Boost Color: #2b90d9
Favorite Color: #ca8f04
Bookmark Color: #6364FF

# Semantic
Success: #79bd9a
Warning: #ca8f04
Error: #df405a

# Borders & Radii
Border Default: #393f4f
Border Radius Small: 4px
Border Radius Medium: 8px
Border Radius Avatar: 4px (square-ish)

# Typography
Font Primary: system-ui, sans-serif
Font Size Base: 15px
Font Size Small: 14px
Font Size Large: 16px
Line Height: 22px
```

### Example Prompts

#### Toot/Post Card
```
Create a Mastodon post (toot) card:
- Container: #282c37 background, 1px #393f4f border-bottom
- Padding: 14px 16px
- Avatar: 46px square with 4px radius, left aligned
- Display name: 15px bold #ffffff
- Handle: 15px regular #606984
- Timestamp: 14px #606984, separated by "·"
- Content: 15px #9baec8, line-height 22px
- Links/hashtags: #6364FF color
- Action bar: reply, boost (#2b90d9), favorite (#ca8f04), bookmark, share
- Hover: background lightens to #2c313d
```

#### Content Warning Component
```
Design a content warning wrapper:
- Outer container: 15px font post content as normal
- CW text: #ffffff bold, followed by warning text
- Toggle button: #282c37 background, #9baec8 text
- Button text: "Show more" / "Show less"
- Hidden content: collapsed by default
- When expanded: full content visible below button
- Border: none, but CW indicator visible
```

#### Boost Indicator
```
Create a boosted post indicator:
- Top bar: "🔁 [User] boosted" in #606984, 13px
- Icon: boost icon in #2b90d9 when boosted
- Border-left: 4px solid #2b90d9 (optional style)
- Original post nested below
- Maintain post author's avatar and info
```

#### Compose Modal
```
Design a compose post modal:
- Modal: #282c37 background, 8px radius
- Header: "New post" title, close button
- Avatar: current user, 46px
- Textarea: #282c37, no border, 15px, placeholder "What's on your mind?"
- Content warning toggle: shield icon, #606984
- Media buttons: image, poll, emoji picker
- Character count: "0/500" in #606984
- Visibility dropdown: public, unlisted, followers-only, mentioned only
- Post button: #6364FF, "Post!" text
```

#### Profile Header
```
Design a user profile header:
- Header image: 400px height or gradient fallback
- Avatar: 80px square, 4px radius, -40px overlap
- Display name: 20px bold #ffffff
- Handle: 15px #606984 with instance badge
- Bio: 15px #9baec8
- Stats: Following, Followers, Posts counts
- Follow button: #6364FF if not following, outlined if following
- Instance badge: #393f4f background, #9baec8 text
```

#### Federation Timeline
```
Create a federated timeline column:
- Column header: "Federated timeline" #ffffff, globe icon
- Settings cog icon in header
- Posts from multiple instances
- Instance badges visible on remote posts
- Load more button at bottom
- Streaming indicator when live updating
```

### CSS Variables Template

```css
:root {
  /* Backgrounds */
  --background-base: #191b22;
  --background-elevated: #282c37;
  --background-input: #1f232b;
  --background-hover: #313543;
  --background-active: #393f4f;
  
  /* Brand */
  --mastodon-purple: #6364FF;
  --mastodon-purple-hover: #7477FF;
  --mastodon-purple-active: #5253E0;
  
  /* Text */
  --text-primary: #ffffff;
  --text-secondary: #9baec8;
  --text-tertiary: #606984;
  --text-link: #6364FF;
  
  /* Semantic */
  --color-success: #79bd9a;
  --color-warning: #ca8f04;
  --color-error: #df405a;
  --color-boost: #2b90d9;
  --color-favorite: #ca8f04;
  
  /* Borders */
  --border-color: #393f4f;
  
  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-10: 10px;
  --spacing-14: 14px;
  --spacing-16: 16px;
  --spacing-20: 20px;
  
  /* Radii */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  
  /* Typography */
  --font-primary: system-ui, -apple-system, sans-serif;
  --font-mono: ui-monospace, monospace;
  --font-size-sm: 13px;
  --font-size-base: 15px;
  --font-size-lg: 16px;
  --line-height: 22px;
}
```

---

## Summary

Mastodon's design system embodies the values of the decentralized, open-source social web:

1. **Dark, immersive interface** with layered backgrounds (#191b22 → #282c37 → #393f4f)
2. **Mastodon Purple (#6364FF)** as the distinctive brand accent
3. **Multi-column TweetDeck-style layout** for power users, with single-column alternative
4. **Federation-aware UI patterns** showing instance context and remote content indicators
5. **Privacy-first components** including content warnings, visibility controls, and sensitive media handling
6. **Accessible, ethical design** avoiding dark patterns and engagement manipulation
7. **Clear action semantics** with distinct boost (blue), favorite (gold), and bookmark (purple) colors

When implementing Mastodon-style interfaces, prioritize:
- User autonomy and control over their experience
- Transparency about content origin and federation
- Content warning system as a first-class feature
- Accessible design with proper contrast and keyboard navigation
- Chronological, algorithm-free timeline presentation
- Respect for decentralization and instance diversity
