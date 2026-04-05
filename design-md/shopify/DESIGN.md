# Shopify Polaris Design System

## Overview

Shopify Polaris is a comprehensive design system built to create consistent, efficient, and professional merchant experiences across the Shopify admin. The system emphasizes data-rich views, action-driven interfaces, and clean professional aesthetics optimized for e-commerce management workflows.

**Design Philosophy:** Pro design language - efficiency, intuition, and style combined to empower merchants with data-rich views, action-driven interfaces, and dynamic interactions.

---

## 1. Color Palette

### Brand Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| Shopify Green (Primary) | `#008060` | `rgb(0, 128, 96)` | Primary brand color, success states |
| Shopify Green (Secondary) | `#95BF47` | `rgb(149, 191, 71)` | Secondary brand accents |
| Brand Fill | `#303030` | `rgba(48, 48, 48, 1)` | Primary buttons, main actions |
| Brand Fill Hover | `#1A1A1A` | `rgba(26, 26, 26, 1)` | Button hover states |

### Background Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--p-color-bg` | `rgba(241, 241, 241, 1)` | Default admin background |
| `--p-color-bg-inverse` | `rgba(26, 26, 26, 1)` | High contrast backgrounds |
| `--p-color-bg-surface` | `rgba(255, 255, 255, 1)` | Cards, highest prominence surfaces |
| `--p-color-bg-surface-hover` | `rgba(247, 247, 247, 1)` | Surface hover state |
| `--p-color-bg-surface-active` | `rgba(243, 243, 243, 1)` | Surface active/pressed state |
| `--p-color-bg-surface-selected` | `rgba(241, 241, 241, 1)` | Selected surface state |
| `--p-color-bg-surface-secondary` | `rgba(247, 247, 247, 1)` | Secondary prominence surfaces |
| `--p-color-bg-surface-tertiary` | `rgba(243, 243, 243, 1)` | Third level surfaces |

### Semantic Colors

| Category | Token | Value | Usage |
|----------|-------|-------|-------|
| **Success** | `--p-color-bg-fill-success` | `rgba(4, 123, 93, 1)` | Success badges, banners |
| **Success Surface** | `--p-color-bg-surface-success` | `rgba(205, 254, 212, 1)` | Success background areas |
| **Info** | `--p-color-bg-fill-info` | `rgba(145, 208, 255, 1)` | Informational elements |
| **Info Surface** | `--p-color-bg-surface-info` | `rgba(234, 244, 255, 1)` | Info background areas |
| **Warning** | `--p-color-bg-fill-warning` | `rgba(255, 184, 0, 1)` | Warning badges, banners |
| **Warning Surface** | `--p-color-bg-surface-warning` | `rgba(255, 241, 227, 1)` | Warning background areas |
| **Caution** | `--p-color-bg-fill-caution` | `rgba(255, 230, 0, 1)` | Caution states |
| **Caution Surface** | `--p-color-bg-surface-caution` | `rgba(255, 248, 219, 1)` | Caution background areas |
| **Critical** | `--p-color-bg-fill-critical` | `rgba(199, 10, 36, 1)` | Critical/error badges |
| **Critical Surface** | `--p-color-bg-surface-critical` | `rgba(254, 232, 235, 1)` | Error background areas |
| **Emphasis** | `--p-color-bg-fill-emphasis` | `rgba(0, 91, 211, 1)` | Focus areas in editors |
| **Magic (AI)** | `--p-color-bg-fill-magic` | `rgba(128, 81, 255, 1)` | AI-suggested elements |

### Text Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--p-color-text` | `rgba(48, 48, 48, 1)` | Default text color |
| `--p-color-text-secondary` | `rgba(97, 97, 97, 1)` | Secondary text |
| `--p-color-text-disabled` | `rgba(181, 181, 181, 1)` | Disabled text |
| `--p-color-text-link` | `rgba(0, 91, 211, 1)` | Link text |
| `--p-color-text-link-hover` | `rgba(0, 66, 153, 1)` | Link hover state |
| `--p-color-text-brand-on-bg-fill` | `rgba(255, 255, 255, 1)` | Text on primary buttons |
| `--p-color-text-inverse` | `rgba(227, 227, 227, 1)` | Text on inverse backgrounds |
| `--p-color-text-success` | `rgba(1, 75, 64, 1)` | Success text |
| `--p-color-text-critical` | `rgba(142, 11, 33, 1)` | Critical/error text |
| `--p-color-text-warning` | `rgba(94, 66, 0, 1)` | Warning text |
| `--p-color-text-info` | `rgba(0, 58, 90, 1)` | Informational text |
| `--p-color-text-magic` | `rgba(87, 0, 209, 1)` | AI-suggested text |

