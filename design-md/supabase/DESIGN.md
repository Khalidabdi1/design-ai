# Supabase Design System

## 1. Brand Overview

### Brand Identity
Supabase is the open-source Firebase alternative, providing a suite of backend tools built around PostgreSQL. The brand embodies developer empowerment, open-source philosophy, and technical sophistication while maintaining approachability.

### Core Brand Values
- **Open Source First**: Transparency and community-driven development
- **Developer Experience**: Code-first approach with minimal friction
- **PostgreSQL Power**: Enterprise-grade database at the core
- **Simplicity**: Complex infrastructure made accessible
- **Speed**: Rapid development and deployment

### Brand Personality
- Technical yet approachable
- Professional with subtle playfulness
- Confident but not arrogant
- Community-focused and inclusive
- Forward-thinking and innovative

### Target Audience
- Full-stack developers
- Backend engineers
- Startup founders and indie hackers
- Enterprise development teams
- Open-source enthusiasts

---

## 2. Color Palette

### Primary Colors

#### Supabase Green (Brand Primary)
```css
--brand-green: #3ECF8E;
--brand-green-light: #4FF8A8;
--brand-green-dark: #24B47E;
--brand-green-darker: #1A8F63;
```

**Usage**: Primary CTAs, brand accents, success states, interactive highlights, logo treatments

#### Dark Backgrounds
```css
--background-dark: #1C1C1C;
--background-darker: #111111;
--background-darkest: #0A0A0A;
--surface-dark: #1F1F1F;
--surface-elevated: #252525;
--surface-overlay: #2A2A2A;
```

**Usage**: Page backgrounds, cards, modals, sidebars, code blocks

### Secondary Colors

#### Gray Scale
```css
--gray-100: #F8F9FA;
--gray-200: #E9ECEF;
--gray-300: #DEE2E6;
--gray-400: #CED4DA;
--gray-500: #8B8B8B;
--gray-600: #6B6B6B;
--gray-700: #4B4B4B;
--gray-800: #3B3B3B;
--gray-900: #2B2B2B;
```

#### Accent Colors
```css
--purple: #9B59B6;
--blue: #3B82F6;
--cyan: #22D3EE;
--orange: #F97316;
--yellow: #FACC15;
--pink: #EC4899;
```

### Functional Colors

#### Status & Feedback
```css
--success: #3ECF8E;
--success-light: rgba(62, 207, 142, 0.15);
--warning: #F5A623;
--warning-light: rgba(245, 166, 35, 0.15);
--error: #EF4444;
--error-light: rgba(239, 68, 68, 0.15);
--info: #3B82F6;
--info-light: rgba(59, 130, 246, 0.15);
```

### Text Colors
```css
--text-primary: #FFFFFF;
--text-secondary: #B3B3B3;
--text-tertiary: #808080;
--text-muted: #666666;
--text-disabled: #4D4D4D;
--text-inverse: #111111;
```

### Border Colors
```css
--border-default: #2E2E2E;
--border-light: #3A3A3A;
--border-focus: #3ECF8E;
--border-error: #EF4444;
```

### Gradient Definitions
```css
--gradient-brand: linear-gradient(135deg, #3ECF8E 0%, #24B47E 100%);
--gradient-dark: linear-gradient(180deg, #1C1C1C 0%, #111111 100%);
--gradient-glow: radial-gradient(ellipse at center, rgba(62, 207, 142, 0.15) 0%, transparent 70%);
--gradient-hero: linear-gradient(to bottom, #111111 0%, #1C1C1C 50%, #111111 100%);
```

---

## 3. Typography

### Font Families

#### Primary Font Stack
```css
--font-sans: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
```

#### Monospace Font (Code)
```css
--font-mono: 'Source Code Pro', 'SF Mono', 'Monaco', 'Inconsolata', 'Fira Code', 'Droid Sans Mono', 'Consolas', monospace;
```

### Type Scale

#### Display
```css
.display-xl {
  font-size: 72px;
  line-height: 1.1;
  font-weight: 700;
  letter-spacing: -0.03em;
}

.display-lg {
  font-size: 56px;
  line-height: 1.15;
  font-weight: 700;
  letter-spacing: -0.02em;
}

.display-md {
  font-size: 44px;
  line-height: 1.2;
  font-weight: 700;
  letter-spacing: -0.02em;
}
```

