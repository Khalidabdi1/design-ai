# Midjourney Design System
> AI image generation platform with a dark, gallery-first aesthetic — deep charcoal surfaces, muted gold accents, and image-forward grid UI.

---

## 1. Visual Theme & Atmosphere
Midjourney is where AI art is born. The web interface is designed entirely around the generated image — dark backgrounds recede so that vibrant, detailed AI artwork becomes the centerpiece. The gallery grid is dense and image-forward. A muted gold accent lends a premium, curatorial feel. The UI is intentionally minimal: a prompt input, an infinite image grid, and a clean detail view.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#C9A227` | Brand gold, CTAs, active states |
| `--color-primary-dark` | `#A07D15` | Hover/active |
| `--color-primary-dim` | `rgba(201,162,39,0.12)` | Subtle gold backgrounds |
| `--color-bg-base` | `#0F0F0F` | Page background |
| `--color-bg-sidebar` | `#161616` | Left sidebar |
| `--color-bg-card` | `#1A1A1A` | Card hover/meta overlay |
| `--color-bg-elevated` | `#242424` | Dropdowns, tooltips |
| `--color-border` | `#2E2E2E` | Subtle borders |
| `--color-text-primary` | `#F0F0F0` | Headings, primary text |
| `--color-text-secondary` | `#888888` | Labels, meta text |
| `--color-text-muted` | `#505050` | Placeholders, timestamps |
| `--color-upscale` | `#3B82F6` | Upscale/variation button accent |
| `--color-vary` | `#8B5CF6` | Variation action accent |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 24px | 700 | 1.25 |
| Section Header | 15px | 600 | 1.4 |
| Image Prompt Text | 13px | 400 | 1.5 |
| Metadata Label | 12px | 400 | 1.4 |
| Caption | 11px | 400 | 1.3 |

## 4. Component Stylings
```css
/* Prompt Input */
.prompt-input {
  background: #1A1A1A;
  border: 1px solid #2E2E2E;
  border-radius: 10px;
  padding: 14px 18px;
  font-size: 14px;
  color: #F0F0F0;
  width: 100%;
  resize: none;
  transition: border-color 0.15s;
}
.prompt-input:focus {
  outline: none;
  border-color: #C9A227;
  box-shadow: 0 0 0 3px rgba(201,162,39,0.1);
}
.prompt-input::placeholder { color: #505050; }

/* Submit Button */
.button-imagine {
  background: #C9A227;
  color: #0F0F0F;
  border: none;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-imagine:hover { background: #A07D15; }

/* Image Grid Item */
.image-grid-item {
  position: relative;
  border-radius: 6px;
  overflow: hidden;
  cursor: pointer;
  aspect-ratio: 1;
  background: #1A1A1A;
}
.image-grid-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.2s ease;
}
.image-grid-item:hover img { transform: scale(1.03); }
.image-grid-item__overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 10px;
  background: linear-gradient(transparent, rgba(0,0,0,0.75));
  opacity: 0;
  transition: opacity 0.15s;
}
.image-grid-item:hover .image-grid-item__overlay { opacity: 1; }
.image-grid-item__prompt {
  font-size: 11px;
  color: rgba(255,255,255,0.8);
  line-height: 1.4;
  overflow: hidden;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}

/* Action Buttons (U1–U4, V1–V4) */
.action-btn {
  background: #242424;
  border: 1px solid #2E2E2E;
  border-radius: 6px;
  padding: 6px 12px;
  font-size: 12px;
  font-weight: 600;
  color: #F0F0F0;
  cursor: pointer;
  transition: background 0.1s, border-color 0.1s;
}
.action-btn:hover { background: #2E2E2E; border-color: #3E3E3E; }
.action-btn--upscale { color: #3B82F6; border-color: rgba(59,130,246,0.3); }
.action-btn--vary { color: #8B5CF6; border-color: rgba(139,92,246,0.3); }

/* Rating Buttons */
.rating-btn {
  background: transparent;
  border: none;
  color: #505050;
  cursor: pointer;
  font-size: 18px;
  transition: color 0.12s;
  padding: 4px;
}
.rating-btn:hover { color: #C9A227; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Action button gaps |
| `--spacing-sm` | `8px` | Grid gap |
| `--spacing-md` | `12px` | Sidebar padding |
| `--spacing-lg` | `20px` | Section gaps |
| `--spacing-xl` | `32px` | Page padding |
| `--grid-gap` | `8px` | Image grid gap |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Small elements |
| `--radius-md` | `6px` | Action buttons |
| `--radius-lg` | `10px` | Prompt input |

## 6. Depth & Elevation
```css
.shadow-image { box-shadow: 0 4px 16px rgba(0,0,0,0.6); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.8); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Images are always the dominant visual — let them fill the grid edge to edge
- Show prompt text on image hover as a darkened overlay at the bottom
- Upscale/variation action buttons are color-coded: blue for U, purple for V
- Keep the grid gap tight (8px) to maximize image density

**Don't:**
- Don't add heavy borders around images — the gallery should feel seamless
- Don't use the gold accent for upscale/vary actions — those have their own colors
- Don't truncate prompts in detail view — show them fully

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | 2-column grid; sidebar hidden |
| Tablet | 768px | 3-column grid; sidebar as drawer |
| Desktop | 1024px | 4-column grid + sidebar |
| Wide | 1440px | 5–6 column grid |

## 9. Agent Prompt Guide
```
You are designing for Midjourney — AI image generation platform.
Use a near-black background (#0F0F0F) with images as the dominant visual element.
Grid images are square aspect ratio with tight 8px gaps; prompt text appears on hover as a gradient overlay.
Gold (#C9A227) is the primary accent for the prompt input focus ring and CTA button.
U (upscale) action buttons use blue; V (variation) buttons use purple.
The sidebar is dark and minimal — just navigation links.
Tone is gallery-dark, image-first, and AI-creative.
```
