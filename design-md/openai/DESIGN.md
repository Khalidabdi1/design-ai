# OpenAI Design System

> Research-driven AI company with academic elegance. Clean whites (#ffffff) and conversational darks (#212121, #343541), signature ChatGPT green (#10a37f), Söhne typeface with precise letter-spacing, research paper aesthetic meets modern product design.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
OpenAI embodies **academic rigor meets accessible technology**. The interface feels like a modern research publication—clean, purposeful, and intellectually sophisticated. Every element communicates credibility while maintaining approachability. The design balances the gravitas of cutting-edge AI research with the usability demands of millions of daily users.

### Mood & Feeling
- **Scholarly authority**: Research paper cleanliness, institutional trust, intellectual weight
- **Approachable intelligence**: Complex technology made accessible, not intimidating
- **Conversational warmth**: ChatGPT interface invites dialogue, feels personal
- **Purposeful minimalism**: Every element serves function, nothing decorative
- **Future-forward optimism**: Green accent suggests growth, progress, positive AI outcomes

### Design Density
**Medium-low density** with intentional breathing room. The ChatGPT interface prioritizes conversation space, while documentation uses generous margins typical of academic publications. Information is presented with enough whitespace to allow focus without feeling sparse.

### Visual Character
- Clean white backgrounds with high contrast text
- Conversational dark mode for extended use
- Signature green (#10a37f) as trust indicator
- Typography-first design approach
- Rounded corners softening technical content
- Subtle shadows creating gentle depth
- Card-based content organization
- Academic paper influence in documentation

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--primary-white` | `#ffffff` | Light mode background, cards |
| `--primary-dark` | `#212121` | Dark mode background base |
| `--chat-dark` | `#343541` | ChatGPT dark mode conversation bg |
| `--chat-input-dark` | `#40414f` | ChatGPT input area dark mode |
| `--text-primary` | `#202123` | Primary text light mode |

### Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--openai-green` | `#10a37f` | Primary accent, CTAs, ChatGPT brand |
| `--openai-green-hover` | `#0d8a6a` | Green hover state |
| `--openai-green-light` | `#d1fae5` | Green backgrounds, highlights |
| `--openai-green-subtle` | `rgba(16, 163, 127, 0.1)` | Subtle green backgrounds |

### Gray Scale (Light Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--gray-50` | `#f7f7f8` | Subtle backgrounds, hover states |
| `--gray-100` | `#ececf1` | Dividers, borders |
| `--gray-200` | `#d9d9e3` | Disabled states, secondary borders |
| `--gray-300` | `#c5c5d2` | Placeholder text |
| `--gray-400` | `#8e8ea0` | Secondary text, metadata |
| `--gray-500` | `#6e6e80` | Tertiary text |
| `--gray-600` | `#565869` | Body text (light mode) |
| `--gray-700` | `#353740` | Strong secondary text |
| `--gray-800` | `#202123` | Primary text |
| `--gray-900` | `#0d0d0d` | Maximum emphasis |

### Gray Scale (Dark Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--dark-bg` | `#212121` | Page background |
| `--dark-surface` | `#2f2f2f` | Elevated surfaces |
| `--dark-surface-hover` | `#3a3a3a` | Hover states |
| `--dark-border` | `#4d4d4d` | Borders, dividers |
| `--dark-text-primary` | `#ececec` | Primary text |
| `--dark-text-secondary` | `#b4b4b4` | Secondary text |
| `--dark-text-tertiary` | `#8e8e8e` | Tertiary text |

### ChatGPT Specific Colors

| Token | Hex | Role |
|-------|-----|------|
| `--chat-bg-light` | `#ffffff` | User message background (light) |
| `--chat-bg-assistant` | `#f7f7f8` | Assistant message background (light) |
| `--chat-bg-dark` | `#343541` | Conversation area (dark) |
| `--chat-sidebar-dark` | `#202123` | Sidebar background (dark) |
| `--chat-hover-dark` | `#2a2b32` | Sidebar hover (dark) |
| `--chat-selected-dark` | `#343541` | Selected conversation (dark) |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--error-red` | `#ef4146` | Errors, destructive actions |
| `--error-bg` | `#fef2f2` | Error backgrounds |
| `--warning-orange` | `#f59e0b` | Warnings, caution states |
| `--warning-bg` | `#fffbeb` | Warning backgrounds |
| `--success-green` | `#10a37f` | Success, confirmation |
| `--success-bg` | `#d1fae5` | Success backgrounds |
| `--info-blue` | `#3b82f6` | Information, links |
| `--info-bg` | `#eff6ff` | Info backgrounds |

### API & Documentation Colors

| Token | Hex | Role |
|-------|-----|------|
| `--code-purple` | `#7c3aed` | API endpoints |
| `--code-blue` | `#2563eb` | Method names |
| `--code-green` | `#059669` | Strings, success |
| `--code-orange` | `#ea580c` | Warnings, deprecated |
| `--code-pink` | `#db2777` | Keywords |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary UI Font - Söhne */
--font-sans: 'Söhne', -apple-system, BlinkMacSystemFont, 'Segoe UI', 
             'Roboto', 'Helvetica Neue', Arial, sans-serif;

/* Monospace - Söhne Mono */
--font-mono: 'Söhne Mono', 'SF Mono', 'Fira Code', 'Fira Mono', 
             'Roboto Mono', 'Menlo', monospace;

/* Fallback System Stack */
--font-system: -apple-system, BlinkMacSystemFont, 'Segoe UI', 
               'Roboto', 'Helvetica Neue', Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 56px | 600 | 1.1 | -0.02em | `--gray-900` |
| Page Title | 40px | 600 | 1.2 | -0.015em | `--gray-900` |
| Section Title | 32px | 600 | 1.25 | -0.01em | `--gray-800` |
| Card Title | 24px | 600 | 1.3 | -0.01em | `--gray-800` |
| Subsection | 20px | 600 | 1.35 | -0.005em | `--gray-800` |
| Large Body | 18px | 400 | 1.6 | 0 | `--gray-600` |
| Body | 16px | 400 | 1.6 | 0 | `--gray-600` |
| Small Body | 14px | 400 | 1.5 | 0 | `--gray-500` |
| Caption | 13px | 400 | 1.4 | 0 | `--gray-400` |
| Label | 12px | 500 | 1.4 | 0.01em | `--gray-500` |
| Chat Message | 16px | 400 | 1.75 | 0 | `--gray-800` |
| Code Inline | 14px | 400 | 1.6 | 0 | `--code-purple` |
| Code Block | 14px | 400 | 1.6 | 0 | `--gray-800` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, chat messages, descriptions |
| 500 | Medium | Labels, navigation, metadata |
| 600 | Semibold | Headlines, titles, buttons |
| 700 | Bold | Maximum emphasis, critical actions |

### Typography Philosophy
OpenAI's typography balances **academic precision with conversational warmth**. The Söhne typeface provides a distinctive, modern feel while remaining highly readable for extended chat interactions. Headlines use restrained negative tracking for a refined appearance, while body text maintains neutral spacing for optimal readability.

```css
/* Letter spacing scale */
--tracking-tight: -0.02em;   /* Hero headlines */
--tracking-snug: -0.01em;    /* Section titles */
--tracking-normal: 0;        /* Body text */
--tracking-wide: 0.01em;     /* Labels, buttons */
```

### Monospace Typography (Söhne Mono)

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Code Block | 14px | 400 | Multi-line code, API examples |
| Inline Code | 13px | 400 | Technical terms, parameters |
| Terminal | 13px | 400 | CLI commands |
| API Endpoint | 14px | 500 | API documentation |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Green)
```css
.button-primary {
  background: #10a37f;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 16px;
  height: 40px;
  border-radius: 6px;
  border: none;
  letter-spacing: 0;
  transition: background 150ms ease;
}

.button-primary:hover {
  background: #0d8a6a;
}

.button-primary:active {
  background: #0b7a5e;
}

.button-primary:focus-visible {
  outline: none;
  box-shadow: 0 0 0 2px #ffffff,
              0 0 0 4px #10a37f;
}

.button-primary:disabled {
  background: #d9d9e3;
  color: #8e8ea0;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.button-secondary {
  background: #ffffff;
  color: #202123;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 16px;
  height: 40px;
  border-radius: 6px;
  border: 1px solid #d9d9e3;
  transition: all 150ms ease;
}

.button-secondary:hover {
  background: #f7f7f8;
  border-color: #c5c5d2;
}

.button-secondary:active {
  background: #ececf1;
}
```

#### Ghost Button
```css
.button-ghost {
  background: transparent;
  color: #6e6e80;
  font-size: 14px;
  font-weight: 500;
  padding: 8px 12px;
  height: 36px;
  border-radius: 6px;
  border: none;
}

.button-ghost:hover {
  background: #f7f7f8;
  color: #202123;
}
```

#### Dark Mode Button
```css
.button-dark {
  background: #10a37f;
  color: #ffffff;
}

.button-dark-secondary {
  background: transparent;
  color: #ececec;
  border: 1px solid #4d4d4d;
}

.button-dark-secondary:hover {
  background: #2f2f2f;
}
```

#### Button Sizes

| Size | Height | Padding | Font Size |
|------|--------|---------|-----------|
| Small | 32px | 8px 12px | 13px |
| Medium (default) | 40px | 10px 16px | 14px |
| Large | 48px | 12px 24px | 16px |

### Inputs

#### Text Input
```css
.input {
  background: #ffffff;
  color: #202123;
  font-size: 16px;
  font-family: var(--font-sans);
  padding: 10px 12px;
  height: 44px;
  border-radius: 8px;
  border: 1px solid #d9d9e3;
  transition: border-color 150ms ease;
  width: 100%;
}

.input:hover {
  border-color: #c5c5d2;
}

.input:focus {
  outline: none;
  border-color: #10a37f;
  box-shadow: 0 0 0 1px #10a37f;
}

.input::placeholder {
  color: #8e8ea0;
}

.input:disabled {
  background: #f7f7f8;
  color: #8e8ea0;
  cursor: not-allowed;
}

.input-error {
  border-color: #ef4146;
}

.input-error:focus {
  box-shadow: 0 0 0 1px #ef4146;
}
```

#### ChatGPT Input (Dark)
```css
.chat-input {
  background: #40414f;
  color: #ececec;
  font-size: 16px;
  padding: 12px 48px 12px 16px;
  border-radius: 12px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  min-height: 52px;
  max-height: 200px;
  resize: none;
}

.chat-input:focus {
  outline: none;
  border-color: rgba(255, 255, 255, 0.2);
}

.chat-input::placeholder {
  color: #8e8ea0;
}
```

### Cards

#### Standard Card
```css
.card {
  background: #ffffff;
  border-radius: 12px;
  padding: 24px;
  border: 1px solid #ececf1;
  transition: box-shadow 200ms ease;
}

.card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
}
```

#### Feature Card
```css
.card-feature {
  background: #ffffff;
  border-radius: 16px;
  padding: 32px;
  border: 1px solid #ececf1;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.card-feature-icon {
  width: 48px;
  height: 48px;
  background: #d1fae5;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
}

.card-feature-icon svg {
  color: #10a37f;
  width: 24px;
  height: 24px;
}
```

#### Conversation Card (Sidebar)
```css
.conversation-card {
  background: transparent;
  border-radius: 8px;
  padding: 12px;
  cursor: pointer;
  transition: background 150ms ease;
}

.conversation-card:hover {
  background: #2a2b32;
}

.conversation-card-active {
  background: #343541;
}

.conversation-card-title {
  font-size: 14px;
  color: #ececec;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

#### API Pricing Card
```css
.pricing-card {
  background: #ffffff;
  border-radius: 16px;
  padding: 32px;
  border: 1px solid #ececf1;
  text-align: center;
}

.pricing-card-featured {
  border-color: #10a37f;
  position: relative;
}

.pricing-card-badge {
  position: absolute;
  top: -12px;
  left: 50%;
  transform: translateX(-50%);
  background: #10a37f;
  color: #ffffff;
  font-size: 12px;
  font-weight: 500;
  padding: 4px 12px;
  border-radius: 100px;
}
```

### Chat Messages

#### User Message
```css
.message-user {
  background: #f7f7f8;
  border-radius: 16px;
  padding: 16px 20px;
  margin: 8px 0;
  max-width: 70%;
  margin-left: auto;
}

/* Dark mode */
.message-user-dark {
  background: #343541;
  color: #ececec;
}
```

#### Assistant Message
```css
.message-assistant {
  background: transparent;
  padding: 16px 0;
  border-bottom: 1px solid #ececf1;
}

.message-assistant-avatar {
  width: 32px;
  height: 32px;
  background: #10a37f;
  border-radius: 6px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.message-assistant-content {
  font-size: 16px;
  line-height: 1.75;
  color: #202123;
}

/* Dark mode */
.message-assistant-dark {
  border-color: rgba(255, 255, 255, 0.1);
}

.message-assistant-content-dark {
  color: #ececec;
}
```

### Navigation

#### Top Navigation
```css
.nav-header {
  height: 64px;
  background: #ffffff;
  border-bottom: 1px solid #ececf1;
  display: flex;
  align-items: center;
  padding: 0 24px;
}

.nav-logo {
  font-size: 20px;
  font-weight: 600;
  color: #202123;
}

.nav-item {
  font-size: 14px;
  font-weight: 500;
  color: #6e6e80;
  padding: 8px 16px;
  border-radius: 6px;
  transition: all 150ms ease;
}

.nav-item:hover {
  color: #202123;
  background: #f7f7f8;
}

.nav-item-active {
  color: #202123;
}
```

#### ChatGPT Sidebar
```css
.sidebar {
  width: 260px;
  background: #202123;
  padding: 8px;
  display: flex;
  flex-direction: column;
  height: 100vh;
}

.sidebar-new-chat {
  background: transparent;
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 8px;
  padding: 12px;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  display: flex;
  align-items: center;
  gap: 12px;
  cursor: pointer;
  transition: background 150ms ease;
}

.sidebar-new-chat:hover {
  background: rgba(255, 255, 255, 0.1);
}
```

### Code Blocks

```css
.code-block {
  background: #f7f7f8;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 14px;
  line-height: 1.6;
  overflow-x: auto;
  border: 1px solid #ececf1;
}

.code-block-header {
  background: #ececf1;
  padding: 8px 16px;
  border-radius: 8px 8px 0 0;
  font-size: 12px;
  font-weight: 500;
  color: #6e6e80;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.code-block-body {
  border-radius: 0 0 8px 8px;
}

/* Dark mode code block */
.code-block-dark {
  background: #1e1e1e;
  border-color: #3a3a3a;
}

.code-block-header-dark {
  background: #2d2d2d;
  color: #b4b4b4;
}

.code-inline {
  background: #f7f7f8;
  padding: 2px 6px;
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #7c3aed;
}
```

### Badges & Status

```css
.badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 6px;
  font-size: 12px;
  font-weight: 500;
}

.badge-success {
  background: #d1fae5;
  color: #059669;
}

.badge-warning {
  background: #fef3c7;
  color: #d97706;
}

.badge-error {
  background: #fee2e2;
  color: #dc2626;
}

.badge-info {
  background: #dbeafe;
  color: #2563eb;
}

.badge-neutral {
  background: #f7f7f8;
  color: #6e6e80;
}

.badge-pro {
  background: linear-gradient(135deg, #7c3aed 0%, #db2777 100%);
  color: #ffffff;
}
```

### Tooltips

```css
.tooltip {
  background: #202123;
  color: #ffffff;
  font-size: 13px;
  font-weight: 400;
  padding: 8px 12px;
  border-radius: 6px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  max-width: 240px;
}

.tooltip-arrow {
  fill: #202123;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(4px);
}

.modal {
  background: #ffffff;
  border-radius: 16px;
  box-shadow: 0 24px 48px rgba(0, 0, 0, 0.16);
  max-width: 500px;
  width: 100%;
  overflow: hidden;
}

.modal-header {
  padding: 24px 24px 0;
}

.modal-title {
  font-size: 20px;
  font-weight: 600;
  color: #202123;
}

.modal-body {
  padding: 16px 24px 24px;
}

.modal-footer {
  padding: 16px 24px;
  background: #f7f7f8;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
}

/* Dark modal */
.modal-dark {
  background: #2f2f2f;
}

.modal-title-dark {
  color: #ececec;
}

.modal-footer-dark {
  background: #212121;
}
```

---

## 5. Layout Principles

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | 4px | Tight gaps, icon padding |
| `--space-2` | 8px | Small gaps, inline spacing |
| `--space-3` | 12px | Compact element spacing |
| `--space-4` | 16px | Standard element spacing |
| `--space-5` | 20px | Card content spacing |
| `--space-6` | 24px | Section padding |
| `--space-7` | 32px | Large section gaps |
| `--space-8` | 48px | Major section separation |
| `--space-9` | 64px | Page section breaks |
| `--space-10` | 96px | Hero spacing |

### Core Layout Structure

#### ChatGPT Interface
```
┌────────────────────────────────────────────────────────────────────┐
│  ┌───────────┬────────────────────────────────────────────────┐   │
│  │           │                                                 │   │
│  │  Sidebar  │              Conversation Area                  │   │
│  │  (260px)  │                                                 │   │
│  │           │     ┌────────────────────────────────────┐     │   │
│  │  History  │     │       Message Thread                │     │   │
│  │  List     │     │       (max-width: 768px)           │     │   │
│  │           │     │       (centered)                    │     │   │
│  │           │     └────────────────────────────────────┘     │   │
│  │           │                                                 │   │
│  │           │     ┌────────────────────────────────────┐     │   │
│  │           │     │         Input Area                  │     │   │
│  │           │     │       (fixed bottom)               │     │   │
│  │           │     └────────────────────────────────────┘     │   │
│  └───────────┴────────────────────────────────────────────────┘   │
└────────────────────────────────────────────────────────────────────┘
```

#### Documentation Layout
```
┌────────────────────────────────────────────────────────────────────┐
│  ┌─────────────────────────────────────────────────────────────┐  │
│  │                    Top Navigation (64px)                     │  │
│  │  Logo    API    Documentation    Research    Products        │  │
│  └─────────────────────────────────────────────────────────────┘  │
│                                                                    │
│  ┌───────────┬──────────────────────────────┬───────────────┐     │
│  │           │                               │               │     │
│  │  Sidebar  │       Content Area           │   On-Page     │     │
│  │  (240px)  │       (max: 768px)           │   Nav (200px) │     │
│  │           │                               │               │     │
│  │  Section  │    Research paper-style       │   Table of    │     │
│  │  Nav      │    typography and spacing     │   Contents    │     │
│  │           │                               │               │     │
│  └───────────┴──────────────────────────────┴───────────────┘     │
└────────────────────────────────────────────────────────────────────┘
```

### Content Widths

| Context | Max Width | Centering |
|---------|-----------|-----------|
| Chat Messages | 768px | Centered |
| Documentation | 768px | Centered |
| Landing Page Content | 1200px | Centered |
| API Playground | 100% | Full-width |
| Settings/Forms | 560px | Left-aligned |
| Modal Content | 500px | Centered |

### Grid System

```css
/* Feature Grid */
.grid-features {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

/* Pricing Grid */
.grid-pricing {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}

/* Documentation Grid */
.grid-docs {
  display: grid;
  grid-template-columns: 240px 1fr 200px;
  gap: 48px;
}
```

### Whitespace Philosophy
OpenAI uses whitespace to create **focus and hierarchy**. The ChatGPT interface maximizes conversation readability with generous line heights and message spacing, while documentation follows academic paper conventions with wider margins and clear section breaks.

---

## 6. Depth & Elevation

### Shadow System

```css
/* Level 0 - Flat */
.shadow-none {
  box-shadow: none;
}

/* Level 1 - Subtle lift */
.shadow-sm {
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
}

/* Level 2 - Card default */
.shadow-md {
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

/* Level 3 - Elevated card */
.shadow-lg {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

/* Level 4 - Dropdown/Popover */
.shadow-xl {
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}

/* Level 5 - Modal */
.shadow-2xl {
  box-shadow: 0 24px 48px rgba(0, 0, 0, 0.16);
}
```

### Border System

```css
/* Light theme borders */
--border-light: 1px solid #ececf1;
--border-light-subtle: 1px solid #f7f7f8;
--border-light-strong: 1px solid #d9d9e3;

/* Dark theme borders */
--border-dark: 1px solid rgba(255, 255, 255, 0.1);
--border-dark-subtle: 1px solid rgba(255, 255, 255, 0.05);
--border-dark-strong: 1px solid rgba(255, 255, 255, 0.2);

/* Focus border */
--border-focus: 1px solid #10a37f;
```

### Surface Hierarchy (Light Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Modal (Elevated)                    #ffffff + shadow-2xl │
├─────────────────────────────────────────────────────────┤
│ Dropdown/Popover                    #ffffff + shadow-xl  │
├─────────────────────────────────────────────────────────┤
│ Cards (Hover)                       #ffffff + shadow-lg  │
├─────────────────────────────────────────────────────────┤
│ Cards (Default)                     #ffffff + border     │
├─────────────────────────────────────────────────────────┤
│ Subtle Background                   #f7f7f8              │
├─────────────────────────────────────────────────────────┤
│ Page Background                     #ffffff              │
└─────────────────────────────────────────────────────────┘
```

### Surface Hierarchy (Dark Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Modal (Elevated)                    #3a3a3a + shadow     │
├─────────────────────────────────────────────────────────┤
│ Dropdown/Popover                    #2f2f2f + shadow     │
├─────────────────────────────────────────────────────────┤
│ Input Area                          #40414f              │
├─────────────────────────────────────────────────────────┤
│ Conversation Area                   #343541              │
├─────────────────────────────────────────────────────────┤
│ Sidebar                             #202123              │
├─────────────────────────────────────────────────────────┤
│ Page Background                     #212121              │
└─────────────────────────────────────────────────────────┘
```

### Z-Index Scale

| Layer | Z-Index | Elements |
|-------|---------|----------|
| Base | 0 | Main content, messages |
| Sticky | 100 | Navigation headers |
| Dropdown | 200 | Menus, autocomplete |
| Sidebar Overlay | 250 | Mobile sidebar |
| Modal | 300 | Dialogs |
| Toast | 400 | Notifications |
| Tooltip | 500 | Tooltips |

---

## 7. Do's and Don'ts

### Do's

| Guideline | Rationale |
|-----------|-----------|
| Use green (#10a37f) for primary actions | Brand recognition, positive association |
| Apply generous line-height (1.6-1.75) for chat | Readability for extended conversations |
| Keep message containers centered and constrained | Optimal reading width, focus |
| Use rounded corners (8-16px) on containers | Friendly, approachable feel |
| Implement both light and dark themes | User preference, eye comfort |
| Show typing indicators during AI responses | User feedback, expectation setting |
| Use subtle borders over heavy shadows | Clean, academic aesthetic |
| Apply Söhne font consistently | Brand identity, readability |
| Provide clear copy buttons for code | Utility for developers |
| Show token/character counts where relevant | Transparency about API usage |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never use bright, saturated colors for UI elements | Contradicts sophisticated aesthetic |
| Avoid dense information layouts | Chat requires breathing room |
| Don't use multiple accent colors | Green is the singular brand color |
| Never hide the AI attribution | Transparency is core to trust |
| Avoid aggressive animations | Professional, calm environment |
| Don't use small text for chat messages | Readability is paramount |
| Never auto-submit without user confirmation | Respect user control |
| Avoid inconsistent dark mode colors | Coherent theme is essential |
| Don't truncate code blocks aggressively | Technical utility matters |
| Never use generic system fonts in UI | Söhne is brand-defining |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use clear, helpful AI responses | Use jargon without explanation |
| Show examples with code | Provide abstract explanations only |
| Indicate when AI is uncertain | Assert false confidence |
| Provide citations for research claims | Make unverified claims |
| Use consistent model naming (GPT-4, etc.) | Use internal codenames |
| Show rate limits and usage clearly | Hide limitations |
| Explain capabilities and limitations | Overpromise functionality |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Mobile | <640px | Full-width chat, collapsible sidebar |
| Tablet | 640px - 1024px | Overlay sidebar, 2-column layouts |
| Desktop | 1024px - 1440px | Full layout, persistent sidebar |
| Wide | >1440px | Maximum content width, centered |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Sidebar | Persistent 260px | Full-screen overlay |
| Chat Messages | 768px max-width | Full width with padding |
| Navigation | Full items | Hamburger menu |
| Input Area | Single row expandable | Full width, larger touch targets |
| Code Blocks | Horizontal scroll | Horizontal scroll |
| Modal | Centered 500px | Full screen or bottom sheet |

### Touch Targets

| Element | Minimum Size | Notes |
|---------|--------------|-------|
| Buttons | 44px height | iOS guidelines |
| Send Button | 48px × 48px | Critical action |
| Navigation Items | 48px height | Easy thumb access |
| Conversation Items | Full width × 56px | Easy selection |
| Input Field | 52px min-height | Comfortable typing |

### Responsive Typography

| Element | Desktop | Mobile |
|---------|---------|--------|
| Hero Display | 56px | 36px |
| Page Title | 40px | 28px |
| Section Title | 32px | 24px |
| Chat Message | 16px | 16px |
| Body | 16px | 16px |
| Caption | 13px | 13px |

### Chat Interface Responsive

```css
/* Mobile: Full width */
@media (max-width: 640px) {
  .chat-container {
    max-width: 100%;
    padding: 0 16px;
  }
  
  .sidebar {
    position: fixed;
    z-index: 250;
    transform: translateX(-100%);
  }
  
  .sidebar-open {
    transform: translateX(0);
  }
}

/* Tablet: Overlay sidebar */
@media (min-width: 640px) and (max-width: 1024px) {
  .sidebar {
    position: fixed;
    z-index: 250;
  }
}

/* Desktop: Persistent sidebar */
@media (min-width: 1024px) {
  .sidebar {
    position: relative;
    flex-shrink: 0;
  }
}
```

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Brand Colors
Primary Green: #10a37f
Green Hover: #0d8a6a
Green Light: #d1fae5

# Light Mode
Background: #ffffff
Surface: #f7f7f8
Border: #ececf1
Text Primary: #202123
Text Secondary: #6e6e80

# Dark Mode (ChatGPT)
Background: #212121
Sidebar: #202123
Conversation: #343541
Input Area: #40414f
Text Primary: #ececec
Text Secondary: #b4b4b4

# Typography
Font Primary: 'Söhne', system-ui, sans-serif
Font Mono: 'Söhne Mono', monospace
Chat Line Height: 1.75

# Radii
Small: 6px
Medium: 8px
Large: 12px
XL: 16px
Full: 100px

# Focus
Focus Ring: 0 0 0 2px #ffffff, 0 0 0 4px #10a37f
```

### Example Prompts

#### Chat Message Component
```
Create a ChatGPT-style message using OpenAI's design system:
- Container: max-width 768px, centered, padding 16px 0
- User message: #f7f7f8 background (light), 16px border-radius
- Assistant message: transparent background, bottom border #ececf1
- Avatar: 32px square, #10a37f background, 6px radius for AI
- Message text: 16px Söhne, line-height 1.75, #202123
- Dark mode user: #343541 background
- Dark mode assistant: border rgba(255, 255, 255, 0.1)
- Spacing between messages: 16px
```

#### ChatGPT Input Area
```
Design the ChatGPT input component:
- Container: fixed bottom, full width, #343541 background
- Inner wrapper: max-width 768px, centered
- Input: #40414f background, 12px border-radius
- Border: 1px solid rgba(255, 255, 255, 0.1)
- Placeholder: "Message ChatGPT" in #8e8ea0
- Send button: 40px circle, #10a37f when active
- Disabled send: #6e6e80
- Font: 16px Söhne, #ececec
- Min-height: 52px, max-height: 200px (expandable)
```

#### API Playground
```
Create API playground interface following OpenAI patterns:
- Split layout: 50% request, 50% response
- Code editor: dark theme #1e1e1e background
- Syntax highlighting with purple (#7c3aed) for keywords
- Request panel: input fields with #f7f7f8 background
- Response panel: formatted JSON with line numbers
- Run button: #10a37f primary style, "Run" label
- Model selector: dropdown with all GPT model options
- Parameter sliders: green accent for active state
```

#### Documentation Page
```
Design a documentation page in OpenAI's style:
- Three-column layout: 240px nav, flexible content, 200px TOC
- Content max-width: 768px
- Heading hierarchy: 32px/24px/20px, semibold
- Body: 16px, line-height 1.6, #565869
- Code blocks: #f7f7f8 with header showing language
- Copy button: ghost style, appears on hover
- Inline code: purple #7c3aed on #f7f7f8
- Tables: clean borders #ececf1, header #f7f7f8
- Warning callouts: orange left border, #fffbeb background
```

#### Settings Modal
```
Create a settings modal for ChatGPT:
- Overlay: rgba(0, 0, 0, 0.6) with backdrop blur
- Modal: #2f2f2f background (dark), 16px border-radius
- Width: 500px max
- Header: 24px padding, "Settings" in 20px semibold #ececec
- Tab navigation: horizontal, #8e8ea0 inactive, #ececec active
- Content sections: 24px padding
- Toggle switches: 44px wide, #10a37f when active
- Close button: ghost style, top right
- Save button: primary green style
```

### CSS Variables Template

```css
:root {
  /* Core Colors */
  --openai-green: #10a37f;
  --openai-green-hover: #0d8a6a;
  --openai-green-light: #d1fae5;
  
  /* Light Theme */
  --bg-primary: #ffffff;
  --bg-secondary: #f7f7f8;
  --text-primary: #202123;
  --text-secondary: #6e6e80;
  --text-tertiary: #8e8ea0;
  --border-color: #ececf1;
  --border-strong: #d9d9e3;
  
  /* Typography */
  --font-sans: 'Söhne', -apple-system, BlinkMacSystemFont, sans-serif;
  --font-mono: 'Söhne Mono', 'SF Mono', monospace;
  
  /* Tracking */
  --tracking-tight: -0.02em;
  --tracking-snug: -0.01em;
  --tracking-normal: 0;
  
  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 20px;
  --space-6: 24px;
  --space-7: 32px;
  --space-8: 48px;
  
  /* Radii */
  --radius-sm: 6px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-full: 100px;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
  --shadow-md: 0 2px 8px rgba(0, 0, 0, 0.08);
  --shadow-lg: 0 4px 12px rgba(0, 0, 0, 0.1);
  --shadow-xl: 0 8px 24px rgba(0, 0, 0, 0.12);
  --shadow-2xl: 0 24px 48px rgba(0, 0, 0, 0.16);
  
  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
}

/* Dark Theme (ChatGPT) */
[data-theme="dark"] {
  --bg-primary: #212121;
  --bg-secondary: #2f2f2f;
  --bg-chat: #343541;
  --bg-sidebar: #202123;
  --bg-input: #40414f;
  
  --text-primary: #ececec;
  --text-secondary: #b4b4b4;
  --text-tertiary: #8e8e8e;
  
  --border-color: rgba(255, 255, 255, 0.1);
  --border-strong: rgba(255, 255, 255, 0.2);
}
```

---

## Summary

OpenAI's design system embodies **academic authority with conversational accessibility** through:

1. **Clean white foundation** with research paper-inspired typography and spacing
2. **Signature green (#10a37f)** as singular brand accent conveying trust and progress
3. **Söhne typeface** with generous line-heights (1.6-1.75) for extended readability
4. **ChatGPT dark theme** (#212121, #343541) optimized for long conversations
5. **Rounded corners** (8-16px) softening technical interfaces
6. **Subtle borders over shadows** for clean, academic aesthetic
7. **Centered, constrained content** (768px max) for optimal reading

When implementing OpenAI-style interfaces, prioritize:
- Conversation-first layouts with ample breathing room
- Consistent green accent for primary actions only
- Clear distinction between user and AI messages
- Readable code blocks with copy functionality
- Both light and dark theme support
- Transparent AI indicators and attributions
- Academic precision in typography and spacing
