# TikTok Design System

## 1. Visual Theme & Atmosphere

### Core Identity
TikTok's design is **bold, immersive, and unapologetically Gen-Z**. The interface disappears to let content shine—video is the hero, and everything else exists to amplify creator expression.

### Design Philosophy
- **Content-First**: The UI is invisible until needed. Full-screen video dominates.
- **Effortless Discovery**: Endless vertical scroll removes friction from content consumption.
- **Playful Energy**: The signature cyan-pink gradient injects life and movement.
- **Creator-Centric**: Every element celebrates and empowers creators.
- **Instant Gratification**: One-tap interactions, swipe navigation, zero loading states.

### Mood & Feeling
| Attribute | Expression |
|-----------|------------|
| Energy | High-octane, dynamic, pulsing |
| Personality | Playful, irreverent, bold |
| Accessibility | Effortless, intuitive, addictive |
| Aesthetic | Dark mode native, neon accents, cinematic |
| Generation | Digital-native, trend-forward, authentic |

### Visual Metaphors
- **The Stage**: Every video is a performance; the interface is the darkened theater.
- **The Pulse**: Interactions glow and animate like a heartbeat.
- **The Scroll**: An infinite reel of entertainment, like flipping channels at light speed.

---

## 2. Color Palette & Roles

### Primary Colors

| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| TikTok Black | `#000000` | 0, 0, 0 | Primary background, video container |
| Deep Black | `#121212` | 18, 18, 18 | Secondary surfaces, cards |
| TikTok Cyan | `#25F4EE` | 37, 244, 238 | Accent, highlights, left gradient |
| TikTok Pink | `#FE2C55` | 254, 44, 85 | Accent, likes, right gradient |

### Extended Palette

| Name | Hex | Usage |
|------|-----|-------|
| Surface Dark | `#1A1A1A` | Elevated cards, modals |
| Surface Elevated | `#2A2A2A` | Input fields, buttons |
| Border Subtle | `#333333` | Dividers, subtle borders |
| Text Primary | `#FFFFFF` | Headlines, usernames |
| Text Secondary | `#AAAAAA` | Descriptions, metadata |
| Text Tertiary | `#666666` | Placeholders, disabled |
| Success Green | `#00F076` | Verified badges, success states |
| Warning Yellow | `#FFE135` | Cautions, highlights |
| Error Red | `#FF4444` | Errors, destructive actions |

### The Signature Gradient
```css
/* TikTok Gradient - The Brand Pulse */
background: linear-gradient(135deg, #25F4EE 0%, #FE2C55 100%);

/* Animated Variant */
background: linear-gradient(90deg, #25F4EE, #FE2C55, #25F4EE);
background-size: 200% 100%;
animation: gradient-shift 3s ease infinite;
```

### Color Roles

| Role | Light Environment | Dark Environment |
|------|-------------------|------------------|
| Background | `#FFFFFF` | `#000000` |
| Surface | `#F5F5F5` | `#121212` |
| Primary Action | `#FE2C55` | `#FE2C55` |
| Secondary Action | `#25F4EE` | `#25F4EE` |
| Interactive | `#FFFFFF` | `#FFFFFF` |
| Like Active | `#FE2C55` | `#FE2C55` (with glow) |
| Follow Button | `#FE2C55` | `#FE2C55` |
| Following State | `#2F2F2F` | `#2F2F2F` |

### Glow Effects
```css
/* Pink Glow - Likes, Hearts */
box-shadow: 0 0 20px rgba(254, 44, 85, 0.6);

/* Cyan Glow - Secondary Highlights */
box-shadow: 0 0 20px rgba(37, 244, 238, 0.6);

/* Dual Glow - Special States */
box-shadow: 
  -3px 0 15px rgba(37, 244, 238, 0.5),
  3px 0 15px rgba(254, 44, 85, 0.5);
```

---

## 3. Typography Rules

### Font Stack
```css
font-family: 'TikTok Sans', 'Proxima Nova', -apple-system, BlinkMacSystemFont, 
             'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| Display | 32px | 700 | 1.2 | -0.02em |
| Headline 1 | 24px | 700 | 1.3 | -0.01em |
| Headline 2 | 20px | 600 | 1.3 | 0 |
| Title | 18px | 600 | 1.4 | 0 |
| Body Large | 16px | 400 | 1.5 | 0 |
| Body | 14px | 400 | 1.5 | 0 |
| Caption | 12px | 400 | 1.4 | 0.01em |
| Micro | 10px | 500 | 1.3 | 0.02em |

### Typography Styles

```css
/* Username - Bold, Attention-Grabbing */
.username {
  font-size: 16px;
  font-weight: 700;
  color: #FFFFFF;
  line-height: 1.3;
}

