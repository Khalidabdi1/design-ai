# Vimeo Design System
> Professional video platform with a clean editorial aesthetic — white-first surfaces, rich blue accents, and creator-focused UI patterns.

---

## 1. Visual Theme & Atmosphere
Vimeo is the professional's video platform — where filmmakers, agencies, and creative teams host and share high-quality work. The design is clean, editorial, and image-forward. White and light surfaces create a gallery-like feel that lets video thumbnails breathe. A rich blue accent signals interactivity and brand confidence. The UI is polished without being flashy, striking a balance between tool and creative showcase.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#1AB7EA` | Brand sky blue, CTAs, links |
| `--color-primary-dark` | `#0E9AC5` | Hover/active primary |
| `--color-primary-light` | `#E8F8FD` | Light backgrounds, badges |
| `--color-secondary` | `#00ADEF` | Alternative brand blue |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F8F8F8` | Section backgrounds |
| `--color-bg-dark` | `#17181F` | Dark header, player shell |
| `--color-text-primary` | `#1A1A1A` | Headings, primary |
| `--color-text-secondary` | `#5A5A5A` | Body text, labels |
| `--color-text-muted` | `#A0A0A0` | Meta, timestamps |
| `--color-border` | `#E0E0E0` | Default borders |
| `--color-border-light` | `#F0F0F0` | Subtle dividers |
| `--color-success` | `#20C997` | Uploaded, live |
| `--color-error` | `#FA5252` | Processing error |
| `--color-pro` | `#1AB7EA` | Pro/Plus badge |

## 3. Typography Rules
```css
--font-sans: 'Helvetica Neue', 'Arial', -apple-system, sans-serif;
--font-display: 'Graphik', 'Helvetica Neue', sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 22px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.6;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 36px | 700 | 1.2 |
| Video Title | 22px | 600 | 1.3 |
| Section Header | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.6 |
| Label / Meta | 13px | 400 | 1.4 |
| Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #1AB7EA;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 10px 20px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #0E9AC5; }

/* Video Thumbnail Card */
.video-card {
  cursor: pointer;
  border-radius: 4px;
  overflow: hidden;
}
.video-card__thumbnail {
  aspect-ratio: 16/9;
  background: #17181F;
  border-radius: 4px;
  overflow: hidden;
  position: relative;
}
.video-card__duration {
  position: absolute;
  bottom: 8px;
  right: 8px;
  background: rgba(0,0,0,0.7);
  color: #FFFFFF;
  font-size: 11px;
  font-weight: 600;
  padding: 2px 6px;
  border-radius: 3px;
}
.video-card__info {
  padding: 10px 0;
}
.video-card__title {
  font-size: 15px;
  font-weight: 600;
  color: #1A1A1A;
  line-height: 1.3;
  margin-bottom: 4px;
}
.video-card__meta {
  font-size: 13px;
  color: #A0A0A0;
}

/* Video Player */
.player {
  background: #17181F;
  border-radius: 4px;
  overflow: hidden;
  aspect-ratio: 16/9;
  position: relative;
}
.player__controls {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 16px;
  background: linear-gradient(transparent, rgba(0,0,0,0.7));
}
.player__progress {
  width: 100%;
  height: 4px;
  background: rgba(255,255,255,0.3);
  border-radius: 2px;
  cursor: pointer;
}
.player__progress-fill {
  height: 100%;
  background: #1AB7EA;
  border-radius: 2px;
}

/* Avatar */
.avatar {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  object-fit: cover;
  border: 2px solid #E0E0E0;
}

/* Pro Badge */
.pro-badge {
  display: inline-flex;
  padding: 2px 7px;
  border-radius: 3px;
  font-size: 11px;
  font-weight: 700;
  background: #1AB7EA;
  color: #FFFFFF;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge padding |
| `--spacing-sm` | `8px` | Card meta gap |
| `--spacing-md` | `16px` | Card grid gap |
| `--spacing-lg` | `24px` | Section padding |
| `--spacing-xl` | `40px` | Page gutter |
| `--max-content` | `1200px` | Max content width |
| `--video-grid-cols` | `3–4` | Responsive video grid |
| `--radius-sm` | `3px` | Badges, duration tag |
| `--radius-md` | `4–6px` | Cards, buttons |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.08); }
.shadow-player { box-shadow: 0 8px 32px rgba(0,0,0,0.2); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.18); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the background white — Vimeo is a gallery, not an app
- Show duration as an overlay on the bottom-right of every thumbnail
- Use sky blue only for the progress bar, CTAs, and pro badges
- Present video grids with consistent 16:9 thumbnails

**Don't:**
- Don't use dark backgrounds in the main content area (only in the player)
- Don't clip video thumbnails to non-16:9 ratios
- Don't add busy hover animations — a subtle play icon overlay is enough

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single-column video list |
| Tablet | 768px | 2-column video grid |
| Desktop | 1024px | 3-column video grid with sidebar |
| Wide | 1440px | 4-column grid, larger thumbnails |

## 9. Agent Prompt Guide
```
You are designing for Vimeo — professional video hosting and sharing.
Use a white/light background as the primary surface — this is a video gallery, not an app.
Sky blue (#1AB7EA) is the accent: progress bars, primary buttons, pro badges.
Video thumbnails are always 16:9, with a dark background and a small duration badge in the corner.
The video player itself is black (#17181F) with a blue progress bar.
Typography is Helvetica Neue at 15px base, generous line height.
Tone is editorial, clean, and creator-professional.
```
