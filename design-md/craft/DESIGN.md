# Craft Design System
> Modern document editor with a clean, minimal aesthetic — white canvas, soft brand blue, and content-first UI.

---

## 1. Visual Theme & Atmosphere
Craft is a beautiful document and notes app that treats writing as an art form. The interface is exceptionally clean — a white or near-white canvas that recedes to put the reader's focus entirely on the content. Soft blue accents mark interactive elements without competing with the writing. The UI supports nesting, blocks, and rich media while maintaining a serene, magazine-quality feel. It bridges journaling, note-taking, and document creation in one polished surface.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#007AFF` | Brand blue, CTAs, links, active states |
| `--color-primary-dark` | `#005EC4` | Hover/active |
| `--color-primary-dim` | `rgba(0,122,255,0.1)` | Selection, highlight backgrounds |
| `--color-bg-base` | `#FFFFFF` | Page/canvas background |
| `--color-bg-surface` | `#F8F8F8` | Sidebar, panel backgrounds |
| `--color-bg-block` | `#F3F4F6` | Block/card surfaces |
| `--color-border` | `#E8E8E8` | Default borders |
| `--color-border-subtle` | `#F0F0F0` | Block separators |
| `--color-text-primary` | `#1A1A1A` | Body text, headings |
| `--color-text-secondary` | `#6B6B6B` | Labels, placeholders |
| `--color-text-muted` | `#AAAAAA` | Timestamps, disabled |
| `--color-text-link` | `#007AFF` | Inline links |
| `--color-success` | `#34C759` | Complete, published |
| `--color-error` | `#FF3B30` | Error states |
| `--color-tag` | `#FF9500` | Tag highlights |

## 3. Typography Rules
```css
--font-text: 'New York', 'Georgia', serif;
--font-sans: 'SF Pro Text', 'Inter', -apple-system, sans-serif;
--font-mono: 'SF Mono', 'JetBrains Mono', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 16px;
--font-size-md: 18px;
--font-size-h3: 20px;
--font-size-h2: 24px;
--font-size-h1: 30px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.3;
--line-height-base: 1.6;
--line-height-body: 1.75;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| H1 | 30px | 700 | 1.25 |
| H2 | 24px | 700 | 1.3 |
| H3 | 20px | 600 | 1.35 |
| Body | 16px | 400 | 1.75 |
| Sidebar Label | 13px | 400 | 1.4 |
| Caption | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Document Canvas */
.document-canvas {
  max-width: 700px;
  margin: 0 auto;
  padding: 60px 40px;
  font-family: var(--font-text);
  font-size: 16px;
  line-height: 1.75;
  color: #1A1A1A;
}

/* Block Container */
.block {
  position: relative;
  padding: 4px 0;
  border-radius: 6px;
  transition: background 0.1s;
}
.block:hover { background: rgba(0,122,255,0.04); }
.block--selected { background: rgba(0,122,255,0.08); }

/* Card Block */
.card-block {
  background: #F3F4F6;
  border-radius: 10px;
  padding: 16px 20px;
  margin: 8px 0;
  border: 1px solid #E8E8E8;
  cursor: pointer;
  transition: box-shadow 0.15s;
}
.card-block:hover { box-shadow: 0 4px 12px rgba(0,0,0,0.08); }
.card-block__title {
  font-size: 15px;
  font-weight: 600;
  color: #1A1A1A;
  font-family: var(--font-sans);
}
.card-block__preview {
  font-size: 13px;
  color: #6B6B6B;
  margin-top: 4px;
  font-family: var(--font-sans);
}

/* Document List Item */
.doc-item {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 6px 12px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 14px;
  color: #1A1A1A;
  font-family: var(--font-sans);
  transition: background 0.08s;
}
.doc-item:hover { background: #F3F4F6; }
.doc-item--active { background: rgba(0,122,255,0.1); color: #007AFF; }
.doc-item__emoji { font-size: 16px; flex-shrink: 0; }
.doc-item__name { flex: 1; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }

/* Tag Pill */
.tag-pill {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: 100px;
  font-size: 12px;
  font-family: var(--font-sans);
  font-weight: 500;
  background: rgba(255,149,0,0.1);
  color: #D4760A;
}

/* Inline Code */
.inline-code {
  background: #F3F4F6;
  border-radius: 4px;
  padding: 1px 5px;
  font-family: var(--font-mono);
  font-size: 0.9em;
  color: #1A1A1A;
}

/* Toolbar Popup */
.toolbar-popup {
  background: #FFFFFF;
  border: 1px solid #E8E8E8;
  border-radius: 10px;
  padding: 6px;
  display: flex;
  gap: 2px;
  box-shadow: 0 8px 24px rgba(0,0,0,0.12);
}
.toolbar-btn {
  width: 32px; height: 32px;
  border-radius: 6px;
  border: none;
  background: transparent;
  cursor: pointer;
  font-size: 14px;
  color: #1A1A1A;
  transition: background 0.1s;
}
.toolbar-btn:hover { background: #F3F4F6; }
.toolbar-btn--active { background: rgba(0,122,255,0.1); color: #007AFF; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--canvas-max-width` | `700px` | Document content column |
| `--canvas-padding-h` | `40px` | Horizontal canvas padding |
| `--canvas-padding-v` | `60px` | Vertical canvas padding |
| `--sidebar-width` | `260px` | Document navigator |
| `--spacing-xs` | `4px` | Block gaps |
| `--spacing-sm` | `8px` | Sidebar item spacing |
| `--spacing-md` | `16px` | Card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--radius-sm` | `4px` | Inline code |
| `--radius-md` | `6px` | Blocks |
| `--radius-lg` | `10px` | Cards, popups |

## 6. Depth & Elevation
```css
.shadow-toolbar { box-shadow: 0 8px 24px rgba(0,0,0,0.12); }
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.14); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the document canvas at max 700px, centered, with generous padding
- Use emoji as document icons throughout the sidebar
- Blue (#007AFF) is the only accent — selection, links, active items
- Toolbar appears on text selection as a floating popup

**Don't:**
- Don't add heavy UI chrome around the canvas — white space IS the design
- Don't use serif font in the sidebar — only in the document body
- Don't color headings — they should remain dark (#1A1A1A) for a premium feel

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Full-screen canvas; sidebar hidden |
| Tablet | 768px | Narrow sidebar + canvas |
| Desktop | 1024px | Sidebar + canvas |
| Wide | 1440px | Sidebar + canvas + backlinks panel |

## 9. Agent Prompt Guide
```
You are designing for Craft — modern document editor.
Use a white canvas (#FFFFFF) with the document centered at max 700px and 40px horizontal padding.
iOS blue (#007AFF) is the single accent color — links, active sidebar items, text selection.
Document sidebar shows emoji + document name for each item; active item has a soft blue background.
Card blocks are rounded (10px) with a light gray background and subtle border.
The text selection toolbar is a floating popup with rounded buttons and a white background.
Tone is minimal, elegant, writing-first, and Apple-adjacent.
```