#### Headings
```css
.heading-h1 {
  font-size: 36px;
  line-height: 1.25;
  font-weight: 600;
  letter-spacing: -0.01em;
}

.heading-h2 {
  font-size: 28px;
  line-height: 1.3;
  font-weight: 600;
  letter-spacing: -0.01em;
}

.heading-h3 {
  font-size: 22px;
  line-height: 1.35;
  font-weight: 600;
}

.heading-h4 {
  font-size: 18px;
  line-height: 1.4;
  font-weight: 600;
}

.heading-h5 {
  font-size: 16px;
  line-height: 1.45;
  font-weight: 600;
}

.heading-h6 {
  font-size: 14px;
  line-height: 1.5;
  font-weight: 600;
}
```

#### Body Text
```css
.body-lg {
  font-size: 18px;
  line-height: 1.7;
  font-weight: 400;
}

.body-md {
  font-size: 16px;
  line-height: 1.65;
  font-weight: 400;
}

.body-sm {
  font-size: 14px;
  line-height: 1.6;
  font-weight: 400;
}

.body-xs {
  font-size: 12px;
  line-height: 1.5;
  font-weight: 400;
}
```

#### Code Typography
```css
.code-block {
  font-family: var(--font-mono);
  font-size: 14px;
  line-height: 1.7;
  font-weight: 400;
}

.code-inline {
  font-family: var(--font-mono);
  font-size: 0.9em;
  font-weight: 500;
  background: rgba(62, 207, 142, 0.1);
  padding: 2px 6px;
  border-radius: 4px;
}

.code-terminal {
  font-family: var(--font-mono);
  font-size: 13px;
  line-height: 1.6;
}
```

#### Utility Text
```css
.caption {
  font-size: 12px;
  line-height: 1.4;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.label {
  font-size: 14px;
  line-height: 1.4;
  font-weight: 500;
}

.overline {
  font-size: 11px;
  line-height: 1.3;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}
```

---

## 4. Spacing System

### Base Unit
```css
--space-unit: 4px;
```

### Spacing Scale
```css
--space-0: 0;
--space-1: 4px;    /* 0.25rem */
--space-2: 8px;    /* 0.5rem */
--space-3: 12px;   /* 0.75rem */
--space-4: 16px;   /* 1rem */
--space-5: 20px;   /* 1.25rem */
--space-6: 24px;   /* 1.5rem */
--space-8: 32px;   /* 2rem */
--space-10: 40px;  /* 2.5rem */
--space-12: 48px;  /* 3rem */
--space-16: 64px;  /* 4rem */
--space-20: 80px;  /* 5rem */
--space-24: 96px;  /* 6rem */
--space-32: 128px; /* 8rem */
```

### Component Spacing

#### Padding Standards
```css
/* Buttons */
--button-padding-sm: 8px 12px;
--button-padding-md: 10px 16px;
--button-padding-lg: 14px 24px;

/* Cards */
--card-padding-sm: 16px;
--card-padding-md: 24px;
--card-padding-lg: 32px;

/* Inputs */
--input-padding-sm: 8px 10px;
--input-padding-md: 10px 14px;
--input-padding-lg: 14px 18px;

/* Modals */
--modal-padding: 24px;
--modal-header-padding: 20px 24px;
--modal-footer-padding: 16px 24px;
```

#### Gap Standards
```css
--gap-inline-sm: 8px;
--gap-inline-md: 12px;
--gap-inline-lg: 16px;
--gap-stack-sm: 12px;
--gap-stack-md: 16px;
--gap-stack-lg: 24px;
```

### Layout Spacing
```css
/* Section spacing */
--section-padding-sm: 48px 0;
--section-padding-md: 80px 0;
--section-padding-lg: 120px 0;

/* Container */
--container-padding: 24px;
--container-max-width: 1280px;

/* Dashboard */
--sidebar-width: 256px;
--header-height: 56px;
--panel-gap: 16px;
```

---

## 5. Component Library

### Buttons

#### Primary Button
```css
.button-primary {
  background: var(--brand-green);
  color: #111111;
  padding: var(--button-padding-md);
  border-radius: 6px;
  font-weight: 500;
  font-size: 14px;
  border: none;
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-primary:hover {
  background: var(--brand-green-light);
  transform: translateY(-1px);
  box-shadow: 0 4px 12px rgba(62, 207, 142, 0.3);
}

.button-primary:active {
  transform: translateY(0);
}

.button-primary:disabled {
  opacity: 0.5;
  cursor: not-allowed;
  transform: none;
}
```