### Border Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--p-color-border` | `rgba(227, 227, 227, 1)` | Default borders |
| `--p-color-border-hover` | `rgba(204, 204, 204, 1)` | Border hover state |
| `--p-color-border-disabled` | `rgba(235, 235, 235, 1)` | Disabled borders |
| `--p-color-border-secondary` | `rgba(235, 235, 235, 1)` | Dividers, visual separators |
| `--p-color-border-focus` | `rgba(0, 91, 211, 1)` | Focus ring color |
| `--p-color-border-success` | `rgba(146, 252, 172, 1)` | Success borders |
| `--p-color-border-critical` | `rgba(254, 193, 199, 1)` | Critical borders |
| `--p-color-border-critical-secondary` | `rgba(142, 11, 33, 1)` | Invalid input borders |

### Icon Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--p-color-icon` | `rgba(74, 74, 74, 1)` | Default icons |
| `--p-color-icon-hover` | `rgba(48, 48, 48, 1)` | Icon hover state |
| `--p-color-icon-secondary` | `rgba(138, 138, 138, 1)` | Secondary icons |
| `--p-color-icon-disabled` | `rgba(204, 204, 204, 1)` | Disabled icons |
| `--p-color-icon-success` | `rgba(4, 123, 93, 1)` | Success icons |
| `--p-color-icon-critical` | `rgba(226, 44, 56, 1)` | Critical icons |
| `--p-color-icon-warning` | `rgba(178, 132, 0, 1)` | Warning icons |
| `--p-color-icon-info` | `rgba(0, 148, 213, 1)` | Informational icons |

### Input Colors

| Token | Value | Usage |
|-------|-------|-------|
| `--p-color-input-bg-surface` | `rgba(253, 253, 253, 1)` | Input background |
| `--p-color-input-bg-surface-hover` | `rgba(250, 250, 250, 1)` | Input hover background |
| `--p-color-input-bg-surface-active` | `rgba(247, 247, 247, 1)` | Input active background |
| `--p-color-input-border` | `rgba(138, 138, 138, 1)` | Input border |
| `--p-color-input-border-hover` | `rgba(97, 97, 97, 1)` | Input border hover |
| `--p-color-input-border-active` | `rgba(26, 26, 26, 1)` | Input border active |

---

## 2. Typography

### Font Families

```css
/* Primary Sans-Serif */
--p-font-family-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'San Francisco', 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;

/* Monospace */
--p-font-family-mono: ui-monospace, SFMono-Regular, 'SF Mono', Consolas, 'Liberation Mono', Menlo, monospace;
```

### Font Sizes

| Token | Size | Usage |
|-------|------|-------|
| `--p-font-size-275` | 11px | Extra small text, captions |
| `--p-font-size-300` | 12px | Small text, metadata |
| `--p-font-size-325` | 13px | Compact UI text |
| `--p-font-size-350` | 14px | Default body text |
| `--p-font-size-400` | 16px | Standard text |
| `--p-font-size-450` | 18px | Subheadings |
| `--p-font-size-500` | 20px | Section headings |
| `--p-font-size-550` | 22px | Card headings |
| `--p-font-size-600` | 24px | Page titles |
| `--p-font-size-750` | 30px | Large display |
| `--p-font-size-800` | 32px | Hero text |
| `--p-font-size-900` | 36px | Display text |
| `--p-font-size-1000` | 40px | Large display text |

### Font Weights

| Token | Value | Usage |
|-------|-------|-------|
| `--p-font-weight-regular` | 450 | Body text, default |
| `--p-font-weight-medium` | 550 | Emphasized body, labels |
| `--p-font-weight-semibold` | 650 | Headings, buttons |
| `--p-font-weight-bold` | 700 | Strong emphasis |

### Line Heights

| Token | Value | Usage |
|-------|-------|-------|
| `--p-font-line-height-300` | 12px | Extra tight |
| `--p-font-line-height-400` | 16px | Tight, compact UI |
| `--p-font-line-height-500` | 20px | Default body |
| `--p-font-line-height-600` | 24px | Standard text |
| `--p-font-line-height-700` | 28px | Subheadings |
| `--p-font-line-height-800` | 32px | Headings |
| `--p-font-line-height-1000` | 40px | Large headings |
| `--p-font-line-height-1200` | 48px | Display text |

