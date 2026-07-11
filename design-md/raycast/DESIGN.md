# Raycast Design System
> Developer launcher and productivity tool with a dark macOS-native aesthetic — obsidian surfaces, precise typography, and keyboard-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Raycast is purpose-built for power users who never leave the keyboard. The design language is dark, precise, and intentionally minimal — a glass-frosted command palette over a blurred desktop. Every element serves speed: instant feedback, razor-thin lines, and a monochromatic palette punctuated by a single orange-red accent. The aesthetic feels like the best parts of macOS design language pushed to its extreme.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FF6363` | Brand red-orange, highlights, active states |
| `--color-primary-dark` | `#E54545` | Hover/pressed |
| `--color-primary-light` | `#FFE8E8` | Light backgrounds (rare) |
| `--color-bg-base` | `#1C1C1E` | Main window background |
| `--color-bg-elevated` | `#2C2C2E` | Result rows, cards |
| `--color-bg-hover` | `#3A3A3C` | Hovered row |
| `--color-bg-input` | `#0F0F10` | Search input area |
| `--color-border` | `#3A3A3C` | Subtle dividers |
| `--color-text-primary` | `#FFFFFF` | Primary text |
| `--color-text-secondary` | `#EBEBF5CC` | Secondary text (85% white) |
| `--color-text-muted` | `#EBEBF566` | Placeholder, hint text (40%) |
| `--color-kbd` | `#636366` | Keyboard shortcut labels |

## 3. Typography Rules
```css
--font-sans: -apple-system, 'SF Pro Text', 'Inter', sans-serif;
--font-display: -apple-system, 'SF Pro Display', 'Inter', sans-serif;
--font-mono: 'SF Mono', 'JetBrains Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.4;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Section Header | 11px | 600 | 1.2 |
| Result Title | 14px | 500 | 1.4 |
| Result Subtitle | 13px | 400 | 1.3 |
| Search Input | 16px | 400 | 1.4 |
| Keyboard Hint | 11px | 500 | 1.2 |

## 4. Component Stylings
```css
/* Command Window */
.raycast-window {
  background: rgba(28, 28, 30, 0.95);
  backdrop-filter: blur(40px) saturate(1.8);
  border: 0.5px solid rgba(255,255,255,0.12);
  border-radius: 12px;
  width: 640px;
  overflow: hidden;
}

/* Search Input */
.search-input {
  background: transparent;
  border: none;
  padding: 16px 20px;
  font-size: 16px;
  font-weight: 400;
  color: #FFFFFF;
  width: 100%;
  caret-color: #FF6363;
}
.search-input:focus { outline: none; }
.search-input::placeholder { color: rgba(235,235,245,0.4); }

/* Result Row */
.result-row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px 16px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.08s ease;
}
.result-row:hover,
.result-row--active { background: #3A3A3C; }
.result-row--active .result-title { color: #FF6363; }

/* Result Icon */
.result-icon {
  width: 28px;
  height: 28px;
  border-radius: 6px;
  flex-shrink: 0;
}

/* Keyboard Badge */
.kbd {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 2px 6px;
  border-radius: 4px;
  background: #3A3A3C;
  border: 0.5px solid rgba(255,255,255,0.12);
  font-size: 11px;
  font-weight: 500;
  color: #EBEBF5CC;
  font-family: var(--font-sans);
  min-width: 20px;
}

/* Section Divider */
.section-header {
  padding: 8px 16px 4px;
  font-size: 11px;
  font-weight: 600;
  color: rgba(235,235,245,0.4);
  text-transform: uppercase;
  letter-spacing: 0.06em;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--window-width` | `640px` | Fixed command palette width |
| `--input-height` | `54px` | Search bar fixed height |
| `--result-row-height` | `44px` | Standard result row |
| `--spacing-xs` | `4px` | Tight gaps |
| `--spacing-sm` | `8px` | Row padding vertical |
| `--spacing-md` | `12px` | Icon-to-text gap |
| `--spacing-lg` | `16px` | Row horizontal padding |
| `--radius-sm` | `4px` | Kbd badges |
| `--radius-md` | `8px` | Result rows |
| `--radius-lg` | `12px` | Main window |

## 6. Depth & Elevation
```css
.window-shadow { box-shadow: 0 24px 64px rgba(0,0,0,0.7), 0 0 0 0.5px rgba(255,255,255,0.1); }
.result-divider { border-top: 0.5px solid rgba(255,255,255,0.08); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the window width fixed at 640px — this is sacred
- Show keyboard shortcuts on every actionable row, aligned right
- Use the red-orange accent ONLY for the active/selected row title and the caret
- Section headers must be uppercase 11px, muted — never bold

**Don't:**
- Don't add decorative illustrations or gradients
- Don't use more than 2 lines of text in a result row
- Don't show primary buttons — every action is triggered by keyboard
- Don't use light backgrounds inside the command window

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Desktop only | 640px | Fixed-size palette, always centered on screen |
| Max results | — | Show 8 results before scroll |

## 9. Agent Prompt Guide
```
You are designing for Raycast — a keyboard-first developer launcher.
Use a dark obsidian window (#1C1C1E) with frosted-glass blur backdrop.
The only accent color is red-orange (#FF6363), used for active selections and the cursor.
Result rows are 44px tall, 16px horizontal padding, subtle hover background (#3A3A3C).
Keyboard shortcuts appear as small rounded badges (--kbd) aligned to the right.
Section headers are 11px uppercase muted text.
Typography is SF Pro / Inter at 14px, never bold for result text.
Tone is macOS-native, keyboard-first, speed-obsessed.
```
