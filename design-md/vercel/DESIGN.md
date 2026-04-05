# Vercel Design System (Geist)

> Developer infrastructure platform with extreme minimalism. Pure black (#171717) and white (#ffffff) foundation, Geist typeface with aggressive letter-spacing, shadow-as-border technique, gallery-like whitespace.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Vercel embodies **Swiss design principles meets developer tooling**. The interface feels like a high-end art gallery—meticulously curated whitespace, surgical precision in every element, and an almost austere restraint. Every pixel serves a purpose. The design whispers rather than shouts, letting the developer's work take center stage.

### Mood & Feeling
- **Clinical precision**: Mathematical spacing, pixel-perfect alignment, obsessive attention to detail
- **Confident minimalism**: Reduction to essentials, nothing decorative or superfluous
- **Professional gravity**: Serious tooling for serious developers, no playfulness
- **Future-forward**: Cutting-edge without trend-chasing, timeless modernism
- **Infrastructure confidence**: Conveys reliability through visual restraint

### Design Density
**Low density** with deliberate abundance of whitespace. The interface breathes—generous padding, ample margins, and gallery-style spacing between elements. Information is presented sparingly, creating focus and reducing cognitive load for developers managing complex deployments.

### Visual Character
- Extreme negative space (40-80px margins common)
- Shadow-as-border technique instead of visible borders
- Multi-layer shadow stacks creating subtle depth
- Monochromatic palette with workflow color accents
- Typography as the primary design element
- Ultra-subtle interaction states
- Grid-perfect alignment throughout

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--geist-foreground` | `#171717` | Primary text, icons, active elements |
| `--geist-background` | `#ffffff` | Primary background, page base |
| `--geist-foreground-rgb` | `23, 23, 23` | RGB value for alpha operations |
| `--geist-background-rgb` | `255, 255, 255` | RGB value for alpha operations |

### Gray Scale (Light Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--accents-1` | `#fafafa` | Subtle backgrounds, hover states |
| `--accents-2` | `#eaeaea` | Dividers, subtle borders |
| `--accents-3` | `#999999` | Placeholder text, disabled icons |
| `--accents-4` | `#888888` | Secondary text, metadata |
| `--accents-5` | `#666666` | Tertiary text, timestamps |
| `--accents-6` | `#444444` | Strong secondary text |
| `--accents-7` | `#333333` | Near-primary text |
| `--accents-8` | `#111111` | Headlines, maximum emphasis |

### Gray Scale (Dark Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--geist-background` | `#000000` | Pure black background |
| `--accents-1` | `#111111` | Elevated surfaces |
| `--accents-2` | `#333333` | Subtle borders, dividers |
| `--accents-3` | `#444444` | Placeholder text |
| `--accents-4` | `#666666` | Secondary text |
| `--accents-5` | `#888888` | Tertiary text |
| `--accents-6` | `#999999` | Metadata |
| `--accents-7` | `#eaeaea` | Primary body text |
| `--accents-8` | `#fafafa` | Headlines, maximum emphasis |

### Workflow Colors (The Vercel Triad)

| Token | Hex | Role |
|-------|-----|------|
| `--geist-error` / Ship | `#ff5b4f` | Production, errors, Ship workflow |
| `--geist-warning` / Preview | `#de1d8d` | Preview deployments, staging |
| `--geist-success` / Develop | `#0a72ef` | Development, local, success indicators |

### Extended Workflow Palette

| Token | Hex | Role |
|-------|-----|------|
| `--geist-error-light` | `#ff8a82` | Error backgrounds, light mode |
| `--geist-error-dark` | `#e5443a` | Error hover states |
| `--geist-warning-light` | `#e94da0` | Preview hover states |
| `--geist-warning-dark` | `#c0176f` | Preview active states |
| `--geist-success-light` | `#3d8ef2` | Success backgrounds |
| `--geist-success-dark` | `#0860c7` | Success active states |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--geist-cyan` | `#79ffe1` | Highlights, special callouts |
| `--geist-purple` | `#f81ce5` | Premium features, pro badges |
| `--geist-violet` | `#7928ca` | AI features, experimental |
| `--geist-alert` | `#ff0080` | Critical alerts, urgent notices |

### Focus & Interaction

| Token | Hex | Role |
|-------|-----|------|
| `--focus-ring` | `hsla(212, 100%, 48%, 1)` | Keyboard focus indicator |
| `--focus-ring-alpha` | `hsla(212, 100%, 48%, 0.5)` | Focus ring with transparency |
| `--selection-bg` | `rgba(0, 112, 243, 0.15)` | Text selection background |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary UI Font - Geist Sans */
--font-sans: 'Geist', -apple-system, BlinkMacSystemFont, 'Segoe UI', 
             'Roboto', 'Oxygen', 'Ubuntu', sans-serif;

/* Monospace - Geist Mono */
--font-mono: 'Geist Mono', 'SF Mono', 'Fira Code', 'Fira Mono', 
             'Roboto Mono', 'Menlo', monospace;
```

### Type Scale with Letter Spacing

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 64px | 700 | 1.1 | -0.04em | `--accents-8` |
| Page Title | 48px | 700 | 1.15 | -0.035em | `--accents-8` |
| Section Title | 32px | 600 | 1.2 | -0.03em | `--accents-8` |
| Card Title | 24px | 600 | 1.25 | -0.025em | `--geist-foreground` |
| Subsection | 20px | 600 | 1.3 | -0.02em | `--geist-foreground` |
| Large Body | 18px | 400 | 1.6 | -0.01em | `--accents-6` |
| Body | 16px | 400 | 1.6 | -0.01em | `--accents-5` |
| Small Body | 14px | 400 | 1.5 | -0.006em | `--accents-5` |
| Caption | 13px | 400 | 1.4 | 0 | `--accents-4` |
| Tiny | 12px | 500 | 1.4 | 0 | `--accents-4` |
| Label | 12px | 500 | 1.3 | 0.02em | `--accents-4` |
| Code Inline | 14px | 400 | 1.6 | 0 | `--geist-foreground` |
| Code Block | 14px | 400 | 1.7 | 0 | `--accents-7` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, descriptions, paragraphs |
| 500 | Medium | Labels, metadata, table headers |
| 600 | Semibold | Card titles, navigation items, buttons |
| 700 | Bold | Headlines, page titles, emphasis |

### Letter Spacing Philosophy
Vercel employs **aggressive negative letter-spacing** on headlines, tightening character spacing as size increases. This creates a dense, confident, magazine-quality typographic presence. The tighter tracking on large text reads as more modern and premium.

```css
/* Letter spacing scale */
--tracking-tighter: -0.04em;  /* 48px+ headlines */
--tracking-tight: -0.025em;   /* 24-32px titles */
--tracking-normal: -0.01em;   /* 16-18px body */
--tracking-wide: 0.02em;      /* Labels, buttons */
```

### Monospace Typography (Geist Mono)

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Code Block | 14px | 400 | Multi-line code, terminal output |
| Inline Code | 13px | 400 | Technical terms in prose |
| Terminal | 13px | 400 | CLI examples, commands |
| File Path | 12px | 400 | Breadcrumbs, file names |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Black)
```css
.button-primary {
  background: #171717;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 0 12px;
  height: 36px;
  border-radius: 6px;
  border: none;
  letter-spacing: 0;
  transition: all 150ms ease;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
}

.button-primary:hover {
  background: #333333;
}

.button-primary:active {
  background: #444444;
  transform: scale(0.98);
}

.button-primary:focus-visible {
  outline: none;
  box-shadow: 0 0 0 2px #ffffff,
              0 0 0 4px hsla(212, 100%, 48%, 1);
}

.button-primary:disabled {
  background: #fafafa;
  color: #999999;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.button-secondary {
  background: #ffffff;
  color: #171717;
  font-size: 14px;
  font-weight: 500;
  padding: 0 12px;
  height: 36px;
  border-radius: 6px;
  border: none;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
  transition: all 150ms ease;
}

.button-secondary:hover {
  background: #fafafa;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.15);
}

.button-secondary:active {
  background: #f5f5f5;
}
```

#### Ghost Button (Minimal)
```css
.button-ghost {
  background: transparent;
  color: #666666;
  font-size: 14px;
  font-weight: 500;
  padding: 0 8px;
  height: 32px;
  border-radius: 6px;
  border: none;
}

.button-ghost:hover {
  background: #fafafa;
  color: #171717;
}
```

#### Danger Button
```css
.button-danger {
  background: #ff5b4f;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 0 12px;
  height: 36px;
  border-radius: 6px;
}

.button-danger:hover {
  background: #e5443a;
}
```

#### Button Sizes

| Size | Height | Padding | Font Size |
|------|--------|---------|-----------|
| Small | 28px | 0 8px | 13px |
| Medium (default) | 36px | 0 12px | 14px |
| Large | 44px | 0 16px | 15px |

### Inputs

#### Text Input
```css
.input {
  background: #ffffff;
  color: #171717;
  font-size: 14px;
  font-family: var(--font-sans);
  padding: 0 12px;
  height: 40px;
  border-radius: 6px;
  border: none;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
  transition: box-shadow 150ms ease;
  width: 100%;
}

.input:hover {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.15);
}

