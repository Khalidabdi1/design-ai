# Pitch Design System
> Collaborative presentation platform with a sleek dark aesthetic — matte black surfaces, vibrant cover accents, and presentation-canvas-first UI.

---

## 1. Visual Theme & Atmosphere
Pitch is what happens when a design team builds a presentation tool. The UI is confident and restrained, stepping back to let the slide content shine. Matte black surfaces frame a bright editing canvas; a vivid coral-pink accent signals active states and brand moments. The overall feel is premium, collaborative, and distinctly modern — closer to Figma than PowerPoint in sensibility.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FF4D4D` | Brand coral-red, CTAs |
| `--color-primary-dark` | `#D93636` | Hover/active primary |
| `--color-primary-light` | `#FFF0F0` | Light-mode badges |
| `--color-accent-purple` | `#7C4DFF` | Secondary accent, templates |
| `--color-bg-base` | `#111111` | App shell background |
| `--color-bg-sidebar` | `#1A1A1A` | Left sidebar, thumbnail rail |
| `--color-bg-card` | `#222222` | Slide thumbnail cards |
| `--color-bg-elevated` | `#2A2A2A` | Dropdowns, tooltips |
| `--color-canvas` | `#FFFFFF` | Slide editing canvas |
| `--color-border` | `#333333` | Default borders |
| `--color-text-primary` | `#F5F5F5` | UI headings, labels |
| `--color-text-secondary` | `#A0A0A0` | Secondary labels |
| `--color-text-muted` | `#606060` | Placeholders, disabled |
| `--color-success` | `#34D399` | Saved, collaborative presence |
| `--color-warning` | `#FBBF24` | Syncing, pending |

## 3. Typography Rules
```css
--font-sans: 'Inter', 'Helvetica Neue', Arial, sans-serif;
--font-display: 'Clash Display', 'Inter', sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 28px;
--font-size-2xl: 40px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| App Header | 14px | 600 | 1.4 |
| Slide Title (template) | 40px | 700 | 1.2 |
| Slide Body (template) | 20px | 400 | 1.5 |
| Sidebar Label | 11px | 600 | 1.3 |
| Toolbar Tooltip | 13px | 500 | 1.4 |
| UI Body | 14px | 400 | 1.5 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FF4D4D;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #D93636; }

/* Slide Thumbnail */
.slide-thumbnail {
  background: #FFFFFF;
  border-radius: 6px;
  border: 2px solid transparent;
  cursor: pointer;
  aspect-ratio: 16/9;
  overflow: hidden;
  transition: border-color 0.12s;
}
.slide-thumbnail:hover { border-color: #555555; }
.slide-thumbnail--active { border-color: #FF4D4D; }

/* Toolbar */
.toolbar {
  background: #1A1A1A;
  border: 1px solid #333333;
  border-radius: 10px;
  padding: 6px 10px;
  display: flex;
  align-items: center;
  gap: 4px;
}
.toolbar-button {
  width: 32px;
  height: 32px;
  border-radius: 6px;
  border: none;
  background: transparent;
  color: #A0A0A0;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: background 0.1s, color 0.1s;
}
.toolbar-button:hover {
  background: #2A2A2A;
  color: #F5F5F5;
}
.toolbar-button--active {
  background: rgba(255,77,77,0.15);
  color: #FF4D4D;
}

/* Collaborator Avatar */
.collab-avatar {
  width: 28px;
  height: 28px;
  border-radius: 50%;
  border: 2px solid #FF4D4D;
  object-fit: cover;
  margin-left: -6px;
}
.collab-avatar:first-child { margin-left: 0; }

/* Template Card */
.template-card {
  border-radius: 8px;
  overflow: hidden;
  cursor: pointer;
  aspect-ratio: 16/9;
  position: relative;
  transition: transform 0.15s;
}
.template-card:hover { transform: scale(1.03); }
.template-card__label {
  position: absolute;
  bottom: 8px;
  left: 8px;
  font-size: 12px;
  font-weight: 600;
  color: #FFFFFF;
  background: rgba(0,0,0,0.5);
  padding: 3px 8px;
  border-radius: 4px;
  backdrop-filter: blur(4px);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Toolbar button gaps |
| `--spacing-sm` | `8px` | Thumbnail list gap |
| `--spacing-md` | `16px` | Panel padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Page gutter |
| `--sidebar-width` | `200px` | Slide thumbnail sidebar |
| `--toolbar-height` | `48px` | Top editor toolbar |
| `--radius-sm` | `4px` | Labels |
| `--radius-md` | `8px` | Buttons, panels |
| `--radius-lg` | `10px` | Toolbar containers |

## 6. Depth & Elevation
```css
.shadow-canvas { box-shadow: 0 8px 40px rgba(0,0,0,0.6); }
.shadow-toolbar { box-shadow: 0 4px 16px rgba(0,0,0,0.5); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the canvas always white — it's the slide, not the app
- Use the coral-red accent for the active slide thumbnail border
- Show collaborator avatars stacked in the top-right of the editor
- Animate slide transitions smoothly (200–300ms ease)

**Don't:**
- Don't use heavy shadows on the toolbar — keep it light and floating
- Don't add decorative backgrounds to the editor shell — let slides stand out
- Don't use more than 2 accent colors in the same UI context

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Presentation view only; editing disabled |
| Tablet | 768px | Minimal editor: canvas + bottom thumbnail strip |
| Desktop | 1024px | Full editor: left thumbnails + canvas + right panel |
| Wide | 1440px | Wider canvas with expanded properties panel |

## 9. Agent Prompt Guide
```
You are designing for Pitch — a collaborative presentation tool.
Use a matte black shell (#111111) with a bright white slide canvas as the hero.
Primary accent is coral-red (#FF4D4D) — for CTAs, active slide borders, and selected states.
The toolbar floats above the canvas as a dark rounded pill with icon buttons.
Slide thumbnails are white 16:9 cards with a red border when active.
Collaborator avatars stack in the top-right, each with a brand-color border.
Tone is premium, design-forward, and collaboration-first.
```