### Letter Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `--p-font-letter-spacing-densest` | -0.54px | Large display text |
| `--p-font-letter-spacing-denser` | -0.3px | Headings |
| `--p-font-letter-spacing-dense` | -0.2px | Subheadings |
| `--p-font-letter-spacing-normal` | 0px | Body text |

### Typography Hierarchy

| Level | Size | Weight | Line Height | Letter Spacing |
|-------|------|--------|-------------|----------------|
| Display XL | 40px | 700 | 48px | -0.54px |
| Display | 36px | 700 | 40px | -0.54px |
| Heading XL | 32px | 650 | 40px | -0.3px |
| Heading L | 24px | 650 | 32px | -0.3px |
| Heading M | 20px | 650 | 28px | -0.2px |
| Heading S | 14px | 650 | 20px | 0px |
| Body L | 16px | 450 | 24px | 0px |
| Body M | 14px | 450 | 20px | 0px |
| Body S | 13px | 450 | 20px | 0px |
| Caption | 12px | 450 | 16px | 0px |

---

## 3. Spacing System

### Base Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--p-space-0` | 0px | No spacing |
| `--p-space-025` | 1px | Minimal spacing |
| `--p-space-050` | 2px | Extra tight |
| `--p-space-100` | 4px | Tight spacing |
| `--p-space-150` | 6px | Compact elements |
| `--p-space-200` | 8px | Default internal spacing |
| `--p-space-300` | 12px | Component spacing |
| `--p-space-400` | 16px | Standard spacing |
| `--p-space-500` | 20px | Medium spacing |
| `--p-space-600` | 24px | Section spacing |
| `--p-space-800` | 32px | Large spacing |
| `--p-space-1000` | 40px | Extra large spacing |
| `--p-space-1200` | 48px | Page section gaps |
| `--p-space-1600` | 64px | Major section spacing |
| `--p-space-2000` | 80px | Large layout spacing |
| `--p-space-2400` | 96px | Extra large layout |
| `--p-space-2800` | 112px | Hero spacing |
| `--p-space-3200` | 128px | Maximum spacing |

### Component-Specific Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `--p-space-button-group-gap` | 8px (var(--p-space-200)) | Gap between buttons |
| `--p-space-card-gap` | 16px (var(--p-space-400)) | Gap within cards |
| `--p-space-card-padding` | 16px (var(--p-space-400)) | Card internal padding |
| `--p-space-table-cell-padding` | 6px (var(--p-space-150)) | Table cell padding |

### Layout Guidelines

- **Card padding:** 16px on all sides
- **Section spacing:** 24-32px between major sections
- **Form field spacing:** 16px between fields
- **Button groups:** 8px gap between buttons
- **List items:** 4-8px vertical spacing
- **Icon-to-text spacing:** 8px

---

## 4. Border & Radius

### Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| `--p-border-radius-0` | 0px | No rounding |
| `--p-border-radius-050` | 2px | Subtle rounding |
| `--p-border-radius-100` | 4px | Buttons, small elements |
| `--p-border-radius-150` | 6px | Inputs, compact elements |
| `--p-border-radius-200` | 8px | Cards, containers |
| `--p-border-radius-300` | 12px | Large cards, modals |
| `--p-border-radius-400` | 16px | Featured sections |
| `--p-border-radius-500` | 20px | Hero elements |
| `--p-border-radius-750` | 30px | Large decorative |
| `--p-border-radius-full` | 9999px | Pills, avatars, circles |

### Border Width

| Token | Value | Usage |
|-------|-------|-------|
| `--p-border-width-0` | 0px | No border |
| `--p-border-width-0165` | 0.66px | Thin hairline borders |
| `--p-border-width-025` | 1px | Default borders |
| `--p-border-width-050` | 2px | Medium emphasis |
| `--p-border-width-100` | 4px | Strong emphasis |

### Common Border Patterns

```css
/* Standard card border */
border: var(--p-border-width-025) solid var(--p-color-border);
border-radius: var(--p-border-radius-200);

/* Input field border */
border: var(--p-border-width-025) solid var(--p-color-input-border);
border-radius: var(--p-border-radius-150);

/* Focus ring */
outline: var(--p-border-width-050) solid var(--p-color-border-focus);
outline-offset: 2px;

/* Button border */
border: none;
border-radius: var(--p-border-radius-100);
```

