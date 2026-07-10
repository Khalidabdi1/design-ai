# Replicate Design System
> ML model hosting platform with a minimal, technical aesthetic — near-black surfaces, monospace code emphasis, and model-card-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Replicate's design is deliberately understated. The platform steps out of the way of the models it hosts, using a near-black background and minimal color to let model outputs — images, audio, text — become the visual centerpiece. The aesthetic is hacker-minimal: monospace code, subtle borders, and a single bright accent for interactive states. It reads like a well-designed terminal interface for the AI age.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#4F46E5` | Brand indigo, active elements |
| `--color-primary-hover` | `#4338CA` | Hover states |
| `--color-primary-light` | `#EEF2FF` | Light-mode badges |
| `--color-success` | `#10B981` | Run succeeded, model active |
| `--color-warning` | `#F59E0B` | Queued, warming up |
| `--color-error` | `#EF4444` | Run failed |
| `--color-bg-base` | `#111111` | Page background |
| `--color-bg-card` | `#1C1C1C` | Card, model panel surfaces |
| `--color-bg-input` | `#242424` | Input backgrounds |
| `--color-border` | `#333333` | Default borders |
| `--color-border-subtle` | `#2A2A2A` | Subtle separators |
| `--color-text-primary` | `#F5F5F5` | Headings, primary text |
| `--color-text-secondary` | `#A3A3A3` | Labels, meta |
| `--color-text-muted` | `#666666` | Placeholders, disabled |
| `--color-code` | `#7DD3FC` | Code token color, API keys |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', 'IBM Plex Mono', monospace;
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
| Page Title | 28px | 700 | 1.2 |
| Section Header | 20px | 600 | 1.3 |
| Model Name | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Meta / Label | 13px | 400 | 1.4 |
| Code / Mono | 13px | 400 | 1.6 |
| Caption | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #4F46E5;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #4338CA; }

/* Run Button (special: full-width, prominent) */
.button-run {
  background: #4F46E5;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 12px 24px;
  font-size: 15px;
  font-weight: 700;
  width: 100%;
  cursor: pointer;
}
.button-run:hover { background: #4338CA; }

/* Model Card */
.model-card {
  background: #1C1C1C;
  border: 1px solid #333333;
  border-radius: 8px;
  padding: 16px;
  cursor: pointer;
  transition: border-color 0.15s ease;
}
.model-card:hover { border-color: #4F46E5; }
.model-card__name {
  font-size: 14px;
  font-weight: 600;
  color: #F5F5F5;
}
.model-card__author {
  font-size: 12px;
  color: #A3A3A3;
  margin-top: 2px;
}

/* Code Block */
.code-block {
  background: #111111;
  border: 1px solid #333333;
  border-radius: 6px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #F5F5F5;
  overflow-x: auto;
  line-height: 1.6;
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 9px;
  border-radius: 4px;
  font-size: 11px;
  font-weight: 600;
  font-family: var(--font-mono);
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.status-badge--running { background: rgba(79,70,229,0.15); color: #818CF8; }
.status-badge--succeeded { background: rgba(16,185,129,0.12); color: #34D399; }
.status-badge--failed { background: rgba(239,68,68,0.12); color: #F87171; }

/* Input */
.input {
  background: #242424;
  border: 1px solid #333333;
  border-radius: 6px;
  padding: 9px 12px;
  font-size: 14px;
  font-family: var(--font-sans);
  color: #F5F5F5;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #4F46E5;
  box-shadow: 0 0 0 2px rgba(79,70,229,0.25);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon padding |
| `--spacing-sm` | `8px` | Compact gaps |
| `--spacing-md` | `16px` | Card inner padding |
| `--spacing-lg` | `24px` | Section spacing |
| `--spacing-xl` | `40px` | Page gutter |
| `--radius-sm` | `4px` | Status badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards, panels |
| `--sidebar-width` | `280px` | Model parameter sidebar |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-hover { box-shadow: 0 4px 16px rgba(0,0,0,0.6); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
```

## 7. Do's and Don'ts
**Do:**
- Make model output the hero — use a large output preview area
- Use monospace for all API code, run IDs, version hashes, and tokens
- Status badges should always be uppercase monospace with semantic colors
- Keep parameter inputs compact and stacked in a sidebar

**Don't:**
- Don't use bright backgrounds — they compete with model output visuals
- Don't decorate code blocks with heavy chrome; the code is the content
- Don't use animation on run outputs — it distracts from model results

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Inputs tab + output tab; no sidebar |
| Tablet | 768px | Stacked: inputs top, output below |
| Desktop | 1024px | Two-column: parameters sidebar + output area |
| Wide | 1440px | Parameters sidebar fixed, output area expands |

## 9. Agent Prompt Guide
```
You are designing for Replicate — an ML model hosting and inference platform.
Use near-black backgrounds (#111111 page, #1C1C1C cards) with #F5F5F5 text.
Primary brand color is indigo (#4F46E5); use for CTAs, active states, and focus rings.
Monospace font (JetBrains Mono) is essential: code blocks, status badges, run IDs, API tokens.
Status badges are uppercase, small, monospace, with semantic background fills.
Model cards have dark backgrounds with subtle borders that glow indigo on hover.
Tone is hacker-minimal, technical, and output-focused.
```
