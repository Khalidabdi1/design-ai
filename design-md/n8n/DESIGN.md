# n8n Design System
> Open-source workflow automation platform with a dark canvas aesthetic — deep gray surfaces, orange node accents, and workflow-graph-first UI.

---

## 1. Visual Theme & Atmosphere
n8n is a visual workflow builder that runs like a developer tool. The canvas dominates the interface — a dark infinite grid where nodes connect into powerful automations. The orange brand accent signals action and energy: trigger nodes, active connections, and run status. The overall aesthetic is dark and technical, balancing the visual complexity of a node graph with enough structure to stay approachable.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#FF6D5A` | Brand orange-red, trigger nodes, CTAs |
| `--color-primary-dark` | `#E05540` | Hover/active |
| `--color-primary-light` | `#FFF0EE` | Light badges (light mode only) |
| `--color-node-trigger` | `#FF6D5A` | Trigger node color |
| `--color-node-action` | `#5C9DF5` | Action/integration node color |
| `--color-node-success` | `#26BD73` | Execution success glow |
| `--color-node-error` | `#F55C5C` | Execution error glow |
| `--color-edge` | `#5C9DF5` | Connection edge lines |
| `--color-canvas-bg` | `#1B1F23` | Canvas background |
| `--color-canvas-grid` | `rgba(255,255,255,0.04)` | Dot grid on canvas |
| `--color-bg-base` | `#121417` | App background |
| `--color-bg-panel` | `#1E2227` | Side panel, properties |
| `--color-bg-node` | `#282E36` | Node body |
| `--color-border` | `#363D47` | Default borders |
| `--color-text-primary` | `#F0F2F5` | Headings, primary text |
| `--color-text-secondary` | `#8B909A` | Labels, secondary |
| `--color-text-muted` | `#525861` | Placeholders |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 11px;
--font-size-sm: 12px;
--font-size-base: 14px;
--font-size-md: 16px;
--font-size-lg: 20px;
--font-size-xl: 24px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 20px | 600 | 1.3 |
| Node Name | 13px | 600 | 1.4 |
| Node Description | 12px | 400 | 1.4 |
| Panel Label | 12px | 500 | 1.4 |
| Body | 14px | 400 | 1.5 |
| Code / Expression | 13px | 400 | 1.6 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #FF6D5A;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.12s;
}
.button-primary:hover { background: #E05540; }

/* Workflow Node */
.node {
  background: #282E36;
  border: 1.5px solid #363D47;
  border-radius: 8px;
  padding: 0;
  width: 100px;
  min-height: 80px;
  display: flex;
  flex-direction: column;
  align-items: center;
  cursor: pointer;
  position: relative;
  transition: border-color 0.12s;
}
.node:hover { border-color: #5C9DF5; }
.node--selected { border-color: #5C9DF5; box-shadow: 0 0 0 2px rgba(92,157,245,0.25); }
.node--trigger { border-color: #FF6D5A; }
.node__icon {
  width: 48px;
  height: 48px;
  border-radius: 8px;
  margin: 12px auto 6px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.node__name {
  font-size: 11px;
  font-weight: 600;
  color: #F0F2F5;
  text-align: center;
  padding: 0 8px 12px;
}

/* Connection Port */
.node__port {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: #363D47;
  border: 2px solid #8B909A;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  cursor: crosshair;
}
.node__port--right { right: -7px; }
.node__port--left { left: -7px; }
.node__port:hover { border-color: #5C9DF5; background: #5C9DF5; }

/* Execution Badge */
.exec-badge {
  position: absolute;
  top: -8px;
  right: -8px;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 10px;
  font-weight: 700;
  color: #FFFFFF;
}
.exec-badge--success { background: #26BD73; }
.exec-badge--error { background: #F55C5C; }

/* Property Panel Input */
.panel-input {
  background: #1B1F23;
  border: 1px solid #363D47;
  border-radius: 6px;
  padding: 8px 12px;
  font-size: 13px;
  color: #F0F2F5;
  width: 100%;
  transition: border-color 0.12s;
}
.panel-input:focus {
  outline: none;
  border-color: #5C9DF5;
  box-shadow: 0 0 0 2px rgba(92,157,245,0.15);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--node-width` | `100px` | Standard node width |
| `--node-min-height` | `80px` | Minimum node height |
| `--edge-width` | `2px` | Connection line width |
| `--spacing-xs` | `4px` | Port offsets |
| `--spacing-sm` | `8px` | Node inner padding |
| `--spacing-md` | `16px` | Panel section gaps |
| `--spacing-lg` | `24px` | Panel padding |
| `--panel-width` | `320px` | Properties side panel |
| `--radius-md` | `6px` | Buttons, inputs |
| `--radius-lg` | `8px` | Nodes |

## 6. Depth & Elevation
```css
.shadow-node { box-shadow: 0 4px 12px rgba(0,0,0,0.4); }
.shadow-node-selected { box-shadow: 0 0 0 2px rgba(92,157,245,0.25), 0 4px 12px rgba(0,0,0,0.4); }
.shadow-panel { box-shadow: -4px 0 16px rgba(0,0,0,0.4); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.6); }
```

## 7. Do's and Don'ts
**Do:**
- Use orange for trigger/start nodes and blue for action/integration nodes
- Show execution success/error as small overlay badges on the node corner
- Connection ports should be visually discoverable on hover
- Keep node labels to 2 lines max — icon conveys the integration type

**Don't:**
- Don't use a white or light canvas — the dark grid is essential for contrast
- Don't use more than 2 distinct node colors in the same workflow view
- Don't add excessive chrome to nodes — the icon and name should dominate

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Read-only workflow view; editing disabled |
| Tablet | 768px | Canvas with minimal controls; panel as modal |
| Desktop | 1024px | Full canvas + right properties panel |
| Wide | 1440px | Wider canvas area; panel fixed at 320px |

## 9. Agent Prompt Guide
```
You are designing for n8n — an open-source workflow automation platform.
The canvas is the hero: dark background (#1B1F23) with a subtle dot grid overlay.
Nodes are small rounded cards (100px wide) with a service icon and a short label.
Trigger nodes use orange (#FF6D5A) borders; action nodes use blue (#5C9DF5).
Connection edges are curved blue lines between node ports.
Execution status appears as small circular badges (green=success, red=error) on the node.
The right panel is for node properties: dark, compact, monospace expressions.
Tone is visual, workflow-centric, and automation-builder-focused.
```
