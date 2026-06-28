# New Relic Design System

> Observability platform design with bold teal identity, full-stack telemetry surfaces, query-builder clarity, and site-reliability UX.

---

## 1. Visual Theme & Atmosphere

New Relic should feel comprehensive, intelligent, and reliable. The design language communicates APM, infrastructure monitoring, distributed tracing, logs, errors, and the unified observability data platform.

- Mood: comprehensive, reliable, intelligent, technical
- Density: high, with metrics charts, distributed trace waterfalls, log streams, and alert policies
- Character: bold teal brand, dark observability surfaces, multi-signal chart colors, NRQL query panels

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--nr-teal` | `#00AC69` | Primary brand CTA and healthy signal |
| `--nr-teal-dark` | `#008A54` | Hover and active states |
| `--nr-green` | `#01B075` | Service healthy and alert resolved |
| `--nr-critical` | `#DF2D24` | Critical alert and error spike |
| `--nr-high` | `#F86624` | High severity and degraded service |
| `--nr-medium` | `#F5C400` | Medium severity and warning |
| `--nr-low` | `#007DC3` | Low severity and informational |
| `--surface-card` | `#FFFFFF` | Metric cards and entity panels |
| `--surface-bg` | `#F4F5F7` | Dashboard background |
| `--surface-dark` | `#0E1520` | Chart canvas and dark panels |
| `--text-primary` | `#1D2433` | Primary labels and metric titles |
| `--border-default` | `#DDE0E7` | Table and panel borders |

The four-tier alert severity scale (critical/high/medium/low) must be applied consistently and never repurposed for non-alert UI states.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", "Roboto Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| Metric Value | 36px | 700 | 1.0 |
| Body | 14px | 400 | 1.6 |
| NRQL Query | 13px | 400 | 1.7 |
| Trace Label | 12px | 500 | 1.4 |
| Severity Label | 11px | 700 | 1.3 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 38px;
  padding: 0 16px;
  border: none;
  border-radius: 4px;
  background: #00AC69;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.entity-card {
  border: 1px solid #DDE0E7;
  border-radius: 8px;
  background: #FFFFFF;
  padding: 16px 20px;
}

.nrql-editor {
  border-radius: 8px;
  background: #0E1520;
  color: #C5D0E6;
  padding: 14px 18px;
  font: 400 13px/1.7 "JetBrains Mono", monospace;
  border: 1px solid #1E2A40;
}

.alert-badge {
  display: inline-flex;
  padding: 2px 8px;
  border-radius: 3px;
  font: 700 11px/1.4 Inter, sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.trace-span {
  height: 20px;
  border-radius: 3px;
  background: #00AC69;
  opacity: 0.85;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Metric row spacing |
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

Entity Explorer as the top-level navigation surface. Golden signals (latency, traffic, errors, saturation) always visible for any selected service. Distributed trace waterfall spans the full canvas width.

## 6. Depth & Elevation

```css
.shadow-card    { box-shadow: 0 1px 4px rgba(29, 36, 51, 0.07); }
.shadow-panel   { box-shadow: 0 6px 20px rgba(0, 172, 105, 0.10); }
.shadow-modal   { box-shadow: 0 20px 50px rgba(29, 36, 51, 0.18); }
```

Chart canvases use dark surfaces with no shadow — the data provides the visual interest.

## 7. Do's and Don'ts

Do always show the four golden signals for every service entity. Do use mono font for all NRQL queries and log lines. Do surface critical alerts immediately in the navigation. Do not use teal for alert or error states. Do not mix the severity color scale with chart series colors.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Alert notifications and critical entity status |
| Tablet | `768px` | Entity list with health indicators |
| Desktop | `1200px` | Full observability platform: dashboards, traces, logs, alerts |

Observability is desktop-primary. Mobile is for on-call alert response only.

## 9. Agent Prompt Guide

Design like New Relic: bold teal CTAs, four-tier severity scale, dark chart canvases, NRQL query panels in mono font, distributed trace waterfall, golden-signal entity cards, and full-stack observability hierarchy.