---

## 5. Shadows & Elevation

### Shadow Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--p-shadow-0` | none | No shadow |
| `--p-shadow-100` | `0px 1px 0px 0px rgba(26, 26, 26, 0.07)` | Subtle lift, cards |
| `--p-shadow-200` | `0px 3px 1px -1px rgba(26, 26, 26, 0.07)` | Raised elements |
| `--p-shadow-300` | `0px 4px 6px -2px rgba(26, 26, 26, 0.20)` | Popovers, dropdowns |
| `--p-shadow-400` | `0px 8px 16px -4px rgba(26, 26, 26, 0.22)` | Modals, overlays |
| `--p-shadow-500` | `0px 12px 20px -8px rgba(26, 26, 26, 0.24)` | Large dialogs |
| `--p-shadow-600` | `0px 20px 20px -8px rgba(26, 26, 26, 0.28)` | Maximum elevation |

### Button Shadows

| Token | Value | Usage |
|-------|-------|-------|
| `--p-shadow-button` | Complex inset shadow | Default button depth |
| `--p-shadow-button-hover` | Complex inset shadow | Button hover state |
| `--p-shadow-button-inset` | Complex inset shadow | Pressed button state |
| `--p-shadow-button-primary` | Complex inset shadow | Primary button depth |
| `--p-shadow-button-primary-hover` | Complex inset shadow | Primary button hover |
| `--p-shadow-button-primary-inset` | `0px 3px 0px 0px rgb(0, 0, 0) inset` | Primary button pressed |

### Inset Shadows

| Token | Value | Usage |
|-------|-------|-------|
| `--p-shadow-inset-100` | Subtle inset shadow | Input fields |
| `--p-shadow-inset-200` | Medium inset shadow | Active inputs |
| `--p-shadow-border-inset` | `0px 0px 0px 1px rgba(0, 0, 0, 0.08) inset` | Border effect |
| `--p-shadow-bevel-100` | Complex bevel shadow | 3D depth effect |

### Elevation Hierarchy

| Level | Shadow | Use Case |
|-------|--------|----------|
| Level 0 | `--p-shadow-0` | Flat content |
| Level 1 | `--p-shadow-100` | Cards at rest |
| Level 2 | `--p-shadow-200` | Hovered cards |
| Level 3 | `--p-shadow-300` | Dropdowns, popovers |
| Level 4 | `--p-shadow-400` | Modals, dialogs |
| Level 5 | `--p-shadow-500` | Large dialogs |
| Level 6 | `--p-shadow-600` | Maximum elevation |

### Z-Index Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--p-z-index-0` | auto | Default stacking |
| `--p-z-index-1` | 100 | Raised elements |
| `--p-z-index-2` | 400 | Dropdown menus |
| `--p-z-index-3` | 510 | Popovers |
| `--p-z-index-4` | 512 | Tooltips |
| `--p-z-index-5` | 513 | Notifications |
| `--p-z-index-6` | 514 | Navigation overlay |
| `--p-z-index-7` | 515 | Modal backdrop |
| `--p-z-index-8` | 516 | Modal content |
| `--p-z-index-9` | 517 | Toast messages |
| `--p-z-index-10` | 518 | Top-level overlays |
| `--p-z-index-11` | 519 | Critical alerts |
| `--p-z-index-12` | 520 | Maximum z-index |

---

## 6. Component Specifications

### Buttons

#### Button Types

