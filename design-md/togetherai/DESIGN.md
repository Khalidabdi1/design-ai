# Together AI Design System
> AI inference platform with a sleek dark aesthetic — deep navy-black surfaces, electric blue-purple brand gradient, and API-first developer UI.

---

## 1. Visual Theme & Atmosphere
Together AI is a high-performance inference platform for open-source AI models. The interface is built for developers who run models at scale — clean, dark, and technical. An electric blue-to-purple gradient carries the brand's forward-looking AI identity. The primary views are the model catalog, inference playground, and usage dashboard. The design is confident and precise, reflecting the platform's focus on speed, reliability, and model diversity.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#5865F2` | Brand indigo-blue, CTAs, links |
| `--color-primary-dark` | `#4350D4` | Hover/active |
| `--color-gradient` | `linear-gradient(135deg, #5865F2, #A855F7)` | Brand gradient, hero elements |
| `--color-accent` | `#A855F7` | Gradient end, secondary accent |
| `--color-bg-base` | `#09090F` | App background |
| `--color-bg-card` | `#111120` | Card, panel surfaces |
| `--color-bg-elevated` | `#191928` | Modals, dropdowns |
| `--color-bg-input` | `#141426` | Input fields |
| `--color-border` | `#252540` | Default borders |
| `--color-border-subtle` | `#1C1C33` | Subtle dividers |
| `--color-text-primary` | `#F0F0FF` | Headings, primary text |
| `--color-text-secondary` | `#8080A8` | Labels, meta |
| `--color-text-muted` | `#4A4A6A` | Placeholders, disabled |
| `--color-success` | `#22D3A0` | Active, running |
| `--color-error` | `#F87171` | Error, failed |
| `--color-token-count` | `#FBBF24` | Token/cost indicators |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
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
--line-height-tight: 1.3;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 26px | 700 | 1.25 |
| Section Header | 16px | 600 | 1.4 |
| Model Name | 14px | 600 | 1.4 |
| Body / Labels | 14px | 400 | 1.5 |
| Code / API Keys | 12px | 400 | 1.6 |
| Token Count | 12px | 500 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: linear-gradient(135deg, #5865F2, #A855F7);
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 10px 22px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: opacity 0.15s;
}
.button-primary:hover { opacity: 0.88; }

/* Model Card */
.model-card {
  background: #111120;
  border: 1px solid #252540;
  border-radius: 10px;
  padding: 18px 20px;
  cursor: pointer;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.model-card:hover {
  border-color: #5865F2;
  box-shadow: 0 0 0 1px rgba(88,101,242,0.2);
}
.model-card__tag {
  display: inline-block;
  padding: 2px 8px;
  border-radius: 4px;
  font-size: 10px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  background: rgba(88,101,242,0.15);
  color: #5865F2;
  margin-bottom: 10px;
}
.model-card__name {
  font-size: 15px;
  font-weight: 600;
  color: #F0F0FF;
  margin-bottom: 4px;
}
.model-card__meta { font-size: 12px; color: #8080A8; }
.model-card__speed {
  margin-top: 12px;
  font-size: 12px;
  color: #22D3A0;
  font-weight: 500;
}

/* Playground Chat */
.chat-container {
  background: #111120;
  border: 1px solid #252540;
  border-radius: 10px;
  overflow: hidden;
}
.chat-message {
  padding: 14px 20px;
  border-bottom: 1px solid #1C1C33;
  font-size: 14px;
  line-height: 1.6;
}
.chat-message--user { background: #141426; color: #F0F0FF; }
.chat-message--assistant { background: #111120; color: #F0F0FF; }
.chat-message__role {
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 6px;
}
.chat-message--user .chat-message__role { color: #5865F2; }
.chat-message--assistant .chat-message__role { color: #22D3A0; }

/* Token Counter */
.token-counter {
  display: flex;
  align-items: center;
  gap: 6px;
  font-size: 12px;
  color: #FBBF24;
  font-family: var(--font-mono);
  font-weight: 500;
}

/* API Key Block */
.api-key-block {
  background: #141426;
  border: 1px solid #252540;
  border-radius: 8px;
  padding: 12px 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  color: #8080A8;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.api-key-block__key { color: #F0F0FF; letter-spacing: 0.05em; }

/* Input */
.input {
  background: #141426;
  border: 1px solid #252540;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 14px;
  color: #F0F0FF;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #5865F2;
  box-shadow: 0 0 0 2px rgba(88,101,242,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight tag gaps |
| `--spacing-sm` | `8px` | Card inner spacing |
| `--spacing-md` | `16px` | Section padding |
| `--spacing-lg` | `24px` | Card padding |
| `--spacing-xl` | `40px` | Page gutter |
| `--sidebar-width` | `240px` | Left navigation |
| `--radius-sm` | `4px` | Tags, badges |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `10px` | Model cards |

## 6. Depth & Elevation
```css
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-hover { box-shadow: 0 0 0 1px rgba(88,101,242,0.2), 0 4px 16px rgba(0,0,0,0.5); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
```

## 7. Do's and Don'ts
**Do:**
- Use the gradient (blue → purple) for the primary CTA and hero brand moments
- Show model speed (tokens/sec) in green as a key metric on model cards
- Token counts appear in amber — they represent cost, so they should stand out
- Chat playground distinguishes user and assistant roles with color-coded role labels

**Don't:**
- Don't use the gradient for anything other than the primary CTA and hero sections
- Don't omit token count from the playground — it's critical context for developers
- Don't truncate model names in the catalog — show full model IDs

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Model list; playground hidden |
| Tablet | 768px | Compact sidebar + model grid |
| Desktop | 1024px | Full sidebar + catalog + playground |
| Wide | 1440px | 3-column model grid + expanded playground |

## 9. Agent Prompt Guide
```
You are designing for Together AI — AI inference platform.
Use a near-black background (#09090F) with card surfaces at #111120.
The brand gradient (indigo #5865F2 → purple #A855F7) drives the primary CTA and hero elements.
Model cards show a category tag, model name, meta (provider, context), and tokens/sec speed in green.
Chat playground distinguishes user messages (darker background, blue role label) from assistant (teal role label).
Token counts display in amber (#FBBF24) using monospace font — they signal compute cost.
Tone is developer-precise, performance-forward, and AI-native.
```
