# Arc Browser Design System
> Innovative browser with a sidebar-first aesthetic — vibrant gradient backgrounds, space-like dark surfaces, and a reimagined tab/space organization UI.

---

## 1. Visual Theme & Atmosphere
Arc from The Browser Company throws out the conventional browser chrome and starts fresh. Tabs live in a collapsible sidebar, URLs disappear after typing, and "Spaces" let you organize context rather than chaos. The design is vibrant and bold: dynamic gradient backgrounds (customizable per Space), a dark vertical sidebar, and whimsical color-forward UI that still feels intentional and calm. It's the most visually distinctive browser ever shipped.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#6B7AFF` | Brand blue-purple |
| `--color-primary-hover` | `#5463E8` | Hover/active |
| `--color-space-1` | `#3D2C8D` | Default space gradient start |
| `--color-space-2` | `#1A1A3E` | Default space gradient end |
| `--color-sidebar-bg` | `rgba(20,20,40,0.85)` | Sidebar background (glass) |
| `--color-sidebar-border` | `rgba(255,255,255,0.08)` | Sidebar right border |
| `--color-tab-bg` | `transparent` | Default tab row |
| `--color-tab-hover` | `rgba(255,255,255,0.08)` | Hovered tab |
| `--color-tab-active` | `rgba(255,255,255,0.14)` | Active/selected tab |
| `--color-text-primary` | `#FFFFFF` | Primary UI text |
| `--color-text-secondary` | `rgba(255,255,255,0.65)` | Secondary labels, domain names |
| `--color-text-muted` | `rgba(255,255,255,0.35)` | Timestamps, hints |
| `--color-url-bar` | `rgba(255,255,255,0.1)` | URL bar background |
| `--color-favicon-border` | `rgba(255,255,255,0.15)` | Favicon container |
| `--color-pinned` | `#6B7AFF` | Pinned tab indicator |

## 3. Typography Rules
```css
--font-sans: -apple-system, 'SF Pro Text', 'Inter', sans-serif;
--font-display: -apple-system, 'SF Pro Display', 'Inter', sans-serif;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 14px;
--font-size-lg: 16px;
--font-size-xl: 20px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.4;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Tab Title | 13px | 400 | 1.4 |
| Tab Domain | 11px | 400 | 1.3 |
| Space Name | 12px | 600 | 1.3 |
| URL Bar | 14px | 400 | 1.4 |
| Omnibox Suggestion | 13px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Space Background */
.space-bg {
  background: linear-gradient(135deg, #3D2C8D 0%, #1A1A3E 60%, #0A0A1E 100%);
  min-height: 100vh;
}

/* Sidebar */
.sidebar {
  width: 240px;
  height: 100vh;
  background: rgba(20, 20, 40, 0.85);
  backdrop-filter: blur(32px) saturate(1.5);
  border-right: 1px solid rgba(255,255,255,0.08);
  display: flex;
  flex-direction: column;
  padding: 12px 8px;
  position: fixed;
  left: 0;
  top: 0;
}

/* Tab Row */
.tab-row {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 6px 10px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.1s ease;
  min-height: 36px;
}
.tab-row:hover { background: rgba(255,255,255,0.08); }
.tab-row--active { background: rgba(255,255,255,0.14); }
.tab-row__title {
  font-size: 13px;
  color: rgba(255,255,255,0.9);
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  flex: 1;
}
.tab-row__favicon {
  width: 16px;
  height: 16px;
  border-radius: 3px;
  flex-shrink: 0;
}

/* Space Badge */
.space-badge {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 4px 8px;
  border-radius: 6px;
  cursor: pointer;
  transition: background 0.1s;
}
.space-badge:hover { background: rgba(255,255,255,0.08); }
.space-badge__dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
}
.space-badge__name {
  font-size: 12px;
  font-weight: 600;
  color: rgba(255,255,255,0.7);
}

/* URL Bar / Omnibox */
.url-bar {
  background: rgba(255,255,255,0.1);
  border: 1px solid rgba(255,255,255,0.12);
  border-radius: 8px;
  padding: 8px 14px;
  font-size: 14px;
  color: #FFFFFF;
  outline: none;
  width: 100%;
  transition: background 0.1s, border-color 0.1s;
}
.url-bar:focus {
  background: rgba(255,255,255,0.15);
  border-color: rgba(107,122,255,0.5);
}
.url-bar::placeholder { color: rgba(255,255,255,0.4); }

/* Pinned Tab Dot */
.pinned-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #6B7AFF;
  flex-shrink: 0;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--sidebar-width` | `240px` | Fixed sidebar (collapsible to 0) |
| `--tab-height` | `36px` | Standard tab row height |
| `--favicon-size` | `16px` | Tab favicon |
| `--spacing-xs` | `4px` | Sidebar item internal gaps |
| `--spacing-sm` | `8px` | Between tab sections |
| `--spacing-md` | `12px` | Sidebar padding |
| `--radius-sm` | `4px` | Small elements |
| `--radius-md` | `8px` | Tab rows, URL bar |
| `--sidebar-blur` | `32px` | Backdrop-filter blur |

## 6. Depth & Elevation
```css
.sidebar-shadow { box-shadow: 4px 0 24px rgba(0,0,0,0.4); }
.omnibox-shadow { box-shadow: 0 8px 32px rgba(0,0,0,0.5); }
.popup-shadow { box-shadow: 0 12px 40px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Use a rich gradient for the Space background — it's the main branding surface
- Keep the sidebar frosted-glass: dark tinted with high blur
- Tab titles truncate with ellipsis — favicons identify tabs visually
- Pinned tabs use a small colored dot, not the full row layout

**Don't:**
- Don't show a traditional top toolbar or tab bar
- Don't use solid opaque backgrounds for the sidebar
- Don't over-saturate gradient colors — keep them deep and space-like
- Don't show the full URL by default — only on focus

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Desktop only | 1024px | Sidebar can collapse; tabs adapt |
| Wide | 1440px | Comfortable sidebar at 240px |

## 9. Agent Prompt Guide
```
You are designing for Arc Browser — a reimagined browser with sidebar-first navigation.
The dominant visual is a deep space-like gradient (dark purple to near-black) filling the entire background.
The sidebar is a frosted-glass panel (blur 32px, dark tinted) with tab rows as compact rounded items.
Tabs show a 16px favicon + title text; active tab has a lighter tinted background.
The URL bar is transparent with a white-tinted background on focus.
Spaces organize tabs into named groups, each with a distinct accent dot.
Tone is vibrant, spatial, and deeply opinionated — no conventional browser chrome.
```