/* Handle - Secondary, Subtle */
.handle {
  font-size: 14px;
  font-weight: 400;
  color: #AAAAAA;
}

/* Video Description - Readable, Truncatable */
.description {
  font-size: 14px;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 1.5;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  overflow: hidden;
}

/* Hashtag - Interactive, Highlighted */
.hashtag {
  font-size: 14px;
  font-weight: 600;
  color: #FFFFFF;
}

/* Engagement Count - Compact, Bold */
.count {
  font-size: 12px;
  font-weight: 700;
  color: #FFFFFF;
  text-align: center;
}

/* Sound Name - Marquee Style */
.sound-name {
  font-size: 14px;
  font-weight: 500;
  color: #FFFFFF;
  white-space: nowrap;
}
```

### Text Treatment Rules
1. **Usernames**: Always white, always bold
2. **Descriptions**: Max 2 lines on feed, expandable on tap
3. **Hashtags**: Bold weight, no # color differentiation needed
4. **Numbers**: Use compact notation (1.2M, 45.3K)
5. **Timestamps**: Relative time (2h ago, 3d)

---

## 4. Component Stylings

### Video Container
```css
.video-container {
  width: 100%;
  height: 100vh;
  background: #000000;
  position: relative;
  overflow: hidden;
}

.video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### Action Bar (Right Side)
```css
.action-bar {
  position: absolute;
  right: 12px;
  bottom: 120px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}

.action-button {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
}

.action-icon {
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #FFFFFF;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.5));
}

.action-count {
  font-size: 12px;
  font-weight: 700;
  color: #FFFFFF;
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.5);
}
```

### Like Button States
```css
/* Default */
.like-button {
  color: #FFFFFF;
  transition: all 0.2s ease;
}

/* Liked - Pink with Glow */
.like-button.active {
  color: #FE2C55;
  filter: drop-shadow(0 0 8px rgba(254, 44, 85, 0.8));
  animation: like-pop 0.3s ease;
}

@keyframes like-pop {
  0% { transform: scale(1); }
  50% { transform: scale(1.3); }
  100% { transform: scale(1); }
}
```

### Creator Profile Avatar
```css
.creator-avatar {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  border: 2px solid #FFFFFF;
  position: relative;
}

.follow-badge {
  position: absolute;
  bottom: -6px;
  left: 50%;
  transform: translateX(-50%);
  width: 20px;
  height: 20px;
  background: #FE2C55;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  color: #FFFFFF;
  border: 2px solid #000000;
}
```

### Follow Button
```css
/* Default - Follow */
.follow-button {
  background: #FE2C55;
  color: #FFFFFF;
  border: none;
  border-radius: 4px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  min-width: 88px;
}

/* Following State */
.follow-button.following {
  background: #2F2F2F;
  border: 1px solid #FFFFFF;
}

/* Friends State */
.follow-button.friends {
  background: transparent;
  border: 1px solid #FFFFFF;
}
```

### Sound/Music Indicator
```css
.sound-indicator {
  position: absolute;
  bottom: 20px;
  left: 12px;
  right: 80px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.music-icon {
  width: 16px;
  height: 16px;
  color: #FFFFFF;
}

.sound-name {
  flex: 1;
  overflow: hidden;
}

.sound-marquee {
  display: inline-block;
  white-space: nowrap;
  animation: marquee 8s linear infinite;
}

@keyframes marquee {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

.spinning-disc {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  animation: spin 3s linear infinite;
}

@keyframes spin {
  100% { transform: rotate(360deg); }
}
```