#### Secondary Button
```css
.button-secondary {
  background: transparent;
  color: var(--text-primary);
  padding: var(--button-padding-md);
  border-radius: 6px;
  font-weight: 500;
  font-size: 14px;
  border: 1px solid var(--border-light);
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-secondary:hover {
  background: var(--surface-elevated);
  border-color: var(--gray-500);
}
```

#### Ghost Button
```css
.button-ghost {
  background: transparent;
  color: var(--text-secondary);
  padding: var(--button-padding-md);
  border-radius: 6px;
  font-weight: 500;
  font-size: 14px;
  border: none;
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-ghost:hover {
  color: var(--text-primary);
  background: var(--surface-dark);
}
```

#### Danger Button
```css
.button-danger {
  background: var(--error);
  color: white;
  padding: var(--button-padding-md);
  border-radius: 6px;
  font-weight: 500;
  font-size: 14px;
  border: none;
  cursor: pointer;
  transition: all 0.2s ease;
}

.button-danger:hover {
  background: #DC2626;
}
```

### Form Elements

#### Input Field
```css
.input {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 6px;
  padding: var(--input-padding-md);
  font-size: 14px;
  color: var(--text-primary);
  width: 100%;
  transition: all 0.2s ease;
}

.input::placeholder {
  color: var(--text-muted);
}

.input:hover {
  border-color: var(--border-light);
}

.input:focus {
  outline: none;
  border-color: var(--brand-green);
  box-shadow: 0 0 0 3px rgba(62, 207, 142, 0.15);
}

.input:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

.input-error {
  border-color: var(--error);
}

.input-error:focus {
  box-shadow: 0 0 0 3px var(--error-light);
}
```

#### Select Dropdown
```css
.select {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 6px;
  padding: var(--input-padding-md);
  font-size: 14px;
  color: var(--text-primary);
  cursor: pointer;
  appearance: none;
  background-image: url("data:image/svg+xml,..."); /* Chevron icon */
  background-repeat: no-repeat;
  background-position: right 12px center;
}
```

#### Checkbox
```css
.checkbox {
  width: 18px;
  height: 18px;
  border: 2px solid var(--border-light);
  border-radius: 4px;
  background: var(--surface-dark);
  cursor: pointer;
  transition: all 0.15s ease;
}

.checkbox:checked {
  background: var(--brand-green);
  border-color: var(--brand-green);
}
```

#### Toggle Switch
```css
.toggle {
  width: 44px;
  height: 24px;
  background: var(--gray-700);
  border-radius: 12px;
  position: relative;
  cursor: pointer;
  transition: background 0.2s ease;
}

.toggle::after {
  content: '';
  width: 18px;
  height: 18px;
  background: white;
  border-radius: 50%;
  position: absolute;
  top: 3px;
  left: 3px;
  transition: transform 0.2s ease;
}

.toggle.active {
  background: var(--brand-green);
}

.toggle.active::after {
  transform: translateX(20px);
}
```

### Cards

#### Standard Card
```css
.card {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 8px;
  padding: var(--card-padding-md);
  transition: all 0.2s ease;
}

.card:hover {
  border-color: var(--border-light);
}
```

#### Feature Card
```css
.card-feature {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 12px;
  padding: var(--card-padding-lg);
  position: relative;
  overflow: hidden;
}

.card-feature::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--gradient-brand);
}
```

#### Pricing Card
```css
.card-pricing {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 12px;
  padding: 32px;
  text-align: center;
}

.card-pricing.featured {
  border-color: var(--brand-green);
  background: linear-gradient(
    180deg,
    rgba(62, 207, 142, 0.08) 0%,
    var(--surface-dark) 100%
  );
}
```

### Navigation

#### Sidebar
```css
.sidebar {
  width: var(--sidebar-width);
  background: var(--background-darker);
  border-right: 1px solid var(--border-default);
  height: 100vh;
  position: fixed;
  left: 0;
  top: 0;
  padding: 16px 0;
  overflow-y: auto;
}

.sidebar-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 16px;
  color: var(--text-secondary);
  font-size: 14px;
  cursor: pointer;
  transition: all 0.15s ease;
  border-radius: 6px;
  margin: 2px 8px;
}

.sidebar-item:hover {
  background: var(--surface-dark);
  color: var(--text-primary);
}

.sidebar-item.active {
  background: rgba(62, 207, 142, 0.1);
  color: var(--brand-green);
}
```

