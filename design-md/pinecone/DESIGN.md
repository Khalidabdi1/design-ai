# Pinecone Design System
> Vector database platform for AI with a clean dark developer aesthetic — deep surfaces, vivid teal-green brand accents, and data-pipeline UI patterns.

---

## 1. Visual Theme & Atmosphere
Pinecone lives at the intersection of infrastructure and AI. The design is polished and developer-centric: dark backgrounds, clean typography, and a vivid teal-green accent that feels both modern and technical. The UI prioritizes dashboard clarity — index status, vector counts, and query latency are surfaced prominently. The aesthetic bridges the gap between a traditional developer database tool and a consumer-grade AI product.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00C18A` | Brand teal-green, CTAs |
| `--color-primary-dark` | `#00A075` | Hover/active primary |
| `--color-primary-light` | `#E0FAF3` | Light badges, highlights |
| `--color-bg-base` | `#0D0F1C` | App background |
| `--color-bg-card` | `#161929` | Card surfaces |
| `--color-bg-elevated` | `#1F2337` | Dropdowns, elevated panels |
| `--color-border` | `#2B2F48` | Default borders |
| `--color-border-subtle` | `#1F2337` | Dividers |
| `--color-text-primary` | `#F0F2FF` | Headings, primary text |
| `--color-text-secondary` | `#8E93B5` | Labels, secondary info |
| `--color-text-muted` | `#4D5275` | Placeholders, disabled |
| `--color-success` | `#00C18A` | Index ready, healthy |
| `--color-warning` | `#F5A623` | Initializing, degraded |
| `--color-error` | `#F87171` | Index error, failed |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
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
| Hero / Dashboard Title | 36px | 700 | 1.2 |
| Page Title | 28px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Mono / Code | 13px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #00C18A;
  color: #0D0F1C;
  border: none;
  border-radius: 8px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #00A075; }

/* Index Card */
.index-card {
  background: #161929;
  border: 1px solid #2B2F48;
  border-radius: 10px;
  padding: 20px;
  cursor: pointer;
  transition: border-color 0.15s;
}
.index-card:hover { border-color: #00C18A; }
.index-card__name {
  font-size: 16px;
  font-weight: 600;
  color: #F0F2FF;
  font-family: var(--font-mono);
}
.index-card__stat {
  font-size: 24px;
  font-weight: 700;
  color: #00C18A;
  font-family: var(--font-mono);
  margin-top: 8px;
}
.index-card__stat-label {
  font-size: 12px;
  color: #8E93B5;
}

/* Status Pill */
.status-pill {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 9px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  font-family: var(--font-mono);
}
.status-pill--ready {
  background: rgba(0,193,138,0.12);
  color: #00C18A;
  border: 1px solid rgba(0,193,138,0.2);
}
.status-pill--initializing {
  background: rgba(245,166,35,0.12);
  color: #F5A623;
  border: 1px solid rgba(245,166,35,0.2);
}
.status-pill--error {
  background: rgba(248,113,113,0.12);
  color: #F87171;
  border: 1px solid rgba(248,113,113,0.2);
}

/* Code Panel */
.code-panel {
  background: #0D0F1C;
  border: 1px solid #2B2F48;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #F0F2FF;
  line-height: 1.6;
  overflow-x: auto;
}

/* Input */
.input {
  background: #161929;
  border: 1.5px solid #2B2F48;
  border-radius: 8px;
  padding: 9px 14px;
  font-size: 14px;
  color: #F0F2FF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #00C18A;
  box-shadow: 0 0 0 3px rgba(0,193,138,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight inline gaps |
| `--spacing-sm` | `8px` | Card inner compact spacing |
| `--spacing-md` | `16px` | Component gaps |
| `--spacing-lg` | `20px` | Card padding |
| `--spacing-xl` | `32px` | Section gaps |
| `--spacing-2xl` | `48px` | Page-level gutter |
| `--radius-sm` | `6px` | Badges, chips |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Index cards, panels |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-hover { box-shadow: 0 0 0 1px #00C18A, 0 4px 16px rgba(0,193,138,0.15); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.65); }
```

## 7. Do's and Don'ts
**Do:**
- Show vector count and query latency as the primary index metrics
- Use monospace for all index names, API keys, and dimension counts
- Color-code index status consistently with the status pill pattern
- Highlight the active/hovered index card with a brand-colored border

**Don't:**
- Don't use light colors for primary surfaces — keep it dark and technical
- Don't show vector data as raw arrays — summarize with dimensions/count
- Don't reuse the teal brand color for error or warning states

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Index list view; no dashboard grid |
| Tablet | 768px | 2-column index card grid |
| Desktop | 1024px | Full layout: sidebar + 3-column index grid + detail |
| Wide | 1440px | Expanded grid with additional analytics |

## 9. Agent Prompt Guide
```
You are designing for Pinecone — a vector database for AI applications.
Use a deep dark background (#0D0F1C) with card surfaces at #161929.
Primary accent is teal-green (#00C18A) — use for CTAs, index stats, ready states, and border highlights.
Index cards show the index name in monospace, vector count in large teal numbers.
Status pills use monospace, semantic colors: teal=ready, orange=initializing, red=error.
Code panels are dark with light text, no syntax coloring needed — keep it clean.
Tone is developer-precise, AI-forward, and data-infrastructure-focused.
```