.input:focus {
  outline: none;
  box-shadow: 0 0 0 1px #171717;
}

.input::placeholder {
  color: #999999;
}

.input:disabled {
  background: #fafafa;
  color: #999999;
  cursor: not-allowed;
}

.input-error {
  box-shadow: 0 0 0 1px #ff5b4f;
}
```

#### Input with Label
```css
.input-label {
  font-size: 14px;
  font-weight: 500;
  color: #171717;
  margin-bottom: 8px;
  display: block;
}

.input-helper {
  font-size: 13px;
  color: #666666;
  margin-top: 6px;
}

.input-error-text {
  font-size: 13px;
  color: #ff5b4f;
  margin-top: 6px;
}
```

#### Search Input
```css
.search-input {
  background: #fafafa;
  padding-left: 36px; /* Space for icon */
  box-shadow: none;
}

.search-input:focus {
  background: #ffffff;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
}
```

### Cards

#### Standard Card
```css
.card {
  background: #ffffff;
  border-radius: 8px;
  padding: 24px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
  transition: box-shadow 200ms ease;
}

.card:hover {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.12),
              0 4px 8px rgba(0, 0, 0, 0.04);
}
```

#### Elevated Card (Multi-Layer Shadow)
```css
.card-elevated {
  background: #ffffff;
  border-radius: 8px;
  padding: 24px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.03),
              0 2px 4px rgba(0, 0, 0, 0.02),
              0 4px 8px rgba(0, 0, 0, 0.02),
              0 8px 16px rgba(0, 0, 0, 0.02),
              0 16px 32px rgba(0, 0, 0, 0.02);
}
```

#### Interactive Card
```css
.card-interactive {
  background: #ffffff;
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
  cursor: pointer;
  transition: all 200ms ease;
}

