# Hex Design System
> Collaborative data notebook and analytics platform with a clean modern aesthetic — white surfaces, vivid amber accents, and notebook-cell-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Hex reimagines the data notebook for modern teams. The interface combines the structured familiarity of a notebook with the collaboration features of a modern SaaS app. Light, clean surfaces prioritize readability of code and outputs; amber-gold accents mark active cells, interactive elements, and the brand itself. The aesthetic is modern and approachable — the kind of analytics tool a designer would actually enjoy using.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#F59E0B` | Brand amber, CTAs, active cells |
| `--color-primary-dark` | `#D97706` | Hover/active primary |
| `--color-primary-light` | `#FFFBEB` | Light cell highlights |
| `--color-secondary` | `#6366F1` | Secondary accent, charts |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F9FAFB` | Notebook outer shell |
| `--color-bg-cell` | `#FFFFFF` | Cell background |
| `--color-bg-code` | `#F8F9FA` | Code cell background |
| `--color-border` | `#E5E7EB` | Default borders |
| `--color-border-cell-active` | `#F59E0B` | Active cell left border |
| `--color-text-primary` | `#111827` | Headings, primary text |
| `--color-text-secondary` | `#4B5563` | Body, labels |
| `--color-text-muted` | `#9CA3AF` | Placeholders, meta |
| `--color-success` | `#10B981` | Cell run success |
| `--color-error` | `#EF4444` | Cell run error |
| `--color-code-keyword` | `#8B5CF6` | Code syntax: keyword |
| `--color-code-string` | `#10B981` | Code syntax: string |
| `--color-code-comment` | `#9CA3AF` | Code syntax: comment |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 15px;
--font-size-lg: 18px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.6;
--line-height-code: 1.7;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Notebook Title | 24px | 700 | 1.25 |
| Section Header | 18px | 600 | 1.3 |
| Cell Output Title | 14px | 600 | 1.4 |
| Body / Markdown | 15px | 400 | 1.6 |
| Code | 13px | 400 | 1.7 |
| Label | 13px | 500 | 1.4 |
| Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #F59E0B;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.12s;
}
.button-primary:hover { background: #D97706; }

/* Notebook Cell */
.cell {
  border: 1px solid #E5E7EB;
  border-left: 3px solid transparent;
  border-radius: 0 6px 6px 0;
  margin-bottom: 8px;
  position: relative;
  transition: border-left-color 0.1s;
}
.cell--active { border-left-color: #F59E0B; }
.cell--running { border-left-color: #6366F1; }
.cell--error { border-left-color: #EF4444; }

/* Code Cell */
.code-cell {
  background: #F8F9FA;
  border-radius: 0 6px 6px 0;
  padding: 12px 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  line-height: 1.7;
  color: #111827;
  min-height: 48px;
}

/* Cell Output */
.cell-output {
  border-top: 1px solid #E5E7EB;
  padding: 12px 16px;
  background: #FFFFFF;
}
.cell-output--error {
  background: rgba(239,68,68,0.04);
  border-top-color: #FCA5A5;
  color: #EF4444;
  font-family: var(--font-mono);
  font-size: 12px;
}

/* Run Button (cell gutter) */
.run-button {
  width: 24px;
  height: 24px;
  border-radius: 4px;
  border: none;
  background: transparent;
  color: #9CA3AF;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: background 0.1s, color 0.1s;
}
.run-button:hover {
  background: #FEF3C7;
  color: #F59E0B;
}

/* Input */
.input {
  border: 1.5px solid #E5E7EB;
  border-radius: 6px;
  padding: 8px 12px;
  font-size: 14px;
  color: #111827;
  background: #FFFFFF;
  transition: border-color 0.12s;
}
.input:focus {
  outline: none;
  border-color: #F59E0B;
  box-shadow: 0 0 0 3px rgba(245,158,11,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Gutter padding |
| `--spacing-sm` | `8px` | Cell gap |
| `--spacing-md` | `12px` | Cell inner padding |
| `--spacing-lg` | `16px` | Section separation |
| `--spacing-xl` | `24px` | Notebook padding |
| `--notebook-max-width` | `860px` | Center column max |
| `--sidebar-width` | `240px` | Table of contents |
| `--cell-gutter` | `48px` | Left gutter for run button + line numbers |
| `--radius-sm` | `4px` | Run button |
| `--radius-md` | `6px` | Cells, inputs |

## 6. Depth & Elevation
```css
.shadow-cell { box-shadow: 0 1px 3px rgba(0,0,0,0.04); }
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Highlight the active cell with an amber left border — it's the key spatial indicator
- Code cells use a slightly off-white (#F8F9FA) background to distinguish from output
- Run buttons in the gutter are icon-only, revealed on hover
- Table of contents in the sidebar auto-generates from markdown headers

**Don't:**
- Don't use full-width cells — the 860px max-width makes the notebook scannable
- Don't add heavy decorative borders around cells — 1px subtle is enough
- Don't truncate code output — let it scroll within the cell

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Read-only view; code cells scroll horizontally |
| Tablet | 768px | Sidebar collapses; cells at full width |
| Desktop | 1024px | Sidebar + centered notebook column |
| Wide | 1440px | Wider with more side margin and larger charts |

## 9. Agent Prompt Guide
```
You are designing for Hex — a collaborative data notebook.
Use a white background with cells displayed in a centered column (max 860px).
The active cell has a 3px amber (#F59E0B) left border as its primary focus indicator.
Code cells have a slightly off-white (#F8F9FA) background; output cells are pure white.
Run buttons live in a left gutter, icon-only, revealed on hover with amber background.
Typography: Inter for UI and markdown, JetBrains Mono for code at 13px line-height 1.7.
Tone is clean, analytical, and collaboration-forward.
```