#### Top Navigation
```css
.topnav {
  height: var(--header-height);
  background: var(--background-darker);
  border-bottom: 1px solid var(--border-default);
  display: flex;
  align-items: center;
  padding: 0 24px;
  position: sticky;
  top: 0;
  z-index: 100;
}
```

### Tables (Database Style)

#### Data Table
```css
.table {
  width: 100%;
  border-collapse: collapse;
  font-size: 14px;
}

.table th {
  text-align: left;
  padding: 12px 16px;
  background: var(--surface-dark);
  border-bottom: 1px solid var(--border-default);
  font-weight: 500;
  color: var(--text-secondary);
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.table td {
  padding: 12px 16px;
  border-bottom: 1px solid var(--border-default);
  color: var(--text-primary);
  font-family: var(--font-mono);
  font-size: 13px;
}

.table tr:hover td {
  background: var(--surface-dark);
}

.table-row-selected td {
  background: rgba(62, 207, 142, 0.1);
}
```

#### Column Header
```css
.column-header {
  display: flex;
  align-items: center;
  gap: 8px;
  cursor: pointer;
}

.column-type {
  color: var(--brand-green);
  font-family: var(--font-mono);
  font-size: 11px;
  padding: 2px 6px;
  background: rgba(62, 207, 142, 0.1);
  border-radius: 4px;
}
```

### Code Blocks

#### Code Editor Style
```css
.code-block {
  background: var(--background-darkest);
  border: 1px solid var(--border-default);
  border-radius: 8px;
  overflow: hidden;
}

.code-block-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 12px 16px;
  background: var(--surface-dark);
  border-bottom: 1px solid var(--border-default);
}

.code-block-content {
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 14px;
  line-height: 1.7;
  overflow-x: auto;
}

.code-block-content pre {
  margin: 0;
}
```

#### Syntax Highlighting
```css
.syntax-keyword { color: #C678DD; }
.syntax-string { color: #98C379; }
.syntax-number { color: #D19A66; }
.syntax-comment { color: #5C6370; font-style: italic; }
.syntax-function { color: #61AFEF; }
.syntax-variable { color: #E5C07B; }
.syntax-property { color: #E06C75; }
.syntax-operator { color: #56B6C2; }
```

#### Terminal Block
```css
.terminal {
  background: var(--background-darkest);
  border: 1px solid var(--border-default);
  border-radius: 8px;
  font-family: var(--font-mono);
  font-size: 13px;
  line-height: 1.6;
}

.terminal-header {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 12px 16px;
  background: var(--surface-dark);
  border-bottom: 1px solid var(--border-default);
}

.terminal-dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
}

.terminal-dot.red { background: #FF5F56; }
.terminal-dot.yellow { background: #FFBD2E; }
.terminal-dot.green { background: #27C93F; }

.terminal-content {
  padding: 16px;
}

.terminal-prompt {
  color: var(--brand-green);
}

.terminal-command {
  color: var(--text-primary);
}

.terminal-output {
  color: var(--text-secondary);
}
```

### Modals

#### Standard Modal
```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.8);
  backdrop-filter: blur(4px);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}

.modal {
  background: var(--surface-dark);
  border: 1px solid var(--border-default);
  border-radius: 12px;
  width: 100%;
  max-width: 500px;
  max-height: 85vh;
  overflow: hidden;
}

.modal-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: var(--modal-header-padding);
  border-bottom: 1px solid var(--border-default);
}

.modal-body {
  padding: var(--modal-padding);
  overflow-y: auto;
}

.modal-footer {
  display: flex;
  justify-content: flex-end;
  gap: 12px;
  padding: var(--modal-footer-padding);
  border-top: 1px solid var(--border-default);
  background: var(--background-darker);
}
```

### Badges & Tags

#### Status Badge
```css
.badge {
  display: inline-flex;
  align-items: center;
  padding: 4px 10px;
  border-radius: 9999px;
  font-size: 12px;
  font-weight: 500;
}

.badge-success {
  background: var(--success-light);
  color: var(--success);
}

.badge-warning {
  background: var(--warning-light);
  color: var(--warning);
}

.badge-error {
  background: var(--error-light);
  color: var(--error);
}

.badge-info {
  background: var(--info-light);
  color: var(--info);
}
```