.card-interactive:hover {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.15),
              0 8px 16px rgba(0, 0, 0, 0.06);
  transform: translateY(-1px);
}

.card-interactive:active {
  transform: translateY(0);
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.12);
}
```

#### Project Card
```css
.project-card {
  background: #ffffff;
  border-radius: 8px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
  overflow: hidden;
}

.project-card-preview {
  height: 200px;
  background: linear-gradient(180deg, #fafafa 0%, #f5f5f5 100%);
  border-bottom: 1px solid #eaeaea;
}

.project-card-content {
  padding: 16px 20px;
}

.project-card-title {
  font-size: 16px;
  font-weight: 600;
  color: #171717;
  letter-spacing: -0.01em;
  margin-bottom: 4px;
}

.project-card-meta {
  font-size: 13px;
  color: #666666;
}
```

### Deployment Status Badges

```css
.badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 500;
}

.badge-ready {
  background: rgba(10, 114, 239, 0.1);
  color: #0a72ef;
}

.badge-building {
  background: rgba(222, 29, 141, 0.1);
  color: #de1d8d;
}

.badge-error {
  background: rgba(255, 91, 79, 0.1);
  color: #ff5b4f;
}

.badge-queued {
  background: #fafafa;
  color: #666666;
}

.badge-dot {
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: currentColor;
}

