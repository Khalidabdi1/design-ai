# Pika Design System
> AI video generation platform with a vibrant dark aesthetic — deep backgrounds, electric purple-pink brand accents, and video-canvas-first UI.

---

## 1. Visual Theme & Atmosphere
Pika makes AI video creation feel exciting and accessible. The design is bold and energetic — dark surfaces that contrast with vivid generated video previews, and a gradient pink-to-purple brand that signals creativity and motion. The UI centers on a prompt bar and a video output canvas, keeping the creative workflow front and center.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#E040FB` | Brand magenta, CTAs |
| `--color-primary-dark` | `#C228D9` | Hover/active |
| `--color-secondary` | `#7B2FBE` | Gradient end, secondary accent |
| `--color-gradient` | `linear-gradient(135deg, #E040FB, #7B2FBE)` | Brand gradient |
| `--color-bg-base` | `#0A0A0F` | Page background |
| `--color-bg-card` | `#141420` | Card, panel surfaces |
| `--color-bg-elevated` | `#1E1E30` | Dropdowns, tooltips |
| `--color-border` | `#2A2A40` | Default borders |
| `--color-text-primary` | `#F2F2FF` | Headings, primary text |
| `--color-text-secondary` | `#8B8BAA` | Labels, meta |
| `--color-text-muted` | `#4A4A6A` | Placeholders, disabled |
| `--color-success` | `#34D399` | Generated, complete |
| `--color-error` | `#F87171` | Failed, error |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Caption | 11px | 400 | 1.3 |

## 4. Component Stylings
```css
/* Gradient Button */
.button-generate {
  background: linear-gradient(135deg, #E040FB, #7B2FBE);
  color: #FFFFFF;
  border: none;
  border-radius: 100px;
  padding: 12px 28px;
  font-size: 15px;
  font-weight: 700;
  cursor: pointer;
  transition: opacity 0.15s;
}
.button-generate:hover { opacity: 0.88; }

/* Prompt Input */
.prompt-bar {
  background: #141420;
  border: 1.5px solid #2A2A40;
  border-radius: 100px;
  padding: 14px 24px;
  font-size: 14px;
  color: #F2F2FF;
  width: 100%;
  transition: border-color 0.15s;
}
.prompt-bar:focus {
  outline: none;
  border-color: #E040FB;
  box-shadow: 0 0 0 3px rgba(224,64,251,0.12);
}
.prompt-bar::placeholder { color: #4A4A6A; }

/* Video Preview Card */
.video-card {
  background: #141420;
  border: 1px solid #2A2A40;
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
  transition: border-color 0.15s, transform 0.15s;
}
.video-card:hover {
  border-color: #E040FB;
  transform: translateY(-2px);
}
.video-card__preview {
  aspect-ratio: 16/9;
  background: #0A0A0F;
  position: relative;
}
.video-card__info {
  padding: 10px 12px;
}
.video-card__prompt {
  font-size: 12px;
  color: #8B8BAA;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

/* Generation Progress */
.progress-bar {
  height: 3px;
  background: #2A2A40;
  border-radius: 100px;
  overflow: hidden;
}
.progress-bar__fill {
  height: 100%;
  background: linear-gradient(90deg, #E040FB, #7B2FBE);
  border-radius: 100px;
  transition: width 0.3s ease;
}

/* Style Preset Chip */
.style-chip {
  display: inline-flex;
  align-items: center;
  padding: 5px 12px;
  border-radius: 100px;
  border: 1.5px solid #2A2A40;
  font-size: 12px;
  font-weight: 500;
  color: #8B8BAA;
  cursor: pointer;
  transition: border-color 0.12s, color 0.12s, background 0.12s;
  background: transparent;
}
.style-chip:hover {
  border-color: #E040FB;
  color: #F2F2FF;
}
.style-chip--active {
  border-color: #E040FB;
  background: rgba(224,64,251,0.1);
  color: #E040FB;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Chip gaps |
| `--spacing-sm` | `8px` | Video grid gap |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Page sections |
| `--spacing-xl` | `40px` | Page gutter |
| `--prompt-max-width` | `720px` | Prompt bar max width |
| `--radius-pill` | `100px` | Buttons, inputs, chips |
| `--radius-lg` | `12px` | Video cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 4px 16px rgba(0,0,0,0.5); }
.shadow-hover { box-shadow: 0 0 0 1px #E040FB, 0 8px 24px rgba(224,64,251,0.2); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
```

## 7. Do's and Don'ts
**Do:**
- Use the gradient (pink → purple) for the primary generate CTA
- Style chips for motion style selection (cinematic, anime, etc.)
- Show a gradient progress bar during video generation
- Video cards lift on hover with a magenta border glow

**Don't:**
- Don't use the magenta for error states — use red (#F87171)
- Don't add heavy chrome around the video output — let it breathe
- Don't use pill buttons for anything other than primary generation actions

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single prompt + video result; no grid |
| Tablet | 768px | 2-column video grid |
| Desktop | 1024px | Prompt + 3-column grid of past videos |
| Wide | 1440px | 4-column grid + side panel |

## 9. Agent Prompt Guide
```
You are designing for Pika — AI video generation platform.
Use near-black backgrounds (#0A0A0F) with card surfaces at #141420.
The primary CTA is a pill-shaped button with a gradient fill (pink #E040FB → purple #7B2FBE).
The prompt input is also pill-shaped, dark, with a magenta focus ring.
Video cards are 16:9 with dark backgrounds; they lift with a gradient border on hover.
Style preset chips are pill-shaped with a magenta active state.
Tone is bold, energetic, AI-creative, and motion-forward.
```