#### Tag
```css
.tag {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 8px;
  background: var(--surface-elevated);
  border: 1px solid var(--border-default);
  border-radius: 4px;
  font-size: 12px;
  color: var(--text-secondary);
}

.tag-primary {
  background: rgba(62, 207, 142, 0.1);
  border-color: rgba(62, 207, 142, 0.2);
  color: var(--brand-green);
}
```

### Tooltips
```css
.tooltip {
  position: relative;
}

.tooltip-content {
  position: absolute;
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%);
  margin-bottom: 8px;
  padding: 8px 12px;
  background: var(--surface-overlay);
  border: 1px solid var(--border-default);
  border-radius: 6px;
  font-size: 12px;
  color: var(--text-primary);
  white-space: nowrap;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
  z-index: 50;
}

.tooltip-content::after {
  content: '';
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  border: 6px solid transparent;
  border-top-color: var(--surface-overlay);
}
```

### Alerts
```css
.alert {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 16px;
  border-radius: 8px;
  font-size: 14px;
}

.alert-success {
  background: var(--success-light);
  border: 1px solid rgba(62, 207, 142, 0.2);
  color: var(--text-primary);
}

.alert-warning {
  background: var(--warning-light);
  border: 1px solid rgba(245, 166, 35, 0.2);
  color: var(--text-primary);
}

.alert-error {
  background: var(--error-light);
  border: 1px solid rgba(239, 68, 68, 0.2);
  color: var(--text-primary);
}

.alert-info {
  background: var(--info-light);
  border: 1px solid rgba(59, 130, 246, 0.2);
  color: var(--text-primary);
}
```

---

## 6. Iconography

### Icon System
Supabase uses a custom icon set alongside Feather Icons, maintaining a consistent stroke weight and sizing system.

### Icon Specifications
```css
--icon-size-xs: 14px;
--icon-size-sm: 16px;
--icon-size-md: 20px;
--icon-size-lg: 24px;
--icon-size-xl: 32px;

--icon-stroke-width: 1.5px;
--icon-color-default: var(--text-secondary);
--icon-color-active: var(--text-primary);
--icon-color-brand: var(--brand-green);
```

### Product Icons
```
Database      - Cylindrical database icon
Auth          - Shield with check
Storage       - Folder/bucket icon
Functions     - Lightning bolt / function symbol
Realtime      - Radio waves / broadcast
Edge          - Globe with network nodes
SQL Editor    - Code brackets with table
API           - Connected nodes
```

### UI Icons
```
Navigation    - Hamburger, arrows, chevrons
Actions       - Plus, edit, delete, copy, download
Status        - Check, X, warning, info
User          - Person, team, settings
File          - Document, folder, upload
Code          - Terminal, brackets, git
```

### Icon Usage Guidelines
- Use 16px icons for inline text and buttons
- Use 20px icons for navigation items
- Use 24px icons for feature highlights
- Maintain 1.5px stroke width for consistency
- Icons should be centered within their bounding box

### Icon Colors
```css
.icon-default { color: var(--text-secondary); }
.icon-primary { color: var(--text-primary); }
.icon-brand { color: var(--brand-green); }
.icon-muted { color: var(--text-muted); }
.icon-success { color: var(--success); }
.icon-warning { color: var(--warning); }
.icon-error { color: var(--error); }
```

---

## 7. Layout & Grid

### Container System
```css
.container {
  width: 100%;
  max-width: var(--container-max-width);
  margin: 0 auto;
  padding: 0 var(--container-padding);
}

.container-sm { max-width: 640px; }
.container-md { max-width: 768px; }
.container-lg { max-width: 1024px; }
.container-xl { max-width: 1280px; }
.container-2xl { max-width: 1536px; }
```

### Grid System
```css
.grid {
  display: grid;
  gap: var(--gap-stack-md);
}

.grid-cols-1 { grid-template-columns: repeat(1, 1fr); }
.grid-cols-2 { grid-template-columns: repeat(2, 1fr); }
.grid-cols-3 { grid-template-columns: repeat(3, 1fr); }
.grid-cols-4 { grid-template-columns: repeat(4, 1fr); }
.grid-cols-6 { grid-template-columns: repeat(6, 1fr); }
.grid-cols-12 { grid-template-columns: repeat(12, 1fr); }
```

