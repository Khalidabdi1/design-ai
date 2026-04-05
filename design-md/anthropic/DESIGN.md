# Anthropic (Claude) Design System

> AI safety research company with warm editorial elegance. Cream backgrounds (#FAF9F5) and warm terracotta accents (#DA7756, #C4553D), dark charcoal text (#1F1915), Styrene typeface with clean letter-spacing, research paper aesthetic meets thoughtful product design—trustworthy, warm, and safety-focused.

---

## 1. Visual Theme & Atmosphere

### Overall Aesthetic
Anthropic embodies **thoughtful research meets human warmth**. The interface feels like a carefully crafted academic journal—warm, considered, and intellectually rigorous. Every element communicates trustworthiness while maintaining approachability. The design balances the gravitas of AI safety research with an inviting, human-centered experience that distinguishes Claude from purely technical competitors.

### Mood & Feeling
- **Scholarly warmth**: Research paper refinement with inviting, human tones
- **Trustworthy intelligence**: Safety-first ethos reflected in considered design choices
- **Conversational depth**: Claude's interface invites thoughtful dialogue and reflection
- **Editorial precision**: Every element has purpose, nothing is superfluous
- **Optimistic restraint**: Warm coral accents suggest capability with responsibility
- **Minimal chrome**: Content-first approach, interface fades to support conversation

### Design Density
**Low-to-medium density** with generous breathing room. The Claude interface prioritizes conversation clarity, while documentation uses academic journal-style margins. Information is presented with ample whitespace to encourage focused, thoughtful engagement without feeling sparse or clinical.

### Visual Character
- Warm cream backgrounds (#FAF9F5) as foundation
- Dark warm gray text (#1F1915) for excellent readability
- Terracotta/coral accent (#DA7756) as trust indicator
- Typography-first design with editorial sensibility
- Subtle rounded corners creating approachable feel
- Minimal shadows, relying on subtle tonal shifts
- Card-based content with warm borders
- Research paper influence throughout documentation
- Deliberate absence of visual noise

---

## 2. Color Palette & Roles

### Core Foundation

| Token | Hex | Role |
|-------|-----|------|
| `--bg-cream` | `#FAF9F5` | Primary background, page base |
| `--bg-cream-deep` | `#F5F3ED` | Subtle surface differentiation |
| `--bg-warm-white` | `#FFFFFE` | Cards, elevated surfaces |
| `--text-primary` | `#1F1915` | Primary text, headlines |
| `--text-warm-dark` | `#2D2825` | Strong secondary text |

### Brand Colors

| Token | Hex | Role |
|-------|-----|------|
| `--anthropic-coral` | `#DA7756` | Primary accent, Claude brand |
| `--anthropic-terracotta` | `#C4553D` | Darker coral, CTAs, active states |
| `--anthropic-coral-light` | `#F5DDD4` | Coral backgrounds, highlights |
| `--anthropic-coral-subtle` | `rgba(218, 119, 86, 0.12)` | Subtle coral tints |
| `--anthropic-coral-hover` | `#E88B6A` | Hover state for coral elements |

### Warm Gray Scale (Light Theme)

| Token | Hex | Role |
|-------|-----|------|
| `--warm-50` | `#FAF9F7` | Lightest background |
| `--warm-100` | `#F5F3EF` | Subtle backgrounds, hover states |
| `--warm-200` | `#EBE8E2` | Dividers, borders |
| `--warm-300` | `#DDD9D1` | Disabled states, secondary borders |
| `--warm-400` | `#B5AFA5` | Placeholder text |
| `--warm-500` | `#8A8279` | Secondary text, metadata |
| `--warm-600` | `#6B6359` | Tertiary text |
| `--warm-700` | `#4D463E` | Body text (light mode) |
| `--warm-800` | `#2D2825` | Strong secondary text |
| `--warm-900` | `#1F1915` | Primary text, maximum emphasis |

### Dark Theme

| Token | Hex | Role |
|-------|-----|------|
| `--dark-bg` | `#1A1816` | Page background |
| `--dark-surface` | `#242220` | Elevated surfaces |
| `--dark-surface-hover` | `#2E2C29` | Hover states |
| `--dark-card` | `#1F1D1B` | Card backgrounds |
| `--dark-border` | `#3A3634` | Borders, dividers |
| `--dark-text-primary` | `#F5F3EF` | Primary text |
| `--dark-text-secondary` | `#B5AFA5` | Secondary text |
| `--dark-text-tertiary` | `#8A8279` | Tertiary text |

### Claude Chat Interface Colors

| Token | Hex | Role |
|-------|-----|------|
| `--chat-bg-light` | `#FAF9F5` | Conversation background (light) |
| `--chat-user-bg` | `#FFFFFE` | User message background |
| `--chat-assistant-bg` | `#F5F3ED` | Claude message background (light) |
| `--chat-input-bg` | `#FFFFFE` | Input area background |
| `--claude-avatar` | `#DA7756` | Claude avatar accent |
| `--user-avatar` | `#4D463E` | User avatar default |

### Semantic Colors

| Token | Hex | Role |
|-------|-----|------|
| `--error-red` | `#D84C4C` | Errors, destructive actions |
| `--error-bg` | `#FDF2F2` | Error backgrounds |
| `--warning-amber` | `#D4883A` | Warnings, caution states |
| `--warning-bg` | `#FDF8F0` | Warning backgrounds |
| `--success-green` | `#3D8B6E` | Success, confirmation |
| `--success-bg` | `#F0F7F4` | Success backgrounds |
| `--info-blue` | `#4A7FB5` | Information, links |
| `--info-bg` | `#F0F5FA` | Info backgrounds |

### Documentation & Code Colors

| Token | Hex | Role |
|-------|-----|------|
| `--code-purple` | `#8B5CF6` | API endpoints, keywords |
| `--code-blue` | `#3B82F6` | Method names, attributes |
| `--code-green` | `#059669` | Strings, success states |
| `--code-orange` | `#EA580C` | Warnings, deprecated |
| `--code-coral` | `#DA7756` | Important highlights |

---

## 3. Typography Rules

### Font Stack

```css
/* Primary UI Font - Styrene */
--font-sans: 'Styrene A', 'Styrene B', -apple-system, BlinkMacSystemFont, 
             'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;

/* Alternative Web Font - Tiempos or fallback */
--font-editorial: 'Tiempos Text', 'Georgia', 'Times New Roman', serif;

/* Monospace */
--font-mono: 'JetBrains Mono', 'SF Mono', 'Fira Code', 
             'Roboto Mono', 'Menlo', monospace;

/* Fallback System Stack */
--font-system: -apple-system, BlinkMacSystemFont, 'Segoe UI', 
               'Roboto', 'Helvetica Neue', Arial, sans-serif;
```

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing | Color |
|---------|------|--------|-------------|----------------|-------|
| Hero Display | 52px | 500 | 1.1 | -0.02em | `--warm-900` |
| Page Title | 36px | 500 | 1.2 | -0.015em | `--warm-900` |
| Section Title | 28px | 500 | 1.25 | -0.01em | `--warm-900` |
| Card Title | 22px | 500 | 1.3 | -0.005em | `--warm-800` |
| Subsection | 18px | 500 | 1.35 | 0 | `--warm-800` |
| Large Body | 17px | 400 | 1.65 | 0.005em | `--warm-700` |
| Body | 15px | 400 | 1.65 | 0.005em | `--warm-700` |
| Small Body | 14px | 400 | 1.55 | 0.005em | `--warm-600` |
| Caption | 13px | 400 | 1.45 | 0.01em | `--warm-500` |
| Label | 12px | 500 | 1.4 | 0.02em | `--warm-500` |
| Chat Message | 15px | 400 | 1.7 | 0.005em | `--warm-800` |
| Code Inline | 14px | 400 | 1.6 | 0 | `--code-coral` |
| Code Block | 13px | 400 | 1.6 | 0 | `--warm-800` |

### Font Weights

| Weight | Name | Usage |
|--------|------|-------|
| 400 | Regular | Body text, chat messages, descriptions |
| 450 | Book | Extended reading, documentation |
| 500 | Medium | Headlines, titles, buttons, emphasis |
| 600 | Semibold | Strong emphasis, critical UI |

### Typography Philosophy
Anthropic's typography embodies **editorial warmth with technical precision**. The Styrene typeface provides a distinctive, modern yet approachable feel—geometric foundations softened with humanist details. Headlines use subtle negative tracking for refinement, while body text employs slight positive tracking for enhanced readability during extended conversations.

```css
/* Letter spacing scale */
--tracking-tight: -0.02em;   /* Hero headlines */
--tracking-snug: -0.01em;    /* Section titles */
--tracking-normal: 0;        /* Buttons, labels */
--tracking-relaxed: 0.005em; /* Body text */
--tracking-wide: 0.02em;     /* Small caps, labels */
```

### Monospace Typography

| Element | Size | Weight | Usage |
|---------|------|--------|-------|
| Code Block | 13px | 400 | Multi-line code, API examples |
| Inline Code | 13px | 400 | Technical terms, parameters |
| Terminal | 13px | 400 | CLI commands |
| API Endpoint | 14px | 500 | API documentation |

---

## 4. Component Stylings

### Buttons

#### Primary Button (Coral)
```css
.button-primary {
  background: #C4553D;
  color: #ffffff;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 18px;
  height: 40px;
  border-radius: 8px;
  border: none;
  letter-spacing: 0.005em;
  transition: all 150ms ease;
}

.button-primary:hover {
  background: #DA7756;
}

.button-primary:active {
  background: #B34A35;
}

.button-primary:focus-visible {
  outline: none;
  box-shadow: 0 0 0 2px #FAF9F5,
              0 0 0 4px #DA7756;
}

.button-primary:disabled {
  background: #DDD9D1;
  color: #8A8279;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.button-secondary {
  background: transparent;
  color: #1F1915;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 18px;
  height: 40px;
  border-radius: 8px;
  border: 1px solid #DDD9D1;
  transition: all 150ms ease;
}

.button-secondary:hover {
  background: #F5F3EF;
  border-color: #B5AFA5;
}

.button-secondary:active {
  background: #EBE8E2;
}
```

#### Ghost Button
```css
.button-ghost {
  background: transparent;
  color: #6B6359;
  font-size: 14px;
  font-weight: 500;
  padding: 8px 14px;
  height: 36px;
  border-radius: 6px;
  border: none;
}

.button-ghost:hover {
  background: #F5F3EF;
  color: #1F1915;
}
```

#### Dark Mode Button
```css
.button-dark-primary {
  background: #DA7756;
  color: #1F1915;
}

.button-dark-primary:hover {
  background: #E88B6A;
}

.button-dark-secondary {
  background: transparent;
  color: #F5F3EF;
  border: 1px solid #3A3634;
}

.button-dark-secondary:hover {
  background: #2E2C29;
}
```

#### Button Sizes

| Size | Height | Padding | Font Size |
|------|--------|---------|-----------|
| Small | 32px | 8px 14px | 13px |
| Medium (default) | 40px | 10px 18px | 14px |
| Large | 48px | 12px 24px | 15px |

### Inputs

#### Text Input
```css
.input {
  background: #FFFFFE;
  color: #1F1915;
  font-size: 15px;
  font-family: var(--font-sans);
  padding: 10px 14px;
  height: 44px;
  border-radius: 8px;
  border: 1px solid #DDD9D1;
  transition: all 150ms ease;
  width: 100%;
}

.input:hover {
  border-color: #B5AFA5;
}

.input:focus {
  outline: none;
  border-color: #DA7756;
  box-shadow: 0 0 0 3px rgba(218, 119, 86, 0.12);
}

.input::placeholder {
  color: #B5AFA5;
}

.input:disabled {
  background: #F5F3EF;
  color: #8A8279;
  cursor: not-allowed;
}

.input-error {
  border-color: #D84C4C;
}

.input-error:focus {
  box-shadow: 0 0 0 3px rgba(216, 76, 76, 0.12);
}
```

#### Claude Chat Input
```css
.chat-input {
  background: #FFFFFE;
  color: #1F1915;
  font-size: 15px;
  line-height: 1.5;
  padding: 14px 48px 14px 16px;
  border-radius: 12px;
  border: 1px solid #DDD9D1;
  min-height: 52px;
  max-height: 200px;
  resize: none;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.04);
}

.chat-input:focus {
  outline: none;
  border-color: #DA7756;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.04),
              0 0 0 3px rgba(218, 119, 86, 0.12);
}

.chat-input::placeholder {
  color: #B5AFA5;
}
```

### Cards

#### Standard Card
```css
.card {
  background: #FFFFFE;
  border-radius: 12px;
  padding: 24px;
  border: 1px solid #EBE8E2;
  transition: all 200ms ease;
}

.card:hover {
  border-color: #DDD9D1;
  box-shadow: 0 4px 12px rgba(31, 25, 21, 0.06);
}
```

#### Feature Card
```css
.card-feature {
  background: #FFFFFE;
  border-radius: 16px;
  padding: 28px;
  border: 1px solid #EBE8E2;
}

.card-feature-icon {
  width: 44px;
  height: 44px;
  background: #F5DDD4;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
}

.card-feature-icon svg {
  color: #C4553D;
  width: 22px;
  height: 22px;
}
```

#### Research Card (Academic)
```css
.card-research {
  background: #FFFFFE;
  border-radius: 8px;
  padding: 24px 28px;
  border: 1px solid #EBE8E2;
  border-left: 3px solid #DA7756;
}

.card-research-category {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: #DA7756;
  margin-bottom: 8px;
}

.card-research-title {
  font-size: 18px;
  font-weight: 500;
  color: #1F1915;
  line-height: 1.35;
  margin-bottom: 12px;
}
```

### Chat Messages

#### User Message
```css
.message-user {
  background: #FFFFFE;
  border-radius: 16px;
  padding: 16px 20px;
  margin: 12px 0;
  max-width: 75%;
  margin-left: auto;
  border: 1px solid #EBE8E2;
}

.message-user-text {
  font-size: 15px;
  line-height: 1.65;
  color: #1F1915;
}
```

#### Claude Message
```css
.message-claude {
  background: #F5F3ED;
  border-radius: 16px;
  padding: 20px 24px;
  margin: 12px 0;
  max-width: 85%;
}

.message-claude-avatar {
  width: 28px;
  height: 28px;
  background: #DA7756;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 12px;
}

.message-claude-avatar svg {
  color: #FFFFFE;
  width: 16px;
  height: 16px;
}

.message-claude-content {
  font-size: 15px;
  line-height: 1.7;
  color: #2D2825;
}

/* Dark mode Claude message */
.message-claude-dark {
  background: #242220;
  color: #F5F3EF;
}
```

### Navigation

#### Top Navigation
```css
.nav-header {
  height: 60px;
  background: #FAF9F5;
  border-bottom: 1px solid #EBE8E2;
  display: flex;
  align-items: center;
  padding: 0 24px;
}

.nav-logo {
  font-size: 18px;
  font-weight: 500;
  color: #1F1915;
  letter-spacing: -0.01em;
}

.nav-logo-claude {
  color: #DA7756;
  font-weight: 500;
}

.nav-item {
  font-size: 14px;
  font-weight: 450;
  color: #6B6359;
  padding: 8px 14px;
  border-radius: 6px;
  transition: all 150ms ease;
}

.nav-item:hover {
  color: #1F1915;
  background: #F5F3EF;
}

.nav-item-active {
  color: #1F1915;
}
```

#### Sidebar Navigation
```css
.sidebar {
  width: 280px;
  background: #FFFFFE;
  padding: 16px 12px;
  border-right: 1px solid #EBE8E2;
  display: flex;
  flex-direction: column;
  height: 100vh;
}

.sidebar-new-chat {
  background: #C4553D;
  border-radius: 10px;
  padding: 12px 16px;
  color: #FFFFFE;
  font-size: 14px;
  font-weight: 500;
  display: flex;
  align-items: center;
  gap: 10px;
  cursor: pointer;
  transition: background 150ms ease;
  margin-bottom: 16px;
}

.sidebar-new-chat:hover {
  background: #DA7756;
}

.sidebar-section-label {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #8A8279;
  padding: 8px 12px;
  margin-top: 8px;
}
```

### Code Blocks

```css
.code-block {
  background: #1F1D1B;
  border-radius: 10px;
  overflow: hidden;
  font-family: var(--font-mono);
  font-size: 13px;
  line-height: 1.6;
}

.code-block-header {
  background: #2A2826;
  padding: 10px 16px;
  font-size: 12px;
  font-weight: 500;
  color: #B5AFA5;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #3A3634;
}

.code-block-body {
  padding: 16px;
  overflow-x: auto;
  color: #F5F3EF;
}

.code-inline {
  background: #F5DDD4;
  padding: 2px 6px;
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #C4553D;
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

.badge-coral {
  background: #F5DDD4;
  color: #C4553D;
}

.badge-success {
  background: #E3F1EA;
  color: #2D7A5E;
}

.badge-warning {
  background: #FDF3E4;
  color: #B87320;
}

.badge-error {
  background: #FDE8E8;
  color: #C43C3C;
}

.badge-neutral {
  background: #F5F3EF;
  color: #6B6359;
}

.badge-safety {
  background: #E8F4F0;
  color: #2D7A5E;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.02em;
}
```

### Tooltips

```css
.tooltip {
  background: #1F1915;
  color: #F5F3EF;
  font-size: 13px;
  font-weight: 400;
  padding: 8px 12px;
  border-radius: 8px;
  box-shadow: 0 4px 16px rgba(31, 25, 21, 0.2);
  max-width: 260px;
  line-height: 1.45;
}

.tooltip-arrow {
  fill: #1F1915;
}
```

### Modals

```css
.modal-overlay {
  background: rgba(31, 25, 21, 0.5);
  backdrop-filter: blur(4px);
}

.modal {
  background: #FFFFFE;
  border-radius: 16px;
  box-shadow: 0 24px 48px rgba(31, 25, 21, 0.18);
  max-width: 480px;
  width: 100%;
  overflow: hidden;
}

.modal-header {
  padding: 24px 24px 0;
}

.modal-title {
  font-size: 20px;
  font-weight: 500;
  color: #1F1915;
}

.modal-body {
  padding: 16px 24px 24px;
}

.modal-footer {
  padding: 16px 24px;
  background: #FAF9F5;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
  border-top: 1px solid #EBE8E2;
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

#### Claude Chat Interface
```
┌────────────────────────────────────────────────────────────────────┐
│  ┌───────────┬────────────────────────────────────────────────┐   │
│  │           │                                                 │   │
│  │  Sidebar  │              Conversation Area                  │   │
│  │  (280px)  │              (#FAF9F5 background)              │   │
│  │           │     ┌────────────────────────────────────┐     │   │
│  │  History  │     │       Message Thread                │     │   │
│  │  List     │     │       (max-width: 720px)           │     │   │
│  │           │     │       (centered)                    │     │   │
│  │           │     └────────────────────────────────────┘     │   │
│  │           │                                                 │   │
│  │           │     ┌────────────────────────────────────┐     │   │
│  │           │     │    Composer Input Area              │     │   │
│  │           │     │    (fixed bottom, cream bg)        │     │   │
│  │           │     └────────────────────────────────────┘     │   │
│  └───────────┴────────────────────────────────────────────────┘   │
└────────────────────────────────────────────────────────────────────┘
```

#### Documentation Layout
```
┌────────────────────────────────────────────────────────────────────┐
│  ┌─────────────────────────────────────────────────────────────┐  │
│  │                    Top Navigation (60px)                     │  │
│  │  Anthropic    Research    Claude    API    Documentation     │  │
│  └─────────────────────────────────────────────────────────────┘  │
│                                                                    │
│  ┌───────────┬──────────────────────────────────────────────┐     │
│  │           │                                               │     │
│  │  Sidebar  │             Content Area                      │     │
│  │  (260px)  │             (max: 720px)                     │     │
│  │           │                                               │     │
│  │  Section  │    Editorial-style typography                 │     │
│  │  Nav      │    and academic spacing                       │     │
│  │           │                                               │     │
│  └───────────┴──────────────────────────────────────────────┘     │
└────────────────────────────────────────────────────────────────────┘
```

### Content Widths

| Context | Max Width | Centering |
|---------|-----------|-----------|
| Chat Messages | 720px | Centered |
| Documentation | 720px | Centered |
| Landing Page Content | 1120px | Centered |
| API Reference | 100% | Split layout |
| Settings/Forms | 520px | Left-aligned |
| Modal Content | 480px | Centered |

### Grid System

```css
/* Feature Grid */
.grid-features {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

/* Research Grid */
.grid-research {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 24px;
}

/* Documentation Grid */
.grid-docs {
  display: grid;
  grid-template-columns: 260px 1fr;
  gap: 48px;
}
```

### Whitespace Philosophy
Anthropic uses whitespace to create **focus and contemplation**. The Claude interface encourages thoughtful interaction with generous line heights and message spacing, while documentation follows academic journal conventions with generous margins, clear section demarcation, and breathing room that supports deep reading.

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
  box-shadow: 0 1px 2px rgba(31, 25, 21, 0.04);
}

/* Level 2 - Card default */
.shadow-md {
  box-shadow: 0 2px 8px rgba(31, 25, 21, 0.06);
}

/* Level 3 - Elevated card */
.shadow-lg {
  box-shadow: 0 4px 12px rgba(31, 25, 21, 0.08);
}

/* Level 4 - Dropdown/Popover */
.shadow-xl {
  box-shadow: 0 8px 24px rgba(31, 25, 21, 0.1);
}

/* Level 5 - Modal */
.shadow-2xl {
  box-shadow: 0 24px 48px rgba(31, 25, 21, 0.18);
}
```

### Border System

```css
/* Light theme borders */
--border-light: 1px solid #EBE8E2;
--border-light-subtle: 1px solid #F5F3EF;
--border-light-strong: 1px solid #DDD9D1;

/* Dark theme borders */
--border-dark: 1px solid #3A3634;
--border-dark-subtle: 1px solid #2E2C29;
--border-dark-strong: 1px solid #4A4644;

/* Focus border */
--border-focus: 1px solid #DA7756;

/* Accent border (research/editorial) */
--border-accent: 3px solid #DA7756;
```

### Surface Hierarchy (Light Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Modal (Elevated)                    #FFFFFE + shadow-2xl │
├─────────────────────────────────────────────────────────┤
│ Dropdown/Popover                    #FFFFFE + shadow-xl  │
├─────────────────────────────────────────────────────────┤
│ Cards (Hover)                       #FFFFFE + shadow-lg  │
├─────────────────────────────────────────────────────────┤
│ Cards (Default)                     #FFFFFE + border     │
├─────────────────────────────────────────────────────────┤
│ Subtle Surface                      #F5F3ED              │
├─────────────────────────────────────────────────────────┤
│ Page Background                     #FAF9F5              │
└─────────────────────────────────────────────────────────┘
```

### Surface Hierarchy (Dark Theme)

```
┌─────────────────────────────────────────────────────────┐
│ Modal (Elevated)                    #2E2C29 + shadow     │
├─────────────────────────────────────────────────────────┤
│ Dropdown/Popover                    #242220 + shadow     │
├─────────────────────────────────────────────────────────┤
│ Cards                               #1F1D1B + border     │
├─────────────────────────────────────────────────────────┤
│ Input Area                          #242220              │
├─────────────────────────────────────────────────────────┤
│ Page Background                     #1A1816              │
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
| Use warm cream (#FAF9F5) as primary background | Brand distinction, warmth, eye comfort |
| Apply coral (#DA7756) sparingly for emphasis | Maintains warmth without overwhelming |
| Use generous line-height (1.65-1.7) for text | Enhanced readability, editorial quality |
| Keep message containers centered and constrained | Optimal reading width, focused experience |
| Use subtle rounded corners (8-12px) | Approachable without being playful |
| Implement warm gray tones throughout | Cohesive visual language, softened contrast |
| Show Claude attribution clearly | Transparency about AI interaction |
| Use subtle borders over heavy shadows | Clean, academic aesthetic |
| Apply consistent warm color temperature | Brand coherence across all elements |
| Provide safety-focused messaging patterns | Core to Anthropic's mission and values |

### Don'ts

| Anti-Pattern | Why to Avoid |
|--------------|--------------|
| Never use pure white (#FFFFFF) as page background | Contradicts warm aesthetic, appears clinical |
| Avoid cool-toned grays | Breaks warm color harmony |
| Don't use multiple bright accent colors | Coral is the singular brand accent |
| Never hide safety-related information | Transparency is core to trust |
| Avoid aggressive animations | Thoughtful, calm environment |
| Don't use overly small text for messages | Readability is paramount |
| Never auto-submit without user review | Respect for deliberate interaction |
| Avoid pure black (#000000) text | Use warm dark gray for softer contrast |
| Don't use heavy shadows for primary UI | Flat, editorial aesthetic preferred |
| Never create urgent/aggressive UI patterns | Counter to safety-focused brand |

### Content Guidelines

| Do | Don't |
|----|-------|
| Use thoughtful, considered AI responses | Provide instant, unconsidered answers |
| Acknowledge limitations honestly | Assert false certainty |
| Show examples with context | Provide abstract explanations only |
| Indicate when Claude is uncertain | Pretend omniscience |
| Use consistent model naming (Claude, Sonnet, etc.) | Use internal codenames |
| Explain capabilities and limitations clearly | Overpromise functionality |
| Reflect safety values in UI copy | Ignore safety considerations |
| Use warm, conversational tone | Be cold or robotic |

---

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Behavior |
|------|-------|----------|
| Mobile | <640px | Full-width chat, collapsible sidebar |
| Tablet | 640px - 1024px | Overlay sidebar, centered content |
| Desktop | 1024px - 1440px | Full layout, persistent sidebar |
| Wide | >1440px | Maximum content width, centered |

### Mobile Adaptations

| Component | Desktop | Mobile |
|-----------|---------|--------|
| Sidebar | Persistent 280px | Full-screen overlay |
| Chat Messages | 720px max-width | Full width with 16px padding |
| Navigation | Full items | Hamburger menu |
| Input Area | Single row expandable | Full width, larger touch targets |
| Code Blocks | Horizontal scroll | Horizontal scroll, smaller text |
| Modal | Centered 480px | Full screen or bottom sheet |

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
| Hero Display | 52px | 32px |
| Page Title | 36px | 26px |
| Section Title | 28px | 22px |
| Chat Message | 15px | 15px |
| Body | 15px | 15px |
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
    width: 100%;
    transform: translateX(-100%);
    background: #FFFFFE;
  }
  
  .sidebar-open {
    transform: translateX(0);
  }
  
  .message-claude {
    max-width: 95%;
  }
}

/* Tablet: Overlay sidebar */
@media (min-width: 640px) and (max-width: 1024px) {
  .sidebar {
    position: fixed;
    z-index: 250;
    width: 300px;
  }
  
  .chat-container {
    max-width: 640px;
  }
}

/* Desktop: Persistent sidebar */
@media (min-width: 1024px) {
  .sidebar {
    position: relative;
    flex-shrink: 0;
  }
  
  .chat-container {
    max-width: 720px;
  }
}
```

---

## 9. Agent Prompt Guide

### Quick Reference

```yaml
# Brand Colors
Primary Coral: #DA7756
Terracotta: #C4553D
Coral Light: #F5DDD4
Coral Hover: #E88B6A

# Light Mode
Background: #FAF9F5
Surface: #FFFFFE
Surface Alt: #F5F3ED
Border: #EBE8E2
Text Primary: #1F1915
Text Secondary: #6B6359
Text Tertiary: #8A8279

# Dark Mode
Background: #1A1816
Surface: #242220
Card: #1F1D1B
Border: #3A3634
Text Primary: #F5F3EF
Text Secondary: #B5AFA5

# Typography
Font Primary: 'Styrene A', system-ui, sans-serif
Font Mono: 'JetBrains Mono', monospace
Body Line Height: 1.65
Chat Line Height: 1.7

# Radii
Small: 6px
Medium: 8px
Large: 12px
XL: 16px

# Focus
Focus Ring: 0 0 0 2px #FAF9F5, 0 0 0 4px #DA7756
Focus Shadow: 0 0 0 3px rgba(218, 119, 86, 0.12)
```

### Example Prompts

#### Claude Message Component
```
Create a Claude-style message using Anthropic's design system:
- Container: max-width 720px, centered, padding 20px 24px
- Background: #F5F3ED (Claude messages), 16px border-radius
- User message: #FFFFFE background with 1px #EBE8E2 border
- Claude avatar: 28px square, #DA7756 background, 8px radius
- Message text: 15px Styrene, line-height 1.7, #2D2825
- Page background: #FAF9F5 (warm cream)
- Spacing between messages: 12px
- Warm, editorial feel throughout
```

#### Claude Chat Input
```
Design the Claude chat input component:
- Container: bottom of screen, #FAF9F5 background
- Inner wrapper: max-width 720px, centered
- Input: #FFFFFE background, 12px border-radius
- Border: 1px solid #DDD9D1, subtle shadow
- Focus: coral border #DA7756 with soft coral glow
- Placeholder: "Message Claude..." in #B5AFA5
- Send button: 40px circle, #C4553D when active
- Disabled send: #DDD9D1
- Font: 15px Styrene, #1F1915
- Min-height: 52px, max-height: 200px (expandable)
```

#### Research/Documentation Page
```
Create a research page in Anthropic's editorial style:
- Background: #FAF9F5 (warm cream)
- Content max-width: 720px, generous margins
- Heading hierarchy: 28px/22px/18px, weight 500
- Body: 15px, line-height 1.65, #4D463E
- Left accent border: 3px solid #DA7756 for callouts
- Code blocks: #1F1D1B dark background
- Inline code: #F5DDD4 bg, #C4553D text
- Links: #C4553D, underline on hover
- Research card: white bg, coral left border
- Academic, journal-like atmosphere
```

#### Safety Callout
```
Design a safety-focused callout component:
- Background: #E8F4F0 (soft green tint)
- Border-left: 3px solid #3D8B6E
- Padding: 16px 20px
- Icon: Shield or similar, #3D8B6E
- Title: 14px weight 500, #2D7A5E
- Body: 14px weight 400, #4D463E
- Border-radius: 8px
- Conveys trust and responsibility
```

#### Settings Modal
```
Create a settings modal for Claude:
- Overlay: rgba(31, 25, 21, 0.5) with backdrop blur
- Modal: #FFFFFE background, 16px border-radius
- Width: 480px max
- Header: 24px padding, "Settings" in 20px weight 500 #1F1915
- Sections: clear dividers with #EBE8E2
- Toggle switches: 40px wide, #DA7756 when active
- Footer: #FAF9F5 background, 1px top border
- Close button: ghost style, top right
- Save button: #C4553D primary style
```

### CSS Variables Template

```css
:root {
  /* Core Brand Colors */
  --anthropic-coral: #DA7756;
  --anthropic-terracotta: #C4553D;
  --anthropic-coral-light: #F5DDD4;
  --anthropic-coral-hover: #E88B6A;
  
  /* Light Theme */
  --bg-primary: #FAF9F5;
  --bg-surface: #FFFFFE;
  --bg-surface-alt: #F5F3ED;
  --text-primary: #1F1915;
  --text-secondary: #6B6359;
  --text-tertiary: #8A8279;
  --border-color: #EBE8E2;
  --border-strong: #DDD9D1;
  
  /* Typography */
  --font-sans: 'Styrene A', 'Styrene B', -apple-system, sans-serif;
  --font-mono: 'JetBrains Mono', 'SF Mono', monospace;
  
  /* Tracking */
  --tracking-tight: -0.02em;
  --tracking-snug: -0.01em;
  --tracking-normal: 0;
  --tracking-relaxed: 0.005em;
  
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
  
  /* Shadows (warm tinted) */
  --shadow-sm: 0 1px 2px rgba(31, 25, 21, 0.04);
  --shadow-md: 0 2px 8px rgba(31, 25, 21, 0.06);
  --shadow-lg: 0 4px 12px rgba(31, 25, 21, 0.08);
  --shadow-xl: 0 8px 24px rgba(31, 25, 21, 0.1);
  --shadow-2xl: 0 24px 48px rgba(31, 25, 21, 0.18);
  
  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
}

/* Dark Theme */
[data-theme="dark"] {
  --bg-primary: #1A1816;
  --bg-surface: #242220;
  --bg-surface-alt: #1F1D1B;
  
  --text-primary: #F5F3EF;
  --text-secondary: #B5AFA5;
  --text-tertiary: #8A8279;
  
  --border-color: #3A3634;
  --border-strong: #4A4644;
}
```

---

## Summary

Anthropic's design system embodies **editorial warmth with safety-conscious intelligence** through:

1. **Warm cream foundation** (#FAF9F5) distinguishing from cold, clinical AI interfaces
2. **Terracotta/coral accent** (#DA7756, #C4553D) as singular warm brand color
3. **Styrene typeface** with generous line-heights (1.65-1.7) for thoughtful reading
4. **Warm gray palette** (#1F1915 to #F5F3EF) maintaining color temperature harmony
5. **Subtle rounded corners** (8-12px) creating approachable, non-aggressive UI
6. **Minimal shadows, border-focused** depth for clean academic aesthetic
7. **Centered, constrained content** (720px max) for optimal reading experience
8. **Research paper influence** in documentation and editorial layouts

When implementing Anthropic/Claude-style interfaces, prioritize:
- Warm color temperature throughout (no pure whites or cool grays)
- Editorial, journal-like typography and spacing
- Thoughtful, considered interaction patterns
- Clear Claude/AI attribution and transparency
- Safety-conscious messaging and UI patterns
- Minimal chrome, content-first approach
- Conversational warmth in both visual design and copy
- Trust-building through honest, approachable design