.badge-dot-animated {
  animation: pulse 1.5s infinite;
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.4; }
}
```

### Navigation

#### Tab Navigation
```css
.tabs {
  display: flex;
  gap: 4px;
  padding: 4px;
  background: #fafafa;
  border-radius: 8px;
}

.tab {
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #666666;
  background: transparent;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  transition: all 150ms ease;
}

.tab:hover {
  color: #171717;
}

.tab-active {
  background: #ffffff;
  color: #171717;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 2px 4px rgba(0, 0, 0, 0.04);
}
```

#### Sidebar Navigation
```css
.nav-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px 12px;
  font-size: 14px;
  font-weight: 500;
  color: #666666;
  border-radius: 6px;
  transition: all 150ms ease;
}

.nav-item:hover {
  background: #fafafa;
  color: #171717;
}

.nav-item-active {
  background: #fafafa;
  color: #171717;
}

.nav-item-icon {
  width: 20px;
  height: 20px;
  opacity: 0.7;
}

.nav-item:hover .nav-item-icon,
.nav-item-active .nav-item-icon {
  opacity: 1;
}
```

### Tables

```css
.table {
  width: 100%;
  border-collapse: collapse;
}

.table-header {
  border-bottom: 1px solid #eaeaea;
}

.table-header th {
  padding: 12px 16px;
  font-size: 13px;
  font-weight: 500;
  color: #666666;
  text-align: left;
  background: #fafafa;
}

.table-row {
  border-bottom: 1px solid #eaeaea;
  transition: background 150ms ease;
}

.table-row:hover {
  background: #fafafa;
}

.table-cell {
  padding: 16px;
  font-size: 14px;
  color: #171717;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(4px);
}

.modal {
  background: #ffffff;
  border-radius: 12px;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 16px 48px rgba(0, 0, 0, 0.12);
  max-width: 480px;
  width: 100%;
  overflow: hidden;
}

.modal-header {
  padding: 20px 24px;
  border-bottom: 1px solid #eaeaea;
}

.modal-title {
  font-size: 18px;
  font-weight: 600;
  color: #171717;
  letter-spacing: -0.02em;
}

.modal-body {
  padding: 24px;
}

.modal-footer {
  padding: 16px 24px;
  background: #fafafa;
  display: flex;
  justify-content: flex-end;
  gap: 8px;
}
```

### Tooltips

```css
.tooltip {
  background: #171717;
  color: #ffffff;
  font-size: 13px;
  font-weight: 500;
  padding: 8px 12px;
  border-radius: 6px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  max-width: 200px;
}

.tooltip-arrow {
  fill: #171717;
}
```

### Code Blocks

```css
.code-block {
  background: #fafafa;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 14px;
  line-height: 1.7;
  overflow-x: auto;
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);
}

/* Dark theme code block */
.code-block-dark {
  background: #111111;
  color: #fafafa;
}