### Dashboard Layout
```css
.dashboard-layout {
  display: grid;
  grid-template-columns: var(--sidebar-width) 1fr;
  grid-template-rows: var(--header-height) 1fr;
  min-height: 100vh;
}

.dashboard-sidebar {
  grid-row: 1 / -1;
  grid-column: 1;
  background: var(--background-darker);
  border-right: 1px solid var(--border-default);
}

.dashboard-header {
  grid-row: 1;
  grid-column: 2;
  background: var(--background-dark);
  border-bottom: 1px solid var(--border-default);
}

.dashboard-main {
  grid-row: 2;
  grid-column: 2;
  background: var(--background-dark);
  padding: var(--space-6);
  overflow-y: auto;
}
```

### Panel Layout (SQL Editor)
```css
.panel-layout {
  display: grid;
  grid-template-columns: 250px 1fr 300px;
  height: calc(100vh - var(--header-height));
}

.panel-sidebar {
  background: var(--background-darker);
  border-right: 1px solid var(--border-default);
  overflow-y: auto;
}

.panel-main {
  display: flex;
  flex-direction: column;
}

.panel-editor {
  flex: 1;
  overflow: hidden;
}

.panel-results {
  height: 40%;
  border-top: 1px solid var(--border-default);
  overflow: auto;
}

.panel-inspector {
  background: var(--background-darker);
  border-left: 1px solid var(--border-default);
  overflow-y: auto;
}
```

### Breakpoints
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;

@media (max-width: 1024px) {
  .dashboard-layout {
    grid-template-columns: 1fr;
  }
  
  .dashboard-sidebar {
    position: fixed;
    transform: translateX(-100%);
    z-index: 200;
  }
  
  .dashboard-sidebar.open {
    transform: translateX(0);
  }
}
```

### Z-Index Scale
```css
--z-dropdown: 100;
--z-sticky: 200;
--z-modal-backdrop: 300;
--z-modal: 400;
--z-popover: 500;
--z-tooltip: 600;
--z-toast: 700;
```

---

## 8. Animation & Motion

### Timing Functions
```css
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

### Duration Scale
```css
--duration-instant: 50ms;
--duration-fast: 150ms;
--duration-normal: 200ms;
--duration-slow: 300ms;
--duration-slower: 500ms;
```

### Transition Presets
```css
.transition-colors {
  transition: color var(--duration-fast) var(--ease-default),
              background-color var(--duration-fast) var(--ease-default),
              border-color var(--duration-fast) var(--ease-default);
}

.transition-transform {
  transition: transform var(--duration-normal) var(--ease-default);
}

.transition-opacity {
  transition: opacity var(--duration-normal) var(--ease-default);
}

.transition-all {
  transition: all var(--duration-normal) var(--ease-default);
}
```

### Animation Keyframes

#### Fade In
```css
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.animate-fade-in {
  animation: fadeIn var(--duration-normal) var(--ease-out);
}
```

#### Slide In
```css
@keyframes slideInUp {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideInDown {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-10px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideInRight {
  from {
    opacity: 0;
    transform: translateX(10px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}
```

#### Scale
```css
@keyframes scaleIn {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

.animate-scale-in {
  animation: scaleIn var(--duration-normal) var(--ease-out);
}
```

#### Pulse (Loading/Active States)
```css
@keyframes pulse {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: 0.5;
  }
}

.animate-pulse {
  animation: pulse 2s var(--ease-in-out) infinite;
}
```

#### Spin (Loading)
```css
@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.animate-spin {
  animation: spin 1s linear infinite;
}
```

#### Glow Effect
```css
@keyframes glow {
  0%, 100% {
    box-shadow: 0 0 5px rgba(62, 207, 142, 0.3);
  }
  50% {
    box-shadow: 0 0 20px rgba(62, 207, 142, 0.5);
  }
}

.animate-glow {
  animation: glow 2s var(--ease-in-out) infinite;
}
```

### Interactive States
```css
/* Hover lift effect */
.hover-lift {
  transition: transform var(--duration-normal) var(--ease-out),
              box-shadow var(--duration-normal) var(--ease-out);
}

.hover-lift:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
}

/* Button press effect */
.press-effect:active {
  transform: scale(0.98);
}

/* Focus ring animation */
@keyframes focusRing {
  0% {
    box-shadow: 0 0 0 0 rgba(62, 207, 142, 0.4);
  }
  100% {
    box-shadow: 0 0 0 4px rgba(62, 207, 142, 0);
  }
}
```

