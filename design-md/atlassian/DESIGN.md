# Atlassian Design System

> Work coordination software with sharp enterprise clarity and bright blue structure. Atlassian's public site uses `Charlie Display` and `Charlie Text`, with white surfaces, pale blue support backgrounds, deep navy text, and a strong Atlassian blue anchored around `#0052CC`.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Atlassian feels like **serious teamwork software expressed through crisp, modern, enterprise-friendly design**. It is product-rich, confident, and structurally disciplined.

### Mood & Feeling
- Structured and dependable
- Technical but approachable
- Enterprise-ready without heaviness
- Modular and product-driven
- Clear, fast, and pragmatic

### Design Density
**Medium density.** Atlassian surfaces carry lots of product and use-case depth, but the system stays scannable through strong grouping, white space, and blue-led structure.

### Visual Character
- White and pale blue foundation
- Clean product cards and feature grids
- Deep navy text and strong blue accents
- Minimal decorative softness
- Enterprise work tools framed with high clarity

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--atl-blue` | `#0052CC` | Core brand and CTA blue |
| `--atl-blue-bright` | `#2684FF` | Hover and vivid highlight blue |
| `--atl-white` | `#FFFFFF` | Main surface and cards |
| `--atl-surface` | `#F4F5F7` | Light background |
| `--atl-ink` | `#172B4D` | Primary text |

### Support Tokens

| Token | Hex | Role |
|-------|-----|------|
| `--atl-muted` | `#42526E` | Secondary copy |
| `--atl-border` | `#DFE1E6` | Card and divider edges |
| `--atl-blue-soft` | `#DEEBFF` | Soft brand tint |
| `--atl-green` | `#36B37E` | Positive state |
| `--atl-orange` | `#FF8B00` | Attention or highlight accent |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Charlie Display", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Charlie Text", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 700 | 1.05 | -0.02em | `#172B4D` |
| Page Title | 42px | 700 | 1.08 | -0.02em | `#172B4D` |
| Section Title | 32px | 700 | 1.14 | -0.01em | `#172B4D` |
| Card Title | 22px | 600 | 1.22 | -0.01em | `#172B4D` |
| Body Large | 18px | 400 | 1.6 | 0 | `#172B4D` |
| Body | 16px | 400 | 1.6 | 0 | `#172B4D` |
| Small Body | 14px | 400 | 1.5 | 0 | `#42526E` |
| Label | 12px | 700 | 1.35 | 0.04em | `#42526E` |

### Typography Philosophy
Atlassian typography should feel **precise, structured, and product-capable**. It supports engineering, IT, project management, and enterprise browsing without visual fluff.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0052cc;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #2684ff;
}

.button-secondary {
  background: #ffffff;
  color: #172b4d;
  border: 1px solid #dfe1e6;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Product Cards

```css
.product-card {
  background: #ffffff;
  border: 1px solid #dfe1e6;
  border-radius: 20px;
  box-shadow: 0 12px 26px rgba(23, 43, 77, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #172b4d;
  border: 1px solid #dfe1e6;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Cards should feel crisp and systematic
- Blue is the structural brand cue, not a general page wash
- Product depth should always remain easy to browse

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignment |
| `--space-3` | `8px` | Small gaps |
| `--space-4` | `12px` | Compact UI padding |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card rhythm |
| `--space-7` | `32px` | Module separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and ecosystem rows |

### Layout Behavior
- Group products by team, role, and workflow
- Keep feature depth organized into cards and columns
- Use blue tints sparingly to support structure
- Favor clean, enterprise-readable alignment over decorative asymmetry

### Whitespace Philosophy
Whitespace should feel **systematic and efficient**, helping dense platform information stay legible and actionable.

---

## 6. Depth & Elevation

### Elevation Strategy
Atlassian uses **light enterprise elevation** with clear card edges and restrained shadows.

```css
--shadow-soft: 0 8px 18px rgba(23, 43, 77, 0.05);
--shadow-card: 0 16px 30px rgba(23, 43, 77, 0.08);
```

### Surface Hierarchy
- White canvas
- Light blue or gray background bands
- Elevated white product cards
- Strong blue CTA and navigation accents

---

## 7. Do's and Don'ts

### Do
- Keep Atlassian interfaces sharp, structured, and product-clear
- Use blue to orient the experience
- Make complex workflows feel manageable through hierarchy
- Preserve enterprise credibility and technical readability

### Don't
- Do not over-soften the design into consumer-app bubbly UI
- Do not oversaturate large surfaces with blue
- Do not hide platform breadth behind weak organization
- Do not use playful decoration where structure should lead

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked product categories and simplified enterprise navigation |
| Tablet | `768px - 1023px` | Two-column feature sections and compact card grids |
| Desktop | `1024px+` | Full platform ecosystem browsing with broad grouped sections |

### Responsive Rules
- Keep navigation and role-based browsing understandable on mobile
- Preserve card clarity and readable headings at all sizes
- Stack dense platform grids before compressing too far
- Maintain obvious CTA hierarchy across responsive states

---

## 9. Agent Prompt Guide

### Quick Reference
- White and pale-blue enterprise foundation with Atlassian blue
- Charlie-style typography and crisp product cards
- Structured, role-based work-software browsing
- Technical clarity with modern enterprise polish

### Prompt Template
```text
Design this like Atlassian's current public website:
- white and light-blue enterprise foundation
- strong Atlassian-blue CTAs and structural accents
- Charlie-style typography with crisp, systematic product cards
- role-based and workflow-based platform browsing
- modern technical enterprise clarity without cold heaviness
```