| Type | Background | Text | Border | Usage |
|------|------------|------|--------|-------|
| Primary | `--p-color-bg-fill-brand` (#303030) | White | None | Main actions (Save, Create) |
| Secondary | `--p-color-bg-fill` (White) | `--p-color-text` | 1px border | Secondary actions |
| Tertiary | Transparent | `--p-color-text-link` | None | Minimal actions |
| Plain | Transparent | `--p-color-text` | None | Inline actions |
| Destructive | `--p-color-bg-fill-critical` | White | None | Delete, Remove |

#### Button Sizes

| Size | Height | Padding | Font Size |
|------|--------|---------|-----------|
| Slim | 28px | 8px 12px | 13px |
| Medium | 32px | 8px 16px | 14px |
| Large | 40px | 12px 20px | 16px |

#### Button States

```css
/* Primary Button */
.button-primary {
  background: var(--p-color-bg-fill-brand);
  color: var(--p-color-text-brand-on-bg-fill);
  box-shadow: var(--p-shadow-button-primary);
  border-radius: var(--p-border-radius-100);
  padding: 8px 16px;
  font-weight: var(--p-font-weight-medium);
}

.button-primary:hover {
  background: var(--p-color-bg-fill-brand-hover);
  box-shadow: var(--p-shadow-button-primary-hover);
}

.button-primary:active {
  background: var(--p-color-bg-fill-brand-active);
  box-shadow: var(--p-shadow-button-primary-inset);
}

/* Secondary Button */
.button-secondary {
  background: var(--p-color-bg-fill);
  color: var(--p-color-text);
  box-shadow: var(--p-shadow-button);
  border-radius: var(--p-border-radius-100);
}
```

### Cards

```css
.card {
  background: var(--p-color-bg-surface);
  border-radius: var(--p-border-radius-200);
  box-shadow: var(--p-shadow-100);
  padding: var(--p-space-card-padding); /* 16px */
}

.card-header {
  padding-bottom: var(--p-space-400);
  border-bottom: var(--p-border-width-025) solid var(--p-color-border-secondary);
}

.card-section {
  padding: var(--p-space-400) 0;
  border-bottom: var(--p-border-width-025) solid var(--p-color-border-secondary);
}
```

### Form Inputs

#### Text Field

```css
.text-field {
  background: var(--p-color-input-bg-surface);
  border: var(--p-border-width-025) solid var(--p-color-input-border);
  border-radius: var(--p-border-radius-150);
  padding: 8px 12px;
  font-size: var(--p-font-size-350);
  line-height: var(--p-font-line-height-500);
  color: var(--p-color-text);
  min-height: 36px;
}

.text-field:hover {
  border-color: var(--p-color-input-border-hover);
  background: var(--p-color-input-bg-surface-hover);
}

.text-field:focus {
  border-color: var(--p-color-input-border-active);
  outline: var(--p-border-width-050) solid var(--p-color-border-focus);
  outline-offset: 1px;
}

.text-field:disabled {
  background: var(--p-color-bg-surface-disabled);
  border-color: var(--p-color-border-disabled);
  color: var(--p-color-text-disabled);
}

.text-field-error {
  border-color: var(--p-color-border-critical-secondary);
}
```

#### Checkbox

```css
.checkbox {
  width: 18px;
  height: 18px;
  border: var(--p-border-width-025) solid var(--p-color-input-border);
  border-radius: var(--p-border-radius-100);
  background: var(--p-color-input-bg-surface);
}

.checkbox:checked {
  background: var(--p-color-bg-fill-brand);
  border-color: var(--p-color-bg-fill-brand);
}

.checkbox:disabled {
  background: var(--p-color-checkbox-bg-surface-disabled);
}
```

#### Select

```css
.select {
  background: var(--p-color-input-bg-surface);
  border: var(--p-border-width-025) solid var(--p-color-input-border);
  border-radius: var(--p-border-radius-150);
  padding: 8px 32px 8px 12px;
  min-height: 36px;
}
```

### Badges

| Tone | Background | Text |
|------|------------|------|
| Default | `--p-color-bg-fill-secondary` | `--p-color-text` |
| Info | `--p-color-bg-fill-info-secondary` | `--p-color-text-info` |
| Success | `--p-color-bg-fill-success-secondary` | `--p-color-text-success` |
| Warning | `--p-color-bg-fill-warning-secondary` | `--p-color-text-warning` |
| Critical | `--p-color-bg-fill-critical-secondary` | `--p-color-text-critical` |

```css
.badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;
  border-radius: var(--p-border-radius-full);
  font-size: var(--p-font-size-300);
  font-weight: var(--p-font-weight-medium);
}
```

### Data Tables

```css
.data-table {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0;
}

.data-table th {
  padding: var(--p-space-table-cell-padding) var(--p-space-400);
  text-align: left;
  font-weight: var(--p-font-weight-semibold);
  font-size: var(--p-font-size-300);
  color: var(--p-color-text-secondary);
  background: var(--p-color-bg-surface-secondary);
  border-bottom: var(--p-border-width-025) solid var(--p-color-border-secondary);
}

.data-table td {
  padding: var(--p-space-table-cell-padding) var(--p-space-400);
  border-bottom: var(--p-border-width-025) solid var(--p-color-border-secondary);
  font-size: var(--p-font-size-350);
}

.data-table tr:hover td {
  background: var(--p-color-bg-surface-hover);
}

.data-table-numeric {
  font-variant-numeric: tabular-nums;
  text-align: right;
}
```

### Banners

```css
.banner {
  padding: var(--p-space-400);
  border-radius: var(--p-border-radius-200);
  display: flex;
  gap: var(--p-space-300);
  align-items: flex-start;
}

.banner-info {
  background: var(--p-color-bg-surface-info);
  border: var(--p-border-width-025) solid var(--p-color-border-info);
}

.banner-success {
  background: var(--p-color-bg-surface-success);
  border: var(--p-border-width-025) solid var(--p-color-border-success);
}

.banner-warning {
  background: var(--p-color-bg-surface-warning);
  border: var(--p-border-width-025) solid var(--p-color-border-warning);
}

.banner-critical {
  background: var(--p-color-bg-surface-critical);
  border: var(--p-border-width-025) solid var(--p-color-border-critical);
}
```

### Navigation

```css
.nav-item {
  display: flex;
  align-items: center;
  padding: var(--p-space-200) var(--p-space-300);
  border-radius: var(--p-border-radius-150);
  color: var(--p-color-text);
  background: var(--p-color-nav-bg-surface);
}

.nav-item:hover {
  background: var(--p-color-nav-bg-surface-hover);
}

.nav-item-active {
  background: var(--p-color-nav-bg-surface-selected);
  font-weight: var(--p-font-weight-medium);
}
```

---

## 7. Motion & Animation

### Timing Functions

| Token | Value | Usage |
|-------|-------|-------|
| `--p-motion-linear` | `cubic-bezier(0, 0, 1, 1)` | Continuous animations (spinners) |
| `--p-motion-ease-in-out` | `cubic-bezier(0.42, 0, 0.58, 1)` | System transitions |
| `--p-motion-ease-out` | `cubic-bezier(0.19, 0.91, 0.38, 1)` | Exit animations |
| `--p-motion-ease-in` | `cubic-bezier(0.42, 0, 1, 1)` | Enter animations |
| `--p-motion-ease` | `cubic-bezier(0.25, 0.1, 0.25, 1)` | Default user interactions |

### Duration Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--p-motion-duration-0` | 0ms | No animation |
| `--p-motion-duration-50` | 50ms | Instant feedback |
| `--p-motion-duration-100` | 100ms | Micro-interactions |
| `--p-motion-duration-150` | 150ms | Quick transitions |
| `--p-motion-duration-200` | 200ms | Standard transitions |
| `--p-motion-duration-250` | 250ms | Medium transitions |
| `--p-motion-duration-300` | 300ms | Page transitions |
| `--p-motion-duration-350` | 350ms | Complex animations |
| `--p-motion-duration-400` | 400ms | Large element transitions |
| `--p-motion-duration-450` | 450ms | Modal/dialog transitions |
| `--p-motion-duration-500` | 500ms | Maximum standard |
| `--p-motion-duration-5000` | 5000ms | Long animations |

### Animation Keyframes

```css
/* Bounce */
@keyframes bounce {
  from, 65%, 85% { transform: scale(1); }
  75% { transform: scale(0.85); }
  82.5% { transform: scale(1.05); }
}

/* Fade In */
@keyframes fade-in {
  to { opacity: 1; }
}

/* Pulse */
@keyframes pulse {
  from, 75% { transform: scale(0.85); opacity: 1; }
  to { transform: scale(2.5); opacity: 0; }
}

/* Spin */
@keyframes spin {
  to { transform: rotate(1turn); }
}

/* Appear from above */
@keyframes appear-above {
  from { transform: translateY(4px); opacity: 0; }
  to { transform: none; opacity: 1; }
}

/* Appear from below */
@keyframes appear-below {
  from { transform: translateY(-4px); opacity: 0; }
  to { transform: none; opacity: 1; }
}
```

### Common Animation Patterns

```css
/* Button hover */
.button {
  transition: background var(--p-motion-duration-100) var(--p-motion-ease),
              box-shadow var(--p-motion-duration-100) var(--p-motion-ease);
}

/* Card hover lift */
.card-interactive {
  transition: box-shadow var(--p-motion-duration-200) var(--p-motion-ease),
              transform var(--p-motion-duration-200) var(--p-motion-ease);
}

.card-interactive:hover {
  box-shadow: var(--p-shadow-300);
  transform: translateY(-2px);
}

/* Popover appearance */
.popover {
  animation: appear-below var(--p-motion-duration-150) var(--p-motion-ease);
}

/* Spinner */
.spinner {
  animation: spin var(--p-motion-duration-500) var(--p-motion-linear) infinite;
}

/* Skeleton loading pulse */
.skeleton {
  animation: pulse 1.5s ease-in-out infinite;
}
```

---

## 8. Responsive Breakpoints

### Breakpoint Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--p-breakpoints-xs` | 0px | Mobile (extra small) |
| `--p-breakpoints-sm` | 490px | Mobile landscape |
| `--p-breakpoints-md` | 768px | Tablet |
| `--p-breakpoints-lg` | 1040px | Desktop |
| `--p-breakpoints-xl` | 1440px | Large desktop |

### Media Query Variables (Sass)

```scss
// Mobile first (recommended)
$p-breakpoints-xs-up: (min-width: 0em);
$p-breakpoints-sm-up: (min-width: 30.625em);  // 490px
$p-breakpoints-md-up: (min-width: 48em);      // 768px
$p-breakpoints-lg-up: (min-width: 65em);      // 1040px
$p-breakpoints-xl-up: (min-width: 90em);      // 1440px

// Desktop first
$p-breakpoints-xs-down: (max-width: -0.0025em);
$p-breakpoints-sm-down: (max-width: 30.6225em);
$p-breakpoints-md-down: (max-width: 47.9975em);
$p-breakpoints-lg-down: (max-width: 64.9975em);
$p-breakpoints-xl-down: (max-width: 89.9975em);

// Specific breakpoint only
$p-breakpoints-xs-only: (min-width: 0em) and (max-width: 30.6225em);
$p-breakpoints-sm-only: (min-width: 30.625em) and (max-width: 47.9975em);
$p-breakpoints-md-only: (min-width: 48em) and (max-width: 64.9975em);
$p-breakpoints-lg-only: (min-width: 65em) and (max-width: 89.9975em);
$p-breakpoints-xl-only: (min-width: 90em);
```

### Responsive Layout Guidelines

| Breakpoint | Navigation | Cards | Grid Columns |
|------------|------------|-------|--------------|
| xs (0-489px) | Collapsed drawer | Full width | 1 column |
| sm (490-767px) | Collapsed drawer | Full width | 1-2 columns |
| md (768-1039px) | Side nav visible | 2-up layout | 2-3 columns |
| lg (1040-1439px) | Side nav + content | 2-3 columns | 3-4 columns |
| xl (1440px+) | Full layout | Max-width containers | 4+ columns |

### Content Width Guidelines

```css
/* Page container */
.page-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: var(--p-space-400);
}

@media #{$p-breakpoints-md-up} {
  .page-container {
    padding: var(--p-space-600);
  }
}

@media #{$p-breakpoints-lg-up} {
  .page-container {
    padding: var(--p-space-800);
  }
}
```

---

## 9. Accessibility Guidelines

### Color Contrast Requirements

| Element | Minimum Ratio | WCAG Level |
|---------|---------------|------------|
| Body text | 4.5:1 | AA |
| Large text (18px+ bold, 24px+ regular) | 3:1 | AA |
| UI components, icons | 3:1 | AA |
| Focus indicators | 3:1 | AA |

### Polaris Color Contrast Compliance

| Combination | Ratio | Compliant |
|-------------|-------|-----------|
| `--p-color-text` on `--p-color-bg-surface` | 12.6:1 | AAA |
| `--p-color-text-secondary` on `--p-color-bg-surface` | 4.6:1 | AA |
| `--p-color-text-brand-on-bg-fill` on `--p-color-bg-fill-brand` | 12.6:1 | AAA |
| `--p-color-text-critical` on `--p-color-bg-surface-critical` | 7.2:1 | AAA |
| `--p-color-text-success` on `--p-color-bg-surface-success` | 5.8:1 | AA |

### Focus States

```css
/* Standard focus ring */
:focus-visible {
  outline: var(--p-border-width-050) solid var(--p-color-border-focus);
  outline-offset: 2px;
}

/* Focus within for complex components */
.component:focus-within {
  box-shadow: 0 0 0 2px var(--p-color-bg-surface),
              0 0 0 4px var(--p-color-border-focus);
}
```

### Touch Target Sizes

| Element | Minimum Size | Recommended |
|---------|--------------|-------------|
| Buttons | 44px x 44px | 48px x 48px |
| Links (inline) | N/A (natural size) | Adequate padding |
| Checkboxes/Radios | 44px x 44px | 48px x 48px |
| Icon buttons | 44px x 44px | 48px x 48px |

### Interaction State Signifiers

| State | Visual Treatment |
|-------|------------------|
| **Hover** | Background color change, cursor: pointer |
| **Focus** | Blue outline ring (2px, 2px offset) |
| **Active/Pressed** | Darker background, inset shadow |
| **Selected** | Checkmark icon, filled state |
| **Disabled** | Reduced opacity (40%), cursor: not-allowed |
| **Loading** | Spinner icon, reduced opacity |
| **Error** | Red border, error icon, error message |

### Keyboard Navigation

- All interactive elements must be keyboard accessible
- Tab order should follow logical reading order
- Skip links for main content areas
- Escape key closes modals/popovers
- Arrow keys for menu navigation
- Space/Enter to activate buttons
- Use `role` and `aria-*` attributes appropriately

### Screen Reader Guidelines

```html
<!-- Button with loading state -->
<button aria-busy="true" aria-live="polite">
  <span class="visually-hidden">Saving</span>
  <Spinner />
</button>

<!-- Icon button -->
<button aria-label="Delete item">
  <DeleteIcon aria-hidden="true" />
</button>

<!-- Badge with status -->
<span role="status" aria-label="Order status: Fulfilled">
  <Badge tone="success">Fulfilled</Badge>
</span>

<!-- Data table -->
<table role="grid" aria-label="Orders list">
  <thead>
    <tr>
      <th scope="col">Order</th>
      <th scope="col">Date</th>
      <th scope="col">Customer</th>
      <th scope="col" aria-sort="descending">Total</th>
    </tr>
  </thead>
</table>
```

### Motion Preferences

```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

### Icon Guidelines

- Icons should be simple and clearly convey meaning
- Use universally recognized symbols
- Minimum touch target: 44x44px
- Always provide text alternatives for icon-only buttons
- Icons should be 20x20px for standard use, with padding for touch targets

---

## Quick Reference

### CSS Custom Properties Import

```css
@import '@shopify/polaris-tokens/css/styles.css';
```

### Essential Tokens

```css
:root {
  /* Brand */
  --shopify-green: #008060;
  
  /* Backgrounds */
  --bg-page: var(--p-color-bg);
  --bg-card: var(--p-color-bg-surface);
  --bg-button-primary: var(--p-color-bg-fill-brand);
  
  /* Text */
  --text-default: var(--p-color-text);
  --text-secondary: var(--p-color-text-secondary);
  --text-link: var(--p-color-text-link);
  
  /* Typography */
  --font-family: var(--p-font-family-sans);
  --font-size-base: var(--p-font-size-350);
  --font-weight-body: var(--p-font-weight-regular);
  --font-weight-heading: var(--p-font-weight-semibold);
  
  /* Spacing */
  --spacing-tight: var(--p-space-100);
  --spacing-base: var(--p-space-200);
  --spacing-loose: var(--p-space-400);
  
  /* Borders */
  --border-radius-base: var(--p-border-radius-200);
  --border-width: var(--p-border-width-025);
  
  /* Shadows */
  --shadow-card: var(--p-shadow-100);
  --shadow-dropdown: var(--p-shadow-300);
  --shadow-modal: var(--p-shadow-400);
  
  /* Animation */
  --transition-base: var(--p-motion-duration-150) var(--p-motion-ease);
}
```

### Component Size Reference

| Component | Height | Min Width |
|-----------|--------|-----------|
| Button (medium) | 32px | 64px |
| Button (large) | 40px | 80px |
| Text field | 36px | 200px |
| Select | 36px | 120px |
| Checkbox | 18px | 18px |
| Avatar (small) | 24px | 24px |
| Avatar (medium) | 40px | 40px |
| Avatar (large) | 60px | 60px |
| Badge | 20px | auto |
| Icon | 20px | 20px |

---

## Resources

- [Polaris Design System](https://polaris.shopify.com)
- [Polaris React Components](https://polaris.shopify.com/components)
- [Polaris Icons](https://polaris.shopify.com/icons)
- [Polaris Tokens](https://polaris.shopify.com/tokens)
- [Shopify App Design Guidelines](https://shopify.dev/docs/apps/design-guidelines)
- [Polaris GitHub Repository](https://github.com/Shopify/polaris)