### Page Transitions
```css
/* Route change fade */
.page-enter {
  opacity: 0;
}

.page-enter-active {
  opacity: 1;
  transition: opacity var(--duration-slow) var(--ease-out);
}

.page-exit {
  opacity: 1;
}

.page-exit-active {
  opacity: 0;
  transition: opacity var(--duration-fast) var(--ease-in);
}
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

---

## 9. Design Patterns & Best Practices

### Code-First Design Philosophy
Supabase prioritizes developer experience with a code-centric approach to all interfaces.

#### SQL Editor Pattern
- Full-featured code editor with syntax highlighting
- Auto-completion for SQL keywords, table names, and columns
- Query history and saved queries sidebar
- Results displayed in tabular format below editor
- Real-time query execution feedback

#### API Documentation Style
```
Pattern: Interactive API reference with code examples

Structure:
1. Endpoint description
2. Request parameters (table format)
3. Code examples in multiple languages (JavaScript, Python, cURL)
4. Response schema
5. Try-it-out section (live API calls)
```

### Dashboard Patterns

#### Project Overview
```
Layout:
- Status cards at top (database health, API requests, storage)
- Quick actions panel (run SQL, create table, invite team)
- Recent activity timeline
- Resource usage graphs
```

#### Table Editor
```
Layout:
- Left sidebar: Table list with search
- Main area: Table grid with inline editing
- Right panel: Column inspector / Row details
- Bottom: Action bar (Add row, filters, export)

Interactions:
- Click cell to edit inline
- Double-click header to rename column
- Drag to resize columns
- Right-click for context menu
```

#### Authentication Interface
```
Pattern: Provider-based auth configuration

Structure:
1. Provider grid (Email, Google, GitHub, etc.)
2. Enable/disable toggles
3. Configuration forms per provider
4. User management table
5. Policy editor for Row Level Security
```

### Form Patterns

#### Settings Form
```css
.settings-section {
  border-bottom: 1px solid var(--border-default);
  padding: 24px 0;
}

.settings-section:last-child {
  border-bottom: none;
}

.settings-header {
  margin-bottom: 16px;
}

.settings-title {
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 4px;
}

.settings-description {
  font-size: 14px;
  color: var(--text-secondary);
}

.settings-field {
  margin-top: 16px;
}

.settings-actions {
  display: flex;
  justify-content: flex-end;
  gap: 12px;
  margin-top: 24px;
  padding-top: 24px;
  border-top: 1px solid var(--border-default);
}
```

#### Connection String Display
```css
.connection-string {
  background: var(--background-darkest);
  border: 1px solid var(--border-default);
  border-radius: 6px;
  padding: 12px 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
}

.connection-string-value {
  flex: 1;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  color: var(--text-secondary);
}

.connection-string-value.revealed {
  color: var(--text-primary);
}
```

### Terminal Integration Pattern
```
CLI Command Display:
- Show command with copy button
- Syntax highlight command parts
- Display expected output
- Show progress indicators for long operations
```

```css
.cli-command {
  display: flex;
  align-items: center;
  gap: 8px;
  background: var(--background-darkest);
  padding: 12px 16px;
  border-radius: 6px;
  font-family: var(--font-mono);
}

.cli-prompt {
  color: var(--text-muted);
  user-select: none;
}

.cli-text {
  flex: 1;
  color: var(--brand-green);
}

.cli-copy {
  color: var(--text-muted);
  cursor: pointer;
  transition: color var(--duration-fast);
}

.cli-copy:hover {
  color: var(--text-primary);
}
```

### Open Source Branding

#### Community Elements
- GitHub stars counter
- Contributor avatars
- Changelog/release notes integration
- Community links (Discord, Twitter, GitHub)

#### Transparency Indicators
```css
.badge-open-source {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  background: rgba(62, 207, 142, 0.1);
  border: 1px solid rgba(62, 207, 142, 0.2);
  border-radius: 4px;
  font-size: 12px;
  color: var(--brand-green);
}
```

### Empty States
```css
.empty-state {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 64px 24px;
  text-align: center;
}