### Bottom Navigation
```css
.bottom-nav {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 56px;
  background: #000000;
  display: flex;
  align-items: center;
  justify-content: space-around;
  padding-bottom: env(safe-area-inset-bottom);
  border-top: 1px solid #1A1A1A;
}

.nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  color: #FFFFFF;
  opacity: 0.6;
}

.nav-item.active {
  opacity: 1;
}

.nav-item-label {
  font-size: 10px;
  font-weight: 500;
}

/* Create Button - Center, Gradient */
.create-button {
  width: 48px;
  height: 32px;
  border-radius: 8px;
  background: #FFFFFF;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}

.create-button::before {
  content: '';
  position: absolute;
  left: -3px;
  top: 0;
  bottom: 0;
  width: 48px;
  border-radius: 8px;
  background: #25F4EE;
  z-index: -1;
}

.create-button::after {
  content: '';
  position: absolute;
  right: -3px;
  top: 0;
  bottom: 0;
  width: 48px;
  border-radius: 8px;
  background: #FE2C55;
  z-index: -2;
}

.create-icon {
  font-size: 24px;
  font-weight: 300;
  color: #000000;
}
```

### Comments Modal
```css
.comments-modal {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  height: 60vh;
  background: #121212;
  border-radius: 12px 12px 0 0;
  animation: slide-up 0.3s ease;
}

.comments-header {
  padding: 16px;
  text-align: center;
  border-bottom: 1px solid #2A2A2A;
}

.comment-item {
  display: flex;
  gap: 12px;
  padding: 12px 16px;
}

.comment-avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
}

.comment-content {
  flex: 1;
}

.comment-actions {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
}
```

### Search & Discovery
```css
.search-bar {
  background: #2A2A2A;
  border-radius: 4px;
  padding: 10px 16px;
  display: flex;
  align-items: center;
  gap: 8px;
}

.search-input {
  background: transparent;
  border: none;
  color: #FFFFFF;
  font-size: 16px;
  flex: 1;
}

.search-input::placeholder {
  color: #666666;
}

.trending-tag {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 8px 12px;
  background: #1A1A1A;
  border-radius: 4px;
  color: #FFFFFF;
  font-size: 14px;
}
```

### Creator Profile Page
```css
.profile-header {
  padding: 20px;
  text-align: center;
}

.profile-avatar-large {
  width: 96px;
  height: 96px;
  border-radius: 50%;
  margin-bottom: 12px;
}

.profile-username {
  font-size: 20px;
  font-weight: 700;
  color: #FFFFFF;
}

.profile-stats {
  display: flex;
  justify-content: center;
  gap: 32px;
  margin: 16px 0;
}

.stat-item {
  text-align: center;
}

.stat-number {
  font-size: 18px;
  font-weight: 700;
  color: #FFFFFF;
}

.stat-label {
  font-size: 12px;
  color: #AAAAAA;
}

.profile-actions {
  display: flex;
  justify-content: center;
  gap: 8px;
  margin-top: 16px;
}

.message-button {
  width: 44px;
  height: 44px;
  border-radius: 4px;
  border: 1px solid #2F2F2F;
  background: transparent;
  color: #FFFFFF;
}

.video-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2px;
}

.video-thumbnail {
  aspect-ratio: 9/16;
  background: #1A1A1A;
  position: relative;
}

.thumbnail-views {
  position: absolute;
  bottom: 4px;
  left: 4px;
  font-size: 12px;
  color: #FFFFFF;
  display: flex;
  align-items: center;
  gap: 4px;
}
```

---

## 5. Layout Principles

### Feed Layout (For You Page)
```
+---------------------------+
|    Status Bar (System)    |
+---------------------------+
| For You | Following  [Q]  |  <- Tab Bar
+---------------------------+
|                           |
|                           |
|                           |
|    FULL SCREEN VIDEO      |
|         (100vh)           |
|                           |
|           [Avatar]        |  <- Right: Action Bar
|           [Heart]         |     (Profile, Like,
|           [Comment]       |      Comment, Bookmark,
|           [Bookmark]      |      Share)
|           [Share]         |
|                           |
| @username                 |
| Description text...       |  <- Bottom Left: Info
| #hashtag #viral           |
| [Music Icon] Song Name    |
|                           |
+---------------------------+
| [Home][Discover][+][Inbox]|  <- Bottom Nav
|        [Profile]          |
+---------------------------+
```

### Spacing System
```css
--spacing-xs: 4px;
--spacing-sm: 8px;
--spacing-md: 12px;
--spacing-lg: 16px;
--spacing-xl: 20px;
--spacing-2xl: 24px;
--spacing-3xl: 32px;
```

