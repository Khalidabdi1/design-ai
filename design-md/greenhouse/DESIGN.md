# Greenhouse Design System
> Applicant tracking and recruiting platform with a clean, structured aesthetic — white surfaces, green brand anchors, and pipeline-stage-first UI.

---

## 1. Visual Theme & Atmosphere
Greenhouse makes hiring systematic. The UI is clean, process-oriented, and data-rich — built for recruiters who need to track candidates through structured hiring pipelines. The design feels like a professional enterprise product that respects the recruiter's workflow. Green accents reinforce the brand identity and mark active, positive states. The overall aesthetic is airy white with purposeful structure.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#3D9970` | Brand green, CTAs |
| `--color-primary-dark` | `#2D7A57` | Hover/active primary |
| `--color-primary-light` | `#EAF5EF` | Highlights, badges |
| `--color-stage-applied` | `#3D9970` | Applied stage |
| `--color-stage-review` | `#F5A623` | Review/screen stage |
| `--color-stage-interview` | `#4A90D9` | Interview stage |
| `--color-stage-offer` | `#7B68EE` | Offer stage |
| `--color-stage-hired` | `#2ECC71` | Hired |
| `--color-stage-rejected` | `#E74C3C` | Rejected |
| `--color-bg-base` | `#FFFFFF` | Page background |
| `--color-bg-subtle` | `#F7F8FA` | Sidebar, table alternates |
| `--color-text-primary` | `#1A1A2C` | Headings, primary |
| `--color-text-secondary` | `#5A6070` | Body, labels |
| `--color-text-muted` | `#9EA6B4` | Meta, timestamps |
| `--color-border` | `#E0E4EA` | Default borders |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-size-xs: 11px;
--font-size-sm: 13px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 26px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 26px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Candidate Name | 16px | 600 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Meta | 11px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #3D9970;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 9px 18px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #2D7A57; }

/* Candidate Card */
.candidate-card {
  background: #FFFFFF;
  border: 1px solid #E0E4EA;
  border-radius: 8px;
  padding: 16px;
  cursor: pointer;
  transition: box-shadow 0.15s;
}
.candidate-card:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.08); }
.candidate-card__name {
  font-size: 15px;
  font-weight: 600;
  color: #1A1A2C;
}
.candidate-card__role {
  font-size: 13px;
  color: #5A6070;
  margin-top: 2px;
}
.candidate-card__avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: #EAF5EF;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  font-weight: 700;
  color: #3D9970;
  flex-shrink: 0;
}

/* Stage Badge */
.stage-badge {
  display: inline-flex;
  align-items: center;
  padding: 3px 9px;
  border-radius: 100px;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.stage-badge--applied { background: #EAF5EF; color: #3D9970; }
.stage-badge--review { background: #FEF3DC; color: #B8760A; }
.stage-badge--interview { background: #EBF4FD; color: #2773B8; }
.stage-badge--offer { background: #F0EEFF; color: #5B44C2; }
.stage-badge--hired { background: #DAFCE6; color: #1A7F37; }
.stage-badge--rejected { background: #FEE8E8; color: #B91C1C; }

/* Pipeline Stage Column Header */
.stage-column-header {
  padding: 12px 16px;
  background: #F7F8FA;
  border-radius: 6px 6px 0 0;
  border-bottom: 3px solid #3D9970;
  font-size: 13px;
  font-weight: 600;
  color: #5A6070;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* Input */
.input {
  border: 1.5px solid #E0E4EA;
  border-radius: 6px;
  padding: 9px 12px;
  font-size: 14px;
  color: #1A1A2C;
  background: #FFFFFF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #3D9970;
  box-shadow: 0 0 0 3px rgba(61,153,112,0.12);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Badge padding |
| `--spacing-sm` | `8px` | Card meta gap |
| `--spacing-md` | `16px` | Card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `32px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Inline badges |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 1px 4px rgba(0,0,0,0.06); }
.shadow-hover { box-shadow: 0 2px 12px rgba(0,0,0,0.08); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Use distinct stage badge colors for each hiring stage — they need to be scannable at a glance
- Show candidate initials in green avatars when no photo is available
- Always show the count of candidates per pipeline stage in the column header
- Use the pipeline board as the primary recruiting view

**Don't:**
- Don't reuse stage colors across different stages — they're semantic identifiers
- Don't overload candidate cards with more than 4 data points
- Don't use dark backgrounds — this is a light, enterprise product

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Single-column candidate list; no pipeline board |
| Tablet | 768px | Pipeline board with horizontal scroll |
| Desktop | 1024px | Full pipeline board + sidebar |
| Wide | 1440px | Wider pipeline board showing more stages |

## 9. Agent Prompt Guide
```
You are designing for Greenhouse — applicant tracking and recruiting software.
Use a white background with green (#3D9970) as the primary brand and CTA color.
The pipeline board shows hiring stages as columns: Applied → Review → Interview → Offer → Hired.
Each stage has a semantically distinct badge color: green, orange, blue, purple, bright green.
Candidate cards are white with green initial avatars, name, role, and current stage badge.
Inputs use green focus rings. Column headers have a green bottom border.
Tone is structured, process-driven, and professional-enterprise.
```