.empty-state-icon {
  width: 64px;
  height: 64px;
  margin-bottom: 24px;
  color: var(--text-muted);
}

.empty-state-title {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 8px;
  color: var(--text-primary);
}

.empty-state-description {
  font-size: 14px;
  color: var(--text-secondary);
  max-width: 400px;
  margin-bottom: 24px;
}
```

### Loading States
```css
/* Skeleton loading */
.skeleton {
  background: linear-gradient(
    90deg,
    var(--surface-dark) 25%,
    var(--surface-elevated) 50%,
    var(--surface-dark) 75%
  );
  background-size: 200% 100%;
  animation: skeleton 1.5s ease infinite;
  border-radius: 4px;
}

@keyframes skeleton {
  0% {
    background-position: 200% 0;
  }
  100% {
    background-position: -200% 0;
  }
}

/* Spinner */
.spinner {
  width: 20px;
  height: 20px;
  border: 2px solid var(--border-default);
  border-top-color: var(--brand-green);
  border-radius: 50%;
  animation: spin 0.8s linear infinite;
}
```

### Error Handling
```css
.error-boundary {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 48px;
  text-align: center;
  background: var(--error-light);
  border: 1px solid rgba(239, 68, 68, 0.2);
  border-radius: 8px;
}

.inline-error {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 12px;
  background: var(--error-light);
  border-radius: 4px;
  font-size: 13px;
  color: var(--error);
}
```

### Accessibility Guidelines

#### Focus Management
```css
/* Visible focus for keyboard navigation */
:focus-visible {
  outline: 2px solid var(--brand-green);
  outline-offset: 2px;
}

/* Skip link for screen readers */
.skip-link {
  position: absolute;
  top: -100%;
  left: 0;
  background: var(--brand-green);
  color: #111111;
  padding: 12px 24px;
  z-index: 9999;
  transition: top var(--duration-fast);
}

.skip-link:focus {
  top: 0;
}
```

#### Color Contrast
- All text must meet WCAG 2.1 AA standards
- Primary text (#FFFFFF) on dark backgrounds (#1C1C1C) = 12.63:1
- Secondary text (#B3B3B3) on dark backgrounds = 7.18:1
- Brand green (#3ECF8E) on dark backgrounds = 8.42:1

#### Screen Reader Support
- Use semantic HTML elements
- Provide aria-labels for icon-only buttons
- Include alt text for all images
- Use aria-live regions for dynamic content updates

### Responsive Behavior

#### Mobile Adaptations
- Sidebar collapses to drawer/overlay
- Tables become horizontally scrollable or card-based
- Touch-friendly tap targets (minimum 44x44px)
- Simplified navigation with bottom tab bar option

#### Desktop Optimizations
- Multi-panel layouts for power users
- Keyboard shortcuts for common actions
- Hover states for additional information
- Drag-and-drop functionality

---

## Appendix: CSS Custom Properties Summary

```css
:root {
  /* Colors */
  --brand-green: #3ECF8E;
  --brand-green-light: #4FF8A8;
  --brand-green-dark: #24B47E;
  
  --background-dark: #1C1C1C;
  --background-darker: #111111;
  --background-darkest: #0A0A0A;
  --surface-dark: #1F1F1F;
  --surface-elevated: #252525;
  
  --text-primary: #FFFFFF;
  --text-secondary: #B3B3B3;
  --text-muted: #666666;
  
  --border-default: #2E2E2E;
  --border-light: #3A3A3A;
  
  --success: #3ECF8E;
  --warning: #F5A623;
  --error: #EF4444;
  --info: #3B82F6;
  
  /* Typography */
  --font-sans: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-mono: 'Source Code Pro', 'SF Mono', Monaco, monospace;
  
  /* Spacing */
  --space-unit: 4px;
  --container-max-width: 1280px;
  --sidebar-width: 256px;
  --header-height: 56px;
  
  /* Animation */
  --duration-fast: 150ms;
  --duration-normal: 200ms;
  --ease-default: cubic-bezier(0.4, 0, 0.2, 1);
  
  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.3);
  --shadow-md: 0 4px 6px rgba(0, 0, 0, 0.3);
  --shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.4);
  --shadow-glow: 0 0 20px rgba(62, 207, 142, 0.3);
  
  /* Border Radius */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  --radius-full: 9999px;
}
```

---

*Last Updated: April 2026*
*Version: 1.0.0*
