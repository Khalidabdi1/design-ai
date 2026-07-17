# Hoppscotch Design System
> Open-source API development platform with a vibrant dark aesthetic — deep surfaces, electric green brand accent, and request-testing-first UI.

---

## 1. Visual Theme & Atmosphere
Hoppscotch is a fast, free, and open-source alternative to Postman. The interface is dark and streamlined with an electric green accent that signals "go" — run requests, execute tests, watch responses. The layout is split into a request builder and a response viewer, with a sidebar of saved collections. The design prioritizes speed and visual density, echoing the terminal-adjacent aesthetics of developer tools while staying approachable and colorful.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#00BFA5` | Brand teal-green, CTAs, active states |
| `--color-primary-dark` | `#00897B` | Hover/active |
| `--color-primary-dim` | `rgba(0,191,165,0.12)` | Highlight backgrounds |
| `--color-bg-base` | `#171823` | App background |
| `--color-bg-sidebar` | `#12131D` | Left sidebar |
| `--color-bg-card` | `#1E1F2E` | Cards, panels |
| `--color-bg-input` | `#252635` | Input, request area |
| `--color-bg-elevated` | `#282940` | Dropdowns, modals |
| `--color-border` | `#2D2F45` | Default borders |
| `--color-text-primary` | `#E0E0F0` | Headings, primary text |
| `--color-text-secondary` | `#7878A0` | Labels, meta |
| `--color-text-muted` | `#454568` | Placeholders, disabled |
| `--color-method-get` | `#61AFEF` | GET method |
| `--color-method-post` | `#98C379` | POST method |
| `--color-method-put` | `#E5C07B` | PUT method |
| `--color-method-delete` | `#E06C75` | DELETE method |
| `--color-method-patch` | `#C678DD` | PATCH method |
| `--color-success` | `#00BFA5` | 2xx responses |
| `--color-error` | `#E06C75` | 4xx/5xx responses |
| `--color-warning` | `#E5C07B` | 3xx responses |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 10px;
--font-size-sm: 12px;
--font-size-base: 13px;
--font-size-md: 14px;
--font-size-lg: 16px;
--font-size-xl: 20px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.3;
--line-height-base: 1.5;
--line-height-code: 1.65;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Section Header | 14px | 600 | 1.4 |
| Request URL | 13px | 400 | 1.5 |
| Label | 12px | 500 | 1.4 |
| Code / JSON | 12px | 400 | 1.65 |
| Status Code | 13px | 700 | 1.3 |
| Tab Label | 12px | 500 | 1.4 |

## 4. Component Stylings
```css
/* Method + URL Bar */
.request-bar {
  display: flex;
  gap: 8px;
  align-items: center;
  background: #252635;
  border: 1px solid #2D2F45;
  border-radius: 8px;
  padding: 0 8px 0 0;
  overflow: hidden;
}
.method-select {
  padding: 10px 14px;
  font-size: 12px;
  font-weight: 700;
  font-family: var(--font-mono);
  border: none;
  background: transparent;
  cursor: pointer;
  letter-spacing: 0.04em;
}
.method-select--GET { color: #61AFEF; }
.method-select--POST { color: #98C379; }
.method-select--PUT { color: #E5C07B; }
.method-select--DELETE { color: #E06C75; }
.method-select--PATCH { color: #C678DD; }
.url-input {
  flex: 1;
  background: transparent;
  border: none;
  padding: 10px 0;
  font-size: 13px;
  color: #E0E0F0;
  font-family: var(--font-mono);
}
.url-input:focus { outline: none; }
.send-button {
  background: #00BFA5;
  color: #171823;
  border: none;
  border-radius: 6px;
  padding: 8px 18px;
  font-size: 13px;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.15s;
}
.send-button:hover { background: #00897B; }

/* Response Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 700;
  font-family: var(--font-mono);
}
.status-badge--2xx { background: rgba(0,191,165,0.12); color: #00BFA5; }
.status-badge--3xx { background: rgba(229,192,123,0.12); color: #E5C07B; }
.status-badge--4xx { background: rgba(224,108,117,0.12); color: #E06C75; }
.status-badge--5xx { background: rgba(224,108,117,0.15); color: #E06C75; }

/* Tab Bar */
.tab-bar {
  display: flex;
  gap: 0;
  border-bottom: 1px solid #2D2F45;
}
.tab {
  padding: 8px 16px;
  font-size: 12px;
  font-weight: 500;
  color: #7878A0;
  cursor: pointer;
  border-bottom: 2px solid transparent;
  transition: color 0.12s, border-color 0.12s;
}
.tab:hover { color: #E0E0F0; }
.tab--active { color: #00BFA5; border-bottom-color: #00BFA5; }

/* JSON Response Viewer */
.json-viewer {
  background: #12131D;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 12px;
  line-height: 1.65;
  overflow: auto;
}
.json-key { color: #61AFEF; }
.json-string { color: #98C379; }
.json-number { color: #E5C07B; }
.json-boolean { color: #C678DD; }
.json-null { color: #7878A0; }

/* Collection Sidebar Item */
.collection-item {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 6px 12px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 12px;
  color: #7878A0;
  transition: background 0.08s, color 0.08s;
}
.collection-item:hover { background: #1E1F2E; color: #E0E0F0; }
.collection-item--active { background: rgba(0,191,165,0.1); color: #00BFA5; }
.collection-item__method {
  font-size: 10px;
  font-weight: 700;
  font-family: var(--font-mono);
  letter-spacing: 0.04em;
  width: 38px;
  flex-shrink: 0;
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tab gaps |
| `--spacing-sm` | `8px` | Bar item spacing |
| `--spacing-md` | `12px` | Panel padding |
| `--spacing-lg` | `20px` | Section gaps |
| `--spacing-xl` | `28px` | Page gutter |
| `--sidebar-width` | `240px` | Collections sidebar |
| `--radius-sm` | `4px` | Small elements |
| `--radius-md` | `6px` | Buttons, badges |
| `--radius-lg` | `8px` | Panels, JSON viewer |

## 6. Depth & Elevation
```css
.shadow-panel { box-shadow: 0 2px 8px rgba(0,0,0,0.5); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.7); }
.shadow-dropdown { box-shadow: 0 8px 24px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Color-code HTTP methods: blue GET, green POST, amber PUT, red DELETE, purple PATCH
- Response status codes use color-coded pill badges (2xx green, 3xx amber, 4xx/5xx red)
- Active tab has a teal bottom border and teal text
- JSON viewer uses syntax-highlighted values

**Don't:**
- Don't use a light theme — Hoppscotch is a developer dark-mode tool
- Don't mix method colors — each HTTP verb has its own consistent color
- Don't hide the response status code — it's the most critical piece of feedback

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Tabs: request or response only |
| Tablet | 768px | Stacked: request above, response below |
| Desktop | 1024px | Side-by-side: request | response |
| Wide | 1440px | Collections + request | response |

## 9. Agent Prompt Guide
```
You are designing for Hoppscotch — open-source API development platform.
Use a deep dark background (#171823) with panel surfaces at #1E1F2E.
Teal-green (#00BFA5) is the primary brand color — the send button, active tabs, active collections.
HTTP methods are color-coded: GET (blue #61AFEF), POST (green #98C379), PUT (amber #E5C07B), DELETE (red #E06C75), PATCH (purple #C678DD).
Response status badges are pill-shaped with color-coded tinted backgrounds (2xx=teal, 3xx=amber, 4xx/5xx=red).
The JSON response viewer uses monospace font with syntax highlighting (keys in blue, strings in green).
Tone is developer-fast, open-source-friendly, dark, and API-testing-first.
```
