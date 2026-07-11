# Penpot Design System
> Open-source design and prototyping tool with a dark canvas-first aesthetic — obsidian surfaces, violet-indigo accents, and precision design-tool UI patterns.

---

## 1. Visual Theme & Atmosphere
Penpot is an open-source alternative to Figma built on web standards. The design language mirrors a professional design tool: a dark surrounding canvas with white artboards, precise panel controls, and a clean hierarchical layers panel. Violet-indigo accents mark selection states and interactive handles. The UI is dense but organized, built to support hours of focused design work.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#7C3AED` | Brand violet, selection handles, CTAs |
| `--color-primary-dark` | `#6D28D9` | Hover/active |
| `--color-primary-light` | `rgba(124,58,237,0.15)` | Selection overlay |
| `--color-selection` | `#7C3AED` | Bounding box, resize handles |
| `--color-bg-canvas` | `#2C2C2C` | Canvas area background |
| `--color-bg-base` | `#1E1E1E` | App shell background |
| `--color-bg-panel` | `#272727` | Properties/layers panels |
| `--color-bg-input` | `#1A1A1A` | Input fields in panels |
| `--color-bg-elevated` | `#333333` | Dropdowns, tooltips |
| `--color-border` | `#3D3D3D` | Default borders |
| `--color-border-subtle` | `#2E2E2E` | Dividers |
| `--color-artboard` | `#FFFFFF` | Artboard background |
| `--color-text-primary` | `#F0F0F0` | Panel labels, headings |
| `--color-text-secondary` | `#9C9C9C` | Sub-labels, hints |
| `--color-text-muted` | `#555555` | Placeholder, disabled |
| `--color-success` | `#22C55E` | Saved, exported |
| `--color-error` | `#EF4444` | Error states |

## 3. Typography Rules
```css
--font-sans: 'Work Sans', 'Inter', -apple-system, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 10px;
--font-size-sm: 11px;
--font-size-base: 12px;
--font-size-md: 14px;
--font-size-lg: 16px;
--font-size-xl: 20px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.2;
--line-height-base: 1.4;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Panel Section Header | 11px | 600 | 1.2 |
| Property Label | 11px | 500 | 1.3 |
| Layer Name | 12px | 400 | 1.4 |
| Input Value | 12px | 400 | 1.4 |
| Page Title | 12px | 600 | 1.4 |
| Tooltip | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Panel Section Header */
.panel-section-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 16px 6px;
  font-size: 11px;
  font-weight: 600;
  color: #9C9C9C;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  border-bottom: 1px solid #2E2E2E;
}

/* Numeric Input (design values) */
.design-input {
  background: #1A1A1A;
  border: 1px solid #3D3D3D;
  border-radius: 4px;
  padding: 5px 8px;
  font-size: 12px;
  font-family: var(--font-mono);
  color: #F0F0F0;
  text-align: center;
  width: 64px;
  transition: border-color 0.1s;
}
.design-input:focus {
  outline: none;
  border-color: #7C3AED;
  box-shadow: 0 0 0 2px rgba(124,58,237,0.2);
}

/* Layer Row */
.layer-row {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 5px 12px;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.08s;
}
.layer-row:hover { background: #2E2E2E; }
.layer-row--selected { background: rgba(124,58,237,0.15); }
.layer-row__icon { color: #9C9C9C; flex-shrink: 0; }
.layer-row__name {
  font-size: 12px;
  color: #F0F0F0;
  flex: 1;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/* Selection Handle */
.selection-handle {
  width: 8px;
  height: 8px;
  border-radius: 2px;
  background: #FFFFFF;
  border: 1.5px solid #7C3AED;
  position: absolute;
}

/* Toolbar Button */
.toolbar-icon-btn {
  width: 32px;
  height: 32px;
  border-radius: 6px;
  border: none;
  background: transparent;
  color: #9C9C9C;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: background 0.08s, color 0.08s;
}
.toolbar-icon-btn:hover { background: #2E2E2E; color: #F0F0F0; }
.toolbar-icon-btn--active { background: rgba(124,58,237,0.15); color: #7C3AED; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Layer indent, handle offset |
| `--spacing-sm` | `6px` | Input vertical padding |
| `--spacing-md` | `8px` | Between design inputs |
| `--spacing-lg` | `16px` | Panel horizontal padding |
| `--left-panel-width` | `220px` | Layers + pages panel |
| `--right-panel-width` | `248px` | Design properties panel |
| `--toolbar-width` | `48px` | Left tool column |
| `--radius-xs` | `2px` | Selection handles |
| `--radius-sm` | `4px` | Inputs, layer rows |
| `--radius-md` | `6px` | Toolbar buttons |

## 6. Depth & Elevation
```css
.shadow-panel { box-shadow: 2px 0 8px rgba(0,0,0,0.4); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
.shadow-selection { box-shadow: 0 0 0 1px #7C3AED; }
```

## 7. Do's and Don'ts
**Do:**
- Use 10–12px font sizes in panels — design tools are information-dense
- Keep numeric inputs monospace and center-aligned with fixed widths
- Show bounding box + handles in violet on any selection
- Group panel sections with uppercase muted headers

**Don't:**
- Don't use large padding in panels — every pixel counts in a design tool
- Don't use rounded corners larger than 6px in panel UI
- Don't make the artboard compete with the canvas background — it must always be white
- Don't use icon labels — tooltips on hover are sufficient

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Desktop | 1280px | Minimum usable: left panel + canvas + right panel |
| Wide | 1440px | Comfortable default layout |
| Ultra-wide | 1920px | Wider canvas area, same panel widths |

## 9. Agent Prompt Guide
```
You are designing for Penpot — an open-source design and prototyping tool.
UI panels are extremely dense: 11–12px text, tight padding, dark surfaces (#272727).
Left panel shows layers hierarchy; right panel shows design properties in small monospace inputs.
Canvas background is dark (#2C2C2C); artboards are always white.
Selections use violet (#7C3AED) bounding boxes with white resize handles.
Toolbar icons are 32px, icon-only with tooltips on hover.
Tone is precision-first, design-tool-native, and open-source professional.
```
