# Bluesky Design System
> Decentralized social platform with a clean, airy aesthetic — sky-blue brand accents, white surfaces, and a feed-first interface.

---

## 1. Visual Theme & Atmosphere
Bluesky is a breath of fresh air — literally named for openness. The design is light, clean, and approachable: white backgrounds, a crisp sky-blue accent, and generous typography that makes reading feeds enjoyable. It intentionally avoids the dark patterns of older social platforms. The UI is calm, legible, and genuinely pleasant to use — a social media product designed by people who wanted to get social media right.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#0085FF` | Brand sky blue, CTAs, links |
| `--color-primary-dark` | `#0066CC` | Hover/active primary |
| `--color-primary-light` | `#E8F4FF` | Highlight backgrounds |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F6F8FA` | Sidebar, alternate rows |
| `--color-text-primary` | `#1A1A1A` | Headings, post text |
| `--color-text-secondary` | `#5A6072` | Display names, labels |
| `--color-text-muted` | `#9BA3AF` | Timestamps, metadata |
| `--color-text-link` | `#0085FF` | Inline links, handles |
| `--color-border` | `#E2E8F0` | Card dividers, borders |
| `--color-border-subtle` | `#F1F5F9` | Section dividers |
| `--color-like` | `#EF4444` | Like/heart indicator |
| `--color-repost` | `#22C55E` | Repost indicator |
| `--color-success` | `#22C55E` | Success, following |
| `--color-error` | `#EF4444` | Error states |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 12px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 20px;
--font-size-xl: 26px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
--line-height-post: 1.6;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Post Text | 15px | 400 | 1.6 |
| Display Name | 15px | 700 | 1.4 |
| Handle | 15px | 400 | 1.4 |
| Section Header | 20px | 700 | 1.3 |
| Timestamp | 13px | 400 | 1.3 |
| Button Label | 14px | 600 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #0085FF;
  color: #FFFFFF;
  border: none;
  border-radius: 100px;
  padding: 10px 24px;
  font-size: 15px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #0066CC; }

/* Follow Button */
.button-follow {
  background: #1A1A1A;
  color: #FFFFFF;
  border: none;
  border-radius: 100px;
  padding: 7px 18px;
  font-size: 13px;
  font-weight: 700;
  cursor: pointer;
  transition: opacity 0.15s;
}
.button-follow--following {
  background: transparent;
  color: #1A1A1A;
  border: 1.5px solid #E2E8F0;
}

/* Post Card */
.post-card {
  padding: 16px;
  border-bottom: 1px solid #E2E8F0;
  cursor: pointer;
  transition: background 0.1s;
}
.post-card:hover { background: #F9FAFB; }

/* Post Header */
.post-header {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 6px;
}
.post-avatar {
  width: 42px;
  height: 42px;
  border-radius: 50%;
  flex-shrink: 0;
  object-fit: cover;
}
.post-display-name {
  font-size: 15px;
  font-weight: 700;
  color: #1A1A1A;
}
.post-handle {
  font-size: 14px;
  color: #9BA3AF;
}
.post-timestamp {
  font-size: 13px;
  color: #9BA3AF;
}

/* Post Text */
.post-text {
  font-size: 15px;
  line-height: 1.6;
  color: #1A1A1A;
  margin-bottom: 10px;
}
.post-text a { color: #0085FF; text-decoration: none; }
.post-text a:hover { text-decoration: underline; }

/* Post Actions */
.post-actions {
  display: flex;
  gap: 28px;
  margin-top: 10px;
}
.post-action {
  display: flex;
  align-items: center;
  gap: 5px;
  font-size: 13px;
  color: #9BA3AF;
  cursor: pointer;
  transition: color 0.12s;
  background: none;
  border: none;
  padding: 0;
}
.post-action:hover { color: #0085FF; }
.post-action--liked { color: #EF4444; }
.post-action--reposted { color: #22C55E; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Action icon gaps |
| `--spacing-sm` | `8px` | Post header gaps |
| `--spacing-md` | `16px` | Post card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--feed-max-width` | `600px` | Feed column max width |
| `--sidebar-width` | `280px` | Left sidebar (desktop) |
| `--right-sidebar` | `320px` | Trending/suggestions |
| `--avatar-size` | `42px` | Post avatar |
| `--radius-pill` | `100px` | Buttons |
| `--radius-sm` | `4px` | Inline badges |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 1px 3px rgba(0,0,0,0.05); }
.shadow-dropdown { box-shadow: 0 4px 16px rgba(0,0,0,0.10); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.14); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the feed column centered and narrow (max 600px) for readability
- Use pill-shaped (border-radius 100px) buttons for all primary actions
- Color like/heart actions red and repost actions green when active
- Show handles in muted gray — display names in bold black

**Don't:**
- Don't use dark backgrounds for the main feed — this is a light, open platform
- Don't add algorithmic "recommended" labels without clear attribution
- Don't collapse post action counts — show them always for transparency
- Don't use the blue accent for anything other than CTAs and links

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single column: nav bar + feed, full width |
| Tablet | 768px | Feed + left nav sidebar |
| Desktop | 1024px | Left sidebar + feed + right sidebar |
| Wide | 1440px | Same with comfortable outer margins |

## 9. Agent Prompt Guide
```
You are designing for Bluesky — a decentralized social media platform.
Use a white background with sky blue (#0085FF) as the primary accent for CTAs and links.
Post cards are white with a bottom border divider; hover adds a subtle gray background.
Post avatars are 42px circles; display names are bold, handles are muted gray.
Buttons are pill-shaped (border-radius 100px): blue-fill for primary, dark-fill for follow.
Like actions turn red when active; repost turns green.
Tone is light, open, airy, and community-first.
```