.code-inline {
  background: #fafafa;
  padding: 2px 6px;
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #de1d8d; /* Pink for inline code */
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | 4px | Tight element gaps, icon padding |
| `--space-2` | 8px | Small gaps, compact layouts |
| `--space-3` | 12px | Standard element spacing |
| `--space-4` | 16px | Card padding, section gaps |
| `--space-5` | 24px | Large card padding, component separation |
| `--space-6` | 32px | Section padding |
| `--space-7` | 48px | Major section breaks |
| `--space-8` | 64px | Page section separation |
| `--space-9` | 80px | Hero padding, gallery spacing |
| `--space-10` | 128px | Maximum breathing room |

### Core Layout Structure

```
┌────────────────────────────────────────────────────────────────────┐
│  ┌─────────────────────────────────────────────────────────────┐  │
│  │                    Top Navigation (64px)                     │  │
│  │  Logo    Dashboard    Deployments    Analytics    Settings   │  │
│  └─────────────────────────────────────────────────────────────┘  │
│                                                                    │
│  ┌──────────┬────────────────────────────────────────────────┐    │
│  │          │                                                 │    │
│  │  Sidebar │                Main Content                     │    │
│  │  (240px) │                (Flexible)                       │    │
│  │          │                                                 │    │
│  │  Project │           ┌─────────────────────────┐           │    │
│  │  Nav     │           │    Content Container    │           │    │
│  │          │           │      (max-width)        │           │    │
│  │          │           └─────────────────────────┘           │    │
│  │          │                                                 │    │
│  └──────────┴────────────────────────────────────────────────┘    │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Content Widths

| Context | Max Width | Centering |
|---------|-----------|-----------|
| Dashboard Content | 1200px | Centered |
| Documentation | 768px | Centered |
| Settings/Forms | 560px | Left-aligned |
| Modal Content | 480px | Centered |
| Landing Page Hero | 1400px | Centered |

### Grid System

```css
/* Dashboard Grid */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
}

/* Stats Grid */
.stats-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
}

/* Two-Column Layout */
.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 32px;
}
```

### Whitespace Philosophy
Vercel treats whitespace as a **primary design element**, not empty space. The abundant margins and padding create:
- Focus by isolation (important elements breathe)
- Hierarchy through spatial relationships
- Premium feel through gallery-like presentation
- Reduced cognitive load through information scarcity

### Container Patterns

```css
/* Page Container */
.page-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 48px 24px;
}

/* Section Container */
.section {
  padding: 64px 0;
}

/* Compact Section */
.section-compact {
  padding: 32px 0;
}

/* Gallery Section (Marketing) */
.section-gallery {
  padding: 128px 48px;
}
```

---

## 6. Depth & Elevation

### Shadow-as-Border Technique

Vercel's signature approach uses `box-shadow` instead of `border` to create subtle, refined edges that don't add to element sizing:

```css
/* Standard border shadow */
box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08);

/* Emphasized border shadow */
box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.12);

/* Strong border shadow */
box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.15);

/* Focus state */
box-shadow: 0 0 0 1px #171717;
```

### Multi-Layer Shadow Stack

Vercel uses stacked shadows for premium depth:

```css
/* Level 1 - Subtle lift */
.shadow-sm {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 2px 4px rgba(0, 0, 0, 0.04);
}

/* Level 2 - Standard card */
.shadow-md {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 4px 8px rgba(0, 0, 0, 0.04),
              0 8px 16px rgba(0, 0, 0, 0.04);
}

/* Level 3 - Elevated card */
.shadow-lg {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.03),
              0 2px 4px rgba(0, 0, 0, 0.02),
              0 4px 8px rgba(0, 0, 0, 0.02),
              0 8px 16px rgba(0, 0, 0, 0.02),
              0 16px 32px rgba(0, 0, 0, 0.02);
}

/* Level 4 - Modal/Dropdown */
.shadow-xl {
  box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.08),
              0 8px 16px rgba(0, 0, 0, 0.08),
              0 16px 32px rgba(0, 0, 0, 0.08),
              0 32px 64px rgba(0, 0, 0, 0.08);
}
```

### Surface Hierarchy (Light Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Elevated (Dropdowns, Modals)       #ffffff + shadow-xl  │
├─────────────────────────────────────────────────────────┤
│ Cards (Standard)                   #ffffff + shadow     │
├─────────────────────────────────────────────────────────┤
│ Subtle Background                  #fafafa              │
├─────────────────────────────────────────────────────────┤
│ Page Background                    #ffffff              │
└─────────────────────────────────────────────────────────┘
```