### Safe Zones
```css
/* Video Content Safe Area */
.video-safe-area {
  /* Keep important video content away from UI overlays */
  padding-top: 80px;      /* Status bar + tabs */
  padding-bottom: 180px;  /* Video info + nav */
  padding-right: 60px;    /* Action bar */
  padding-left: 16px;
}

/* Action Bar Positioning */
.action-bar {
  right: 12px;
  bottom: calc(56px + 120px); /* nav height + info height */
}

/* Video Info Positioning */
.video-info {
  left: 12px;
  right: 80px;
  bottom: calc(56px + 20px); /* nav + padding */
}
```

### Grid Systems
```css
/* Profile Video Grid */
.video-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2px;
}

/* Discovery Grid - Mixed */
.discovery-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 8px;
  padding: 8px;
}

/* Comments List */
.comments-list {
  display: flex;
  flex-direction: column;
  gap: 0; /* Items handle their own spacing */
}
```

### Scroll Behavior
```css
/* Vertical Video Scroll - Snap to Each Video */
.feed-container {
  scroll-snap-type: y mandatory;
  overflow-y: scroll;
  height: 100vh;
}

.video-container {
  scroll-snap-align: start;
  scroll-snap-stop: always;
  height: 100vh;
}

/* Horizontal Tab Scroll */
.tabs-container {
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scrollbar-width: none;
}

.tab {
  scroll-snap-align: center;
}
```

### Z-Index Layers
```css
--z-video: 1;
--z-overlay: 10;
--z-action-bar: 20;
--z-video-info: 20;
--z-header: 30;
--z-bottom-nav: 30;
--z-modal-backdrop: 40;
--z-modal: 50;
--z-toast: 60;
--z-loading: 70;
```

---

## 6. Depth & Elevation

### Shadow System
TikTok uses minimal shadows in favor of darkness and glow effects.

```css
/* Text Shadow - For legibility on video */
.text-overlay {
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.5);
}

/* Icon Shadow - Subtle depth */
.icon-overlay {
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.5));
}

/* Modal Shadow */
.modal {
  box-shadow: 0 -4px 20px rgba(0, 0, 0, 0.5);
}

/* Card Shadow (Light Mode) */
.card-light {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}
```

### Glow Effects (Signature)
```css
/* Like Glow */
.like-active {
  filter: drop-shadow(0 0 8px rgba(254, 44, 85, 0.8));
}

/* Cyan Accent Glow */
.cyan-glow {
  filter: drop-shadow(0 0 8px rgba(37, 244, 238, 0.8));
}

/* Dual Brand Glow */
.brand-glow {
  box-shadow: 
    -4px 0 12px rgba(37, 244, 238, 0.5),
    4px 0 12px rgba(254, 44, 85, 0.5);
}

/* Pulsing Glow Animation */
@keyframes pulse-glow {
  0%, 100% {
    filter: drop-shadow(0 0 8px rgba(254, 44, 85, 0.6));
  }
  50% {
    filter: drop-shadow(0 0 16px rgba(254, 44, 85, 0.9));
  }
}
```

### Blur Effects
```css
/* Background Blur - Modals */
.modal-backdrop {
  backdrop-filter: blur(20px);
  background: rgba(0, 0, 0, 0.7);
}

/* Frosted Glass Effect */
.glass-surface {
  background: rgba(18, 18, 18, 0.8);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}

/* Video Blur - Loading State */
.video-blur {
  filter: blur(20px);
  transform: scale(1.1);
}
```

### Elevation Hierarchy
| Level | Usage | Treatment |
|-------|-------|-----------|
| 0 | Video background | Pure black, no shadow |
| 1 | Feed content | Overlay on video |
| 2 | Cards, surfaces | Subtle elevation |
| 3 | Bottom nav, headers | Fixed, slight shadow |
| 4 | Modals, sheets | Strong shadow + backdrop |
| 5 | Toasts, tooltips | Floating, glow optional |

---

## 7. Do's and Don'ts

### Do's

**Content & Layout**
- Let video content be the hero - UI should complement, not compete
- Use full-screen, edge-to-edge video display
- Implement snap scrolling for seamless feed navigation
- Keep action buttons within thumb reach (bottom-right)
- Use vertical aspect ratio (9:16) as the primary format

