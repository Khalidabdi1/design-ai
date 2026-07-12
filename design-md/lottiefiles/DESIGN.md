# LottieFiles Design System
> Animation platform and marketplace with a playful, creative aesthetic — vivid teal-green brand, white surfaces, and motion-first UI patterns.

---

## 1. Visual Theme & Atmosphere
LottieFiles celebrates animation and motion. The design is bright, friendly, and joyful — a teal-green brand color that evokes creativity and forward movement. Animation previews are the hero, surrounded by clean white space that lets motion take center stage. The UI is accessible to both developers and designers, balancing a clean consumer aesthetic with practical tooling for integrating Lottie animations.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00C2A8` | Brand teal-green, CTAs |
| `--color-primary-dark` | `#00A08C` | Hover/active primary |
| `--color-primary-light` | `#E0F9F6` | Light backgrounds, badges |
| `--color-secondary` | `#6C5CE7` | Purple accent, premium |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F7F8FC` | Sidebar, alternate areas |
| `--color-bg-player` | `#F0F4F8` | Animation preview background |
| `--color-text-primary` | `#1A1A2E` | Headings, primary text |
| `--color-text-secondary` | `#5C6070` | Body text, labels |
| `--color-text-muted` | `#9EA5B4` | Timestamps, meta |
| `--color-border` | `#E4E8F0` | Default borders |
| `--color-like` | `#EF4444` | Favorites |
| `--color-success` | `#22C55E` | Saved, uploaded |
| `--color-error` | `#EF4444` | Error states |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero Title | 36px | 700 | 1.2 |
| Page Title | 28px | 700 | 1.25 |
| Section Header | 20px | 600 | 1.3 |
| Animation Title | 14px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label / Meta | 13px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #00C2A8;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #00A08C; }

/* Animation Card */
.anim-card {
  background: #FFFFFF;
  border: 1px solid #E4E8F0;
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
  transition: box-shadow 0.15s, transform 0.15s;
}
.anim-card:hover {
  box-shadow: 0 8px 24px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}
.anim-card__preview {
  background: #F0F4F8;
  aspect-ratio: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.anim-card__info {
  padding: 10px 12px;
}
.anim-card__title {
  font-size: 13px;
  font-weight: 600;
  color: #1A1A2E;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.anim-card__author {
  font-size: 11px;
  color: #9EA5B4;
  margin-top: 2px;
}

/* Favorite Button */
.btn-favorite {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  border: none;
  background: rgba(255,255,255,0.9);
  color: #9EA5B4;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: color 0.12s, transform 0.12s;
}
.btn-favorite:hover { transform: scale(1.1); }
.btn-favorite--active { color: #EF4444; }

/* Download Button */
.btn-download {
  display: flex;
  align-items: center;
  gap: 6px;
  background: #00C2A8;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 7px 14px;
  font-size: 13px;
  font-weight: 600;
  cursor: pointer;
}
.btn-download:hover { background: #00A08C; }

/* Format Badge */
.format-badge {
  display: inline-flex;
  padding: 2px 7px;
  border-radius: 4px;
  font-size: 10px;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}
.format-badge--lottie { background: #E0F9F6; color: #00A08C; }
.format-badge--dotlottie { background: #EDE9FE; color: #6C5CE7; }
.format-badge--gif { background: #FEF3C7; color: #D97706; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight gaps |
| `--spacing-sm` | `8px` | Card meta spacing |
| `--spacing-md` | `12px` | Card inner padding |
| `--spacing-lg` | `16px` | Grid gaps |
| `--spacing-xl` | `24px` | Section padding |
| `--spacing-2xl` | `40px` | Page gutter |
| `--grid-cols` | `4–6` | Animation grid columns |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `8px` | Buttons |
| `--radius-lg` | `12px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-hover { box-shadow: 0 8px 24px rgba(0,0,0,0.10); }
.shadow-player { box-shadow: 0 4px 16px rgba(0,0,0,0.08); }
```

## 7. Do's and Don'ts
**Do:**
- Use square (1:1) animation preview areas — Lottie animations are often square
- Add a subtle lift (translateY -2px) on card hover to suggest interactivity
- Show format badges (Lottie, dotLottie, GIF) on every card
- Allow animation to play on card hover

**Don't:**
- Don't use dark preview backgrounds — light (#F0F4F8) lets animation colors show
- Don't crop animations — always use their natural aspect ratio
- Don't use busy backgrounds behind animation previews

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | 2-column grid |
| Tablet | 768px | 3-column grid |
| Desktop | 1024px | 4-column grid |
| Wide | 1440px | 5–6 column grid |

## 9. Agent Prompt Guide
```
You are designing for LottieFiles — animation platform and marketplace.
Use a white background with teal-green (#00C2A8) as the primary brand accent.
Animation cards are square preview + metadata: title and author below.
Card previews use a light gray background (#F0F4F8) to frame animation content.
Format badges (Lottie/dotLottie/GIF) are small uppercase pill labels with color coding.
Cards lift slightly on hover with a subtle shadow.
Tone is playful, creative, motion-first, and approachable.
```
