# Airbyte Design System

> Open-source data integration design with bold blue identity, connector-catalog surfaces, pipeline-flow clarity, and ELT-first developer UX.

---

## 1. Visual Theme & Atmosphere

Airbyte should feel open, powerful, and developer-trusted. The design language communicates data connectors, ELT pipelines, sync schedules, schema normalization, and the open-source ecosystem behind modern data infrastructure.

- Mood: open, reliable, developer-native, data-forward
- Density: medium-to-high, with connector catalogs, sync logs, schema tables, and pipeline dashboards
- Character: bold blue brand, white pipeline surfaces, dark sync-log panels, connector-icon grid

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--ab-blue` | `#615EFF` | Primary brand CTA and active connector |
| `--ab-blue-dark` | `#4B48DD` | Hover and active states |
| `--ab-green` | `#00D97E` | Sync successful and healthy connection |
| `--ab-amber` | `#F5A623` | Sync warning and partial failure |
| `--ab-red` | `#F04438` | Sync failed and connection error |
| `--ab-teal` | `#0BA5EC` | Schema and transformation accent |
| `--surface-card` | `#FFFFFF` | Connector and sync cards |
| `--surface-bg` | `#F9FAFB` | Dashboard background |
| `--surface-log` | `#0D1117` | Sync log and debug panel |
| `--text-primary` | `#101828` | Connector names and schema labels |
| `--text-secondary` | `#667085` | Last sync time and row counts |
| `--border-default` | `#EAECF0` | Panel and table borders |

Blue is the primary action and brand signal. The sync-status color scale (green/amber/red) is critical — it must never be repurposed and must be applied consistently across all connection views.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| Connector Name | 15px | 600 | 1.3 |
| Body | 15px | 400 | 1.6 |
| Log Line | 13px | 400 | 1.7 |
| Schema Field | 13px | 500 | 1.4 |
| Label | 12px | 600 | 1.35 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 40px;
  padding: 0 18px;
  border: none;
  border-radius: 8px;
  background: #615EFF;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.connector-card {
  border: 1px solid #EAECF0;
  border-radius: 12px;
  background: #FFFFFF;
  padding: 20px;
  display: flex;
  align-items: center;
  gap: 14px;
}

.sync-status {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 3px 10px;
  border-radius: 999px;
  font: 600 12px/1.4 Inter, sans-serif;
}

.log-panel {
  border-radius: 10px;
  background: #0D1117;
  color: #8B949E;
  padding: 16px 20px;
  font: 400 13px/1.7 "JetBrains Mono", monospace;
  overflow-y: auto;
}

.schema-row {
  display: grid;
  grid-template-columns: 1fr auto auto;
  padding: 10px 14px;
  border-bottom: 1px solid #EAECF0;
  font: 400 13px/1.5 Inter, sans-serif;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Connector card internal spacing |
| `--space-4` | `16px` | Core rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

Connector catalog uses a searchable grid. Active connections list with status indicators. Sync log expands inline below each connection row — never navigate away.

## 6. Depth & Elevation

```css
.shadow-card   { box-shadow: 0 1px 4px rgba(16, 24, 40, 0.06); }
.shadow-panel  { box-shadow: 0 8px 24px rgba(97, 94, 255, 0.10); }
.shadow-modal  { box-shadow: 0 20px 50px rgba(16, 24, 40, 0.16); }
```

Connector cards are lightweight. Sync configuration modals carry more weight to signal importance.

## 7. Do's and Don'ts

Do show sync status and last-run time on every connection card. Do use mono font for all log output and schema field names. Do surface failed syncs at the top of the connection list automatically. Do not use blue for sync-warning or error states. Do not hide the sync log — it is the primary debugging surface.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Connection status list, no configuration |
| Tablet | `768px` | Connector catalog and connection list |
| Desktop | `1200px` | Full workspace: catalog + connections + schema browser + logs |

Data pipeline configuration is a desktop workflow. Mobile is for status monitoring only.

## 9. Agent Prompt Guide

Design like Airbyte: bold blue CTAs, connector-icon catalog grid, sync-status color scale, dark log panels with mono font, schema browser tables, and open-source ELT pipeline hierarchy.