**Color & Branding**
- Use the cyan-pink gradient sparingly for maximum impact
- Apply glow effects to active states (likes, notifications)
- Maintain high contrast for text overlays on video
- Default to dark mode - it's the native experience
- Use pure black (#000000) for true OLED blacks

**Typography**
- Keep usernames bold and prominent
- Truncate long descriptions with "...more" expansion
- Use compact number notation (1.2M, not 1,200,000)
- Ensure text shadows for legibility on any video background

**Interactions**
- Double-tap to like - make it feel rewarding
- Animate the heart with scale and glow
- Use haptic feedback on key interactions
- Auto-play videos on scroll (muted by default on web)
- Show loading states that don't interrupt content flow

**Creator Focus**
- Make follow buttons highly visible and accessible
- Show creator profile pics with clear tap targets
- Display engagement counts prominently
- Highlight music/sound usage with spinning disc animation

### Don'ts

**Content & Layout**
- Don't use horizontal video layouts in the main feed
- Don't obscure video content with heavy UI overlays
- Don't use pagination - always infinite scroll
- Don't show empty states without engaging content
- Don't break the immersive full-screen experience

**Color & Branding**
- Don't overuse the gradient - it loses impact
- Don't use competing accent colors
- Don't apply glow effects to inactive states
- Don't use light backgrounds in the main feed
- Don't use gray or muted versions of brand colors

**Typography**
- Don't use small, hard-to-read text over video
- Don't display full numbers (show 1.2M not 1,200,000)
- Don't wrap usernames to multiple lines
- Don't use decorative fonts
- Don't center-align body text or descriptions

**Interactions**
- Don't require multiple taps for common actions
- Don't use boring, static interactions
- Don't show intrusive loading spinners
- Don't interrupt video playback unnecessarily
- Don't use slow, heavy animations

**Creator Focus**
- Don't hide creator information
- Don't make following require multiple steps
- Don't deprioritize engagement indicators
- Don't use generic placeholder avatars
- Don't separate sound/music from its creator context

### Common Pitfalls

| Mistake | Better Approach |
|---------|-----------------|
| Horizontal scroll for videos | Vertical snap-scroll feed |
| Small action buttons | 44px+ touch targets |
| Static like button | Animated pop + glow |
| Generic loading spinner | Skeleton or content blur |
| Heavy navigation UI | Minimal bottom nav + gestures |
| Text without shadow | Text-shadow for all overlays |
| Muted brand colors | Vibrant cyan and pink |
| Square video thumbnails | 9:16 aspect ratio |

---

## 8. Responsive Behavior

### Breakpoints
```css
/* TikTok is mobile-first, with desktop as secondary */
--breakpoint-mobile: 480px;
--breakpoint-tablet: 768px;
--breakpoint-desktop: 1024px;
--breakpoint-wide: 1280px;
```

### Mobile (Primary - < 768px)
```css
.feed-mobile {
  /* Full-screen, single-column video feed */
  width: 100vw;
  height: 100vh;
}

.video-container-mobile {
  width: 100%;
  height: 100vh;
  scroll-snap-align: start;
}

.action-bar-mobile {
  position: absolute;
  right: 12px;
  bottom: 120px;
}

.bottom-nav-mobile {
  position: fixed;
  bottom: 0;
  height: 56px;
  padding-bottom: env(safe-area-inset-bottom);
}
```

### Tablet (768px - 1024px)
```css
.feed-tablet {
  /* Centered video with side margins */
  max-width: 500px;
  margin: 0 auto;
  height: 100vh;
}

.video-container-tablet {
  border-radius: 12px;
  margin: 8px;
  height: calc(100vh - 16px);
}

.bottom-nav-tablet {
  max-width: 500px;
  margin: 0 auto;
  border-radius: 16px 16px 0 0;
}
```

### Desktop (> 1024px)
```css
.layout-desktop {
  display: grid;
  grid-template-columns: 240px 1fr 320px;
  height: 100vh;
}

/* Left Sidebar Navigation */
.sidebar-left {
  background: #121212;
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.nav-item-desktop {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 16px;
  border-radius: 8px;
  color: #FFFFFF;
  font-size: 18px;
}

.nav-item-desktop:hover {
  background: #2A2A2A;
}

/* Center Feed - Constrained Width */
.feed-desktop {
  max-width: 480px;
  margin: 0 auto;
  padding: 20px;
}

.video-container-desktop {
  border-radius: 16px;
  overflow: hidden;
  aspect-ratio: 9/16;
  max-height: calc(100vh - 100px);
}

/* Right Sidebar - Suggestions */
.sidebar-right {
  background: #121212;
  padding: 20px;
}
```

### Container Queries (Modern)
```css
@container feed (max-width: 480px) {
  .video-info {
    padding: 12px;
    font-size: 14px;
  }
  
  .action-bar {
    gap: 16px;
  }
}

@container feed (min-width: 481px) {
  .video-info {
    padding: 20px;
    font-size: 16px;
  }
  
  .action-bar {
    gap: 24px;
  }
}
```

### Touch vs Mouse Adaptation
```css
/* Touch Devices - Larger Targets */
@media (pointer: coarse) {
  .action-button {
    min-width: 44px;
    min-height: 44px;
  }
  
  .follow-button {
    padding: 10px 20px;
  }
}

/* Mouse Devices - Hover States */
@media (hover: hover) {
  .action-button:hover {
    transform: scale(1.1);
  }
  
  .video-thumbnail:hover .play-overlay {
    opacity: 1;
  }
  
  .follow-button:hover {
    background: #E01E4A;
  }
}
```

### Safe Areas
```css
/* iOS Notch & Home Indicator */
.video-container {
  padding-top: env(safe-area-inset-top);
}

.bottom-nav {
  padding-bottom: env(safe-area-inset-bottom);
}

/* Android Navigation */
@supports (padding-bottom: env(safe-area-inset-bottom)) {
  .bottom-nav {
    padding-bottom: max(env(safe-area-inset-bottom), 8px);
  }
}
```

---

## 9. Agent Prompt Guide

### Core Design Prompt
```
You are designing a TikTok-style interface. Follow these principles:

VISUAL IDENTITY:
- Dark mode native: Primary black (#000000), surfaces (#121212)
- Signature gradient: Cyan (#25F4EE) to Pink (#FE2C55)
- Full-screen, video-first, immersive experience
- Content is the hero - UI should be minimal and supportive

LAYOUT:
- Vertical scroll, snap-to-video navigation
- Right-side action bar (like, comment, share, bookmark)
- Bottom left video info (username, description, sound)
- Bottom navigation with centered create button
- Mobile-first, 9:16 aspect ratio focus

INTERACTIONS:
- Double-tap to like with heart animation and glow
- Swipe up/down to navigate between videos
- Tap to pause/play video
- All interactions should feel instant and rewarding

TYPOGRAPHY:
- TikTok Sans or system fonts
- Bold usernames, compact engagement numbers
- Text shadows for legibility on video
- Max 2 lines for descriptions with expand option
```

### Component Generation Prompts

**Video Feed Card**
```
Create a TikTok video feed component:
- Full viewport height, edge-to-edge video
- Black background (#000000) with video covering full area
- Right action bar: avatar (48px), like, comment, bookmark, share
- Like count with glow effect when active (#FE2C55)
- Bottom left: @username (bold), description (2 lines max), sound with marquee
- Spinning album cover for sound indicator
- All text with drop shadow for video legibility
```

**Engagement Button**
```
Create a TikTok action button (like/comment/share):
- Vertical stack: icon (24px) + count below
- White icons with drop-shadow on dark video
- Active state: color fill + glow effect
- Like: #FE2C55 with scale+glow animation
- Touch target minimum 44px
- Count in compact notation (1.2K, 3.4M)
```

**Create Button (Plus)**
```
Create the TikTok plus/create button:
- Rectangle with rounded corners (48x32px)
- White center layer with "+" icon
- Cyan layer offset left (-3px)
- Pink layer offset right (+3px)
- Creates layered 3D gradient effect
- Icon is black on white background
```

**Follow Button**
```
Create TikTok follow button:
- Default: #FE2C55 background, white text "Follow"
- Following: #2F2F2F background, white border, "Following"
- Friends: transparent, white border, "Friends"
- Min width 88px, height 36px, border-radius 4px
- Bold text, 14px font size
```

**Sound/Music Bar**
```
Create TikTok sound indicator:
- Music note icon (16px)
- Sound name with marquee animation (8s loop)
- Spinning album art disc on right (44px)
- White text with subtle shadow
- Positioned bottom left, above navigation
```

### Layout Generation Prompts

**For You Page**
```
Create TikTok For You page layout:
- Full screen video container (100vh)
- Top tabs: "For You | Following" with underline indicator
- Search icon top right
- Video snaps to viewport on scroll
- Action bar positioned right, thumb-reachable
- Video info positioned bottom left
- Bottom navigation: Home, Discover, Create(+), Inbox, Profile
- Create button uses signature cyan-pink layered style
```

**Profile Page**
```
Create TikTok profile page:
- Header with large avatar (96px), username, handle
- Stats row: Following, Followers, Likes (centered)
- Action row: Follow button, Message icon, Arrow icon
- Tab bar: Videos, Liked, Bookmarks (with icons)
- 3-column grid of video thumbnails
- Each thumbnail shows view count with play icon
- 9:16 aspect ratio for thumbnails
- 2px gap between grid items
```

**Comments Modal**
```
Create TikTok comments bottom sheet:
- Slides up from bottom, 60% viewport height
- Dark surface (#121212) with rounded top corners
- Header: "X comments" centered, X close button
- Comment list with avatar (36px), username, text, time
- Like button per comment with count
- Reply functionality
- Bottom input: avatar, text field, emoji, send button
```

### Animation Specifications
```
TikTok Animation Guidelines:

LIKE ANIMATION:
- Scale from 1 → 1.3 → 1 (0.3s ease)
- Add glow: drop-shadow(0 0 8px rgba(254, 44, 85, 0.8))
- Optional: spawn floating hearts from tap point

SCROLL SNAP:
- scroll-snap-type: y mandatory
- scroll-snap-align: start
- scroll-snap-stop: always
- Smooth momentum scrolling

SOUND MARQUEE:
- translateX from 0% to -50% (8s linear infinite)
- Duplicate text for seamless loop

SPINNING DISC:
- rotate 360deg (3s linear infinite)
- Pause animation when video paused

MODAL SLIDE:
- translateY from 100% to 0 (0.3s ease-out)
- Backdrop fade from 0 to 0.7

FOLLOW BUTTON:
- Background transition (0.2s ease)
- Optional subtle scale on press (0.95)
```

### State Handling
```
TikTok State Patterns:

VIDEO STATES:
- Loading: blurred thumbnail with subtle pulse
- Playing: no UI indicator (full immersion)
- Paused: play icon center, UI stays visible
- Error: retry button with message

LIKE STATES:
- Default: white heart outline
- Liked: filled pink heart with glow, animated pop
- Processing: subtle pulse animation

FOLLOW STATES:
- Not following: pink "Follow" button
- Following: gray "Following" button
- Mutual: outline "Friends" button
- Processing: loading spinner in button

COMMENT STATES:
- Default: comment icon with count
- New comments: subtle dot indicator
- Loading: skeleton comments
- Empty: "Be the first to comment"

SOUND STATES:
- Playing: spinning disc, marquee active
- Muted: mute icon overlay
- No sound: hide sound bar entirely
```

### Accessibility Notes
```
TikTok Accessibility Requirements:

CONTRAST:
- Text overlays must have shadows for video legibility
- Minimum 4.5:1 contrast for essential UI
- Active states clearly distinguishable

TOUCH TARGETS:
- Minimum 44x44px for all interactive elements
- Action bar icons adequately spaced (20px gap)

MOTION:
- Respect prefers-reduced-motion
- Provide pause controls for video
- Stop marquee on user interaction

SCREEN READERS:
- Announce video creator and description
- Include engagement counts in labels
- Describe action results (liked, followed)

KEYBOARD:
- Arrow keys for video navigation
- Space/Enter for play/pause
- Tab through action buttons
- Escape to close modals
```

---

## Quick Reference

### Essential Colors
```css
--tiktok-black: #000000;
--tiktok-surface: #121212;
--tiktok-cyan: #25F4EE;
--tiktok-pink: #FE2C55;
--tiktok-white: #FFFFFF;
--tiktok-gray: #AAAAAA;
```

### Essential Spacing
```css
--space-xs: 4px;
--space-sm: 8px;
--space-md: 12px;
--space-lg: 16px;
--space-xl: 20px;
```

### Essential Animations
```css
@keyframes like-pop {
  0% { transform: scale(1); }
  50% { transform: scale(1.3); }
  100% { transform: scale(1); }
}

@keyframes spin {
  100% { transform: rotate(360deg); }
}

@keyframes marquee {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}
```

### Essential Shadows
```css
--shadow-text: 0 1px 3px rgba(0, 0, 0, 0.5);
--shadow-icon: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.5));
--glow-pink: drop-shadow(0 0 8px rgba(254, 44, 85, 0.8));
--glow-cyan: drop-shadow(0 0 8px rgba(37, 244, 238, 0.8));
```