### Surface Hierarchy (Dark Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Elevated (Dropdowns, Modals)       #1a1a1a + shadow     │
├─────────────────────────────────────────────────────────┤
│ Cards (Standard)                   #111111              │
├─────────────────────────────────────────────────────────┤
│ Subtle Background                  #0a0a0a              │
├─────────────────────────────────────────────────────────┤
│ Page Background                    #000000              │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, cards |
| Sticky | 100 | Navigation, headers |
| Dropdown | 200 | Menus, autocomplete |
| Modal | 300 | Dialogs, full-screen overlays |
| Toast | 400 | Notifications |
| Tooltip | 500 | Tooltips, popovers |
| Maximum | 9999 | Debug overlays |

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use shadow-as-border technique | Refined edges without box-model impact |
| Apply aggressive negative letter-spacing on headlines | Modern, premium typographic presence |
| Embrace generous whitespace | Gallery-like focus and reduced cognitive load |
| Use the workflow triad (Red/Pink/Blue) semantically | Consistent meaning across Ship/Preview/Develop |
| Keep interactions minimal and fast (<200ms) | Developer efficiency, no wasted time |
| Use Geist Sans and Geist Mono exclusively | Brand consistency, optimized legibility |
| Prefer monochrome palette with color as exception | Intentional color draws appropriate attention |
| Use multi-layer shadow stacks for depth | Premium, realistic elevation |
| Keep border-radius consistent (6px buttons, 8px cards) | Visual harmony |
| Show system status clearly with badges | Deployment clarity is critical |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never use visible borders (1px solid) | Shadow-as-border is the standard |
| Avoid decorative elements or ornamentation | Contradicts minimalist philosophy |
| Don't use gradients on UI elements | Reserved for marketing/special cases |
| Never use rounded-full on rectangular elements | Only pills and avatars use full radius |
| Avoid dense, cluttered layouts | Whitespace is a feature, not a bug |
| Don't use color for decoration | Color is semantic, not aesthetic |
| Never use positive letter-spacing on body text | Counter to Geist's tight aesthetic |
| Avoid animations >200ms for UI interactions | Perceived sluggishness |
| Don't mix font families | Geist Sans + Mono only |
| Never use pure black (#000000) in light mode | Reserve for dark mode backgrounds |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use clear, technical language | Use marketing fluff in the dashboard |
| Provide specific error messages | Show generic "Something went wrong" |
| Show deployment URLs prominently | Hide or abbreviate URLs |
| Use consistent terminology (Deploy, Preview, Build) | Mix terminology (Launch, Stage, Compile) |
| Display timestamps in relative format ("2m ago") | Show only absolute timestamps |
| Confirm destructive actions | Delete without warning |
| Show loading states with progress | Use indefinite spinners when progress is known |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Mobile | <640px | Single column, stacked navigation |
| Tablet | 640px - 1024px | Collapsible sidebar, 2-column grids |
| Desktop | 1024px - 1440px | Full layout, 3-4 column grids |
| Wide | >1440px | Maximum content width, centered |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Navigation | Horizontal top bar | Hamburger menu + drawer |
| Sidebar | Fixed 240px | Full-screen overlay |
| Project Grid | 3-4 columns | Single column |
| Deployment List | Table view | Card stack |
| Actions | Inline buttons | Bottom sheet or dropdown |
| Tabs | Horizontal scroll | Horizontal scroll (same) |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Buttons | 44px height | Comfortable tap target |
| Navigation Items | 48px height | Larger for quick navigation |
| Form Inputs | 44px height | Standard mobile input |
| Icon Buttons | 40px × 40px | Square touch targets |
| List Items | Full width × 56px | Easy row selection |

### Responsive Typography

| Element | Desktop | Mobile |
|---------|---------|--------|
| Hero Display | 64px | 36px |
| Page Title | 48px | 28px |
| Section Title | 32px | 24px |
| Body | 16px | 16px |
| Caption | 13px | 13px |

### Adaptive Spacing

```css
/* Mobile spacing reduction */
@media (max-width: 640px) {
  --space-7: 32px;   /* 48px desktop */
  --space-8: 48px;   /* 64px desktop */
  --space-9: 64px;   /* 80px desktop */
  --space-10: 80px;  /* 128px desktop */
}
```

### Image Handling

- **Deployment Screenshots**: Full-width on mobile, cropped preview on desktop
- **Avatars**: 32px mobile, 40px desktop
- **Logo marks**: 24px consistent across breakpoints
- **Graphics**: Lazy-loaded, responsive srcset

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Colors
Primary Black: #171717
Primary White: #ffffff
Ship Red: #ff5b4f
Preview Pink: #de1d8d
Develop Blue: #0a72ef

# Grays (Light)
Background: #ffffff
Subtle Background: #fafafa
Border (shadow): rgba(0, 0, 0, 0.08)
Secondary Text: #666666
Primary Text: #171717

# Typography
Font Primary: 'Geist', system-ui, sans-serif
Font Mono: 'Geist Mono', monospace
Headline Tracking: -0.04em to -0.025em
Body Tracking: -0.01em

# Radii
Button Radius: 6px
Card Radius: 8px
Modal Radius: 12px
Badge Radius: 100px

# Focus
Focus Ring: hsla(212, 100%, 48%, 1)

# Shadows
Border Shadow: 0 0 0 1px rgba(0, 0, 0, 0.08)
Card Shadow: Multi-layer stack
```

### Example Prompts

#### Deployment Card
```
Create a deployment card using Vercel's Geist design system:
- Card background: #ffffff with 8px border-radius
- Shadow-as-border: 0 0 0 1px rgba(0, 0, 0, 0.08)
- Hover: Add 0 4px 8px rgba(0, 0, 0, 0.04) shadow layer
- Padding: 20px
- Project name: 16px semibold #171717, letter-spacing -0.01em
- Branch name: 14px regular #666666 with Geist Mono
- Status badge: Pill shape, 12px medium weight
  - Ready: #0a72ef text on rgba(10, 114, 239, 0.1) background
  - Building: #de1d8d text on rgba(222, 29, 141, 0.1) background
  - Error: #ff5b4f text on rgba(255, 91, 79, 0.1) background
- Timestamp: 13px #999999 relative format
```

#### Navigation Header
```
Design a navigation header following Vercel conventions:
- Height: 64px
- Background: #ffffff with border-bottom shadow
- Border: box-shadow: 0 1px 0 0 rgba(0, 0, 0, 0.08)
- Logo: Vercel triangle, 20px, #171717
- Nav items: 14px medium #666666, hover #171717
- Active nav: #171717 with subtle background #fafafa
- Spacing between items: 24px
- Right-aligned user menu: Avatar + dropdown chevron
```

#### Form Input Group
```
Create a form input following Vercel's design:
- Label: 14px medium #171717, margin-bottom 8px
- Input height: 40px
- Border radius: 6px
- Border: box-shadow 0 0 0 1px rgba(0, 0, 0, 0.08)
- Focus: box-shadow 0 0 0 1px #171717
- Padding: 0 12px
- Font: 14px Geist Sans, #171717
- Placeholder: #999999
- Helper text: 13px #666666, margin-top 6px
- Error state: Red border shadow, red helper text #ff5b4f
```

#### Modal Dialog
```
Design a confirmation modal:
- Overlay: rgba(0, 0, 0, 0.5) with backdrop-filter blur(4px)
- Modal: #ffffff, 12px border-radius
- Shadow: Multi-layer xl shadow stack
- Width: 480px max
- Header: 20px padding, 18px semibold title, bottom border
- Body: 24px padding
- Footer: #fafafa background, 16px padding
- Buttons: 6px radius, 36px height
- Cancel: Secondary (outline)
- Confirm: Primary black or Danger red
```

#### Workflow Status Component
```
Create a workflow status indicator:
- Use the Vercel triad colors semantically:
- Production/Ship: #ff5b4f (red)
- Preview/Staging: #de1d8d (pink)
- Development: #0a72ef (blue)
- Status dot: 8px circle with matching color
- Status text: 14px medium, same color as dot
- Background pill: 8px vertical padding, full-radius
- Background color: 10% opacity of status color
```

### CSS Variables Template

```css
:root {
  /* Core */
  --geist-foreground: #171717;
  --geist-background: #ffffff;
  
  /* Grays */
  --accents-1: #fafafa;
  --accents-2: #eaeaea;
  --accents-3: #999999;
  --accents-4: #888888;
  --accents-5: #666666;
  --accents-6: #444444;
  --accents-7: #333333;
  --accents-8: #111111;
  
  /* Workflow */
  --geist-error: #ff5b4f;
  --geist-warning: #de1d8d;
  --geist-success: #0a72ef;
  
  /* Typography */
  --font-sans: 'Geist', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-mono: 'Geist Mono', 'SF Mono', monospace;
  
  /* Tracking */
  --tracking-tighter: -0.04em;
  --tracking-tight: -0.025em;
  --tracking-normal: -0.01em;
  
  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 24px;
  --space-6: 32px;
  --space-7: 48px;
  --space-8: 64px;
  
  /* Radii */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  --radius-full: 100px;
  
  /* Shadows */
  --shadow-border: 0 0 0 1px rgba(0, 0, 0, 0.08);
  --shadow-sm: 0 0 0 1px rgba(0, 0, 0, 0.08), 0 2px 4px rgba(0, 0, 0, 0.04);
  --shadow-md: 0 0 0 1px rgba(0, 0, 0, 0.08), 0 4px 8px rgba(0, 0, 0, 0.04);
  --shadow-lg: 0 0 0 1px rgba(0, 0, 0, 0.03), 0 2px 4px rgba(0, 0, 0, 0.02), 
               0 4px 8px rgba(0, 0, 0, 0.02), 0 8px 16px rgba(0, 0, 0, 0.02), 
               0 16px 32px rgba(0, 0, 0, 0.02);
  
  /* Focus */
  --focus-ring: hsla(212, 100%, 48%, 1);
  
  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
}

/* Dark Theme */
[data-theme="dark"] {
  --geist-foreground: #ededed;
  --geist-background: #000000;
  
  --accents-1: #111111;
  --accents-2: #333333;
  --accents-3: #444444;
  --accents-4: #666666;
  --accents-5: #888888;
  --accents-6: #999999;
  --accents-7: #eaeaea;
  --accents-8: #fafafa;
  
  --shadow-border: 0 0 0 1px rgba(255, 255, 255, 0.08);
}
```

---

## Summary

Vercel's Geist design system embodies **developer infrastructure minimalism** through:

1. **Pure black and white foundation** with workflow color accents (#ff5b4f, #de1d8d, #0a72ef)
2. **Shadow-as-border technique** replacing traditional borders with refined box-shadow
3. **Aggressive negative letter-spacing** on Geist typeface for premium typography
4. **Gallery-like whitespace** with 48-80px+ margins creating focus
5. **Multi-layer shadow stacks** for realistic, premium depth
6. **Consistent 6px/8px border radius** system for visual harmony
7. **Monochromatic palette** with semantic color as exception

When implementing Vercel-style interfaces, prioritize:
- Surgical precision in spacing and alignment
- Typography as the primary design element
- Restraint over decoration
- Shadow-based depth and borders
- Clear workflow status communication
- Fast, minimal interactions
