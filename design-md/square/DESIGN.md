# Square Design System

> Commerce infrastructure with black-and-white precision and practical business breadth. Square's public site uses a clean sans system, sharp monochrome structure, and modest accent color while balancing payments, hardware, restaurants, retail, appointments, and services in one cohesive platform.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Square feels like **real business operations software presented with premium simplicity**. The system is grounded, modern, and highly utilitarian, but it avoids looking cold or overly enterprise-heavy.

### Mood & Feeling
- Practical and polished
- Business-first and efficient
- Clean and premium
- Broad commerce infrastructure clarity
- Trustworthy without visual excess

### Design Density
**Medium density.** Square covers many industries and capabilities, but uses strong hierarchy and clean modular structure to keep the experience digestible.

### Visual Character
- Black and white base
- Hardware and point-of-sale product imagery
- Practical feature grouping by industry and capability
- Minimal accent color
- Quietly premium operational design

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--square-black` | `#0D0D0D` | Primary text, nav, CTA |
| `--square-white` | `#FFFFFF` | Main surface and cards |
| `--square-surface` | `#F6F6F6` | Soft background |
| `--square-border` | `#E3E3E3` | Dividers and card edges |
| `--square-muted` | `#666666` | Secondary copy |

### Support Colors

| Token | Hex | Role |
|-------|-----|------|
| `--square-green` | `#12805C` | Positive state |
| `--square-blue-soft` | `#EAF2FF` | Optional support tint |
| `--square-warning` | `#A55F14` | Caution state |

---

## 3. Typography Rules

### Font Stack

```css
--font-display: "Square Sans Display", "Helvetica Neue", Arial, sans-serif;
--font-sans: "Square Sans Text", "Helvetica Neue", Arial, sans-serif;
--font-mono: "SF Mono", Menlo, monospace;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 60px | 700 | 1.03 | -0.03em | `#0D0D0D` |
| Page Title | 44px | 700 | 1.08 | -0.02em | `#0D0D0D` |
| Section Title | 32px | 700 | 1.12 | -0.01em | `#0D0D0D` |
| Card Title | 22px | 600 | 1.2 | -0.01em | `#0D0D0D` |
| Body Large | 18px | 400 | 1.6 | 0 | `#0D0D0D` |
| Body | 16px | 400 | 1.6 | 0 | `#0D0D0D` |
| Small Body | 14px | 400 | 1.5 | 0 | `#666666` |
| Label | 12px | 600 | 1.35 | 0.05em | `#666666` |

### Typography Philosophy
Square typography should feel **clear, operational, and premium without fuss**. It should communicate software capability and business trust quickly.

---

## 4. Component Stylings

### Buttons

```css
.button-primary {
  background: #0d0d0d;
  color: #ffffff;
  border: none;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
  font-size: 15px;
  font-weight: 600;
}

.button-primary:hover {
  background: #232323;
}

.button-secondary {
  background: #ffffff;
  color: #0d0d0d;
  border: 1px solid #e3e3e3;
  border-radius: 999px;
  min-height: 44px;
  padding: 0 20px;
}
```

### Cards and Capability Modules

```css
.capability-card {
  background: #ffffff;
  border: 1px solid #e3e3e3;
  border-radius: 20px;
  box-shadow: 0 10px 24px rgba(13, 13, 13, 0.06);
}
```

### Inputs

```css
.input {
  background: #ffffff;
  color: #0d0d0d;
  border: 1px solid #e3e3e3;
  border-radius: 12px;
  min-height: 44px;
  padding: 12px 14px;
}
```

### Component Notes
- Hardware and commerce workflow modules should feel tangible and credible
- Square works best when the product breadth is organized with strong hierarchy
- Color should remain secondary to black-and-white clarity

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `4px` | Tight alignments |
| `--space-3` | `8px` | Small rhythm |
| `--space-4` | `12px` | Compact spacing |
| `--space-5` | `16px` | Default spacing |
| `--space-6` | `24px` | Card spacing |
| `--space-7` | `32px` | Industry/capability separation |
| `--space-8` | `48px` | Section spacing |
| `--space-9` | `64px` | Hero and broad platform sections |

### Layout Behavior
- Organize by business type and capability
- Use clean product rows for hardware and software modules
- Keep page rhythm practical and easy to skim
- Let the commerce platform breadth feel structured rather than sprawling

### Whitespace Philosophy
Whitespace should feel **business-smart and premium**, helping operational complexity feel manageable.

---

## 6. Depth & Elevation

### Elevation Strategy
Square uses **subtle premium utility elevation**. Cards lift gently, but most separation comes from spacing and crisp container edges.

```css
--shadow-soft: 0 8px 18px rgba(13, 13, 13, 0.05);
--shadow-card: 0 14px 30px rgba(13, 13, 13, 0.08);
```

### Surface Hierarchy
- White base
- Soft gray support sections
- Lightly elevated white cards
- Black CTA anchors and occasional status color

---

## 7. Do's and Don'ts

### Do
- Keep the design clean, business-capable, and quietly premium
- Organize industry and capability breadth clearly
- Use black and white as the primary language
- Let hardware and workflow proof carry trust

### Don't
- Do not add unnecessary decorative gradients or startup fluff
- Do not turn Square into heavy enterprise blue-gray software
- Do not clutter the page with weakly grouped product options
- Do not dilute the operational clarity of the platform

---

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Behavior |
|------------|-------|----------|
| Mobile | `< 768px` | Stacked industry modules and simplified capability browsing |
| Tablet | `768px - 1023px` | Two-column product sections and compact hardware rows |
| Desktop | `1024px+` | Broad platform storytelling with clear business-type segmentation |

### Responsive Rules
- Keep industry-specific navigation understandable on mobile
- Preserve legible hardware and product imagery
- Stack dense business modules before shrinking text too aggressively
- Maintain clear CTA hierarchy and readable spacing

---

## 9. Agent Prompt Guide

### Quick Reference
- Black-white commerce infrastructure foundation
- Square Sans-style typography and practical capability cards
- Hardware plus software breadth organized by industry and business outcome
- Premium utility, minimal chrome, operational trust

### Prompt Template
```text
Design this like Square's current public website:
- clean black-and-white commerce-platform foundation
- premium utility typography with simple rounded capability cards
- hardware and software modules organized by business type and outcome
- practical operational clarity with very restrained accent color
- polished real-business infrastructure energy rather than flashy startup styling
```
