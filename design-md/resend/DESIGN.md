# Resend Design System

> Developer email API design with clean black identity, code-first surfaces, deliverability-metric clarity, and DX-obsessed simplicity.

---

## 1. Visual Theme & Atmosphere

Resend should feel clean, fast, and developer-obsessed. The design language communicates transactional email APIs, React email templates, domain authentication, deliverability analytics, and a DX that makes email feel like a joy.

- Mood: clean, developer-obsessed, modern, minimal
- Density: low-to-medium, with generous whitespace, code-first examples, and deliverability dashboards
- Character: clean black brand, white surfaces, subtle gray hierarchy, code-snippet-first documentation

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--res-black` | `#000000` | Primary brand CTA and identity |
| `--res-gray-900` | `#111827` | Primary text |
| `--res-gray-600` | `#4B5563` | Secondary text |
| `--res-green` | `#16A34A` | Delivered and domain verified |
| `--res-amber` | `#D97706` | Pending and unverified |
| `--res-red` | `#DC2626` | Bounced, complained, and blocked |
| `--res-blue` | `#3B82F6` | Links and informational |
| `--surface-card` | `#FFFFFF` | Email log and domain cards |
| `--surface-bg` | `#FAFAFA` | Dashboard background |
| `--surface-code` | `#18181B` | Code block background |
| `--text-primary` | `#111827` | Labels and values |
| `--border-default` | `#E4E4E7` | Card and panel borders |

Black is the identity — pure, confident, minimal. The delivery-status color scale (green/amber/red) must be used consistently across all email log views.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "Geist Mono", "JetBrains Mono", "Fira Code", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 30px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| Card Title | 18px | 600 | 1.3 |
| Body | 15px | 400 | 1.65 |
| Code | 13px | 400 | 1.75 |
| Email Log Row | 14px | 400 | 1.5 |
| Label | 12px | 600 | 1.35 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 38px;
  padding: 0 16px;
  border: none;
  border-radius: 8px;
  background: #000000;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.code-block {
  border-radius: 10px;
  background: #18181B;
  color: #E4E4E7;
  padding: 20px 24px;
  font: 400 13px/1.75 "Geist Mono", monospace;
  border: 1px solid #27272A;
}

.email-log-row {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  border-bottom: 1px solid #F4F4F5;
  font: 400 14px/1.5 Inter, sans-serif;
}

.domain-card {
  border: 1px solid #E4E4E7;
  border-radius: 10px;
  background: #FFFFFF;
  padding: 20px 24px;
}

.status-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  flex-shrink: 0;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Email log row spacing |
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

Code examples appear at every possible opportunity — Resend is a developer product and code is the primary documentation. Email log table is the main dashboard surface.

## 6. Depth & Elevation

```css
.shadow-card   { box-shadow: 0 1px 3px rgba(0, 0, 0, 0.06); }
.shadow-panel  { box-shadow: 0 4px 16px rgba(0, 0, 0, 0.08); }
.shadow-modal  { box-shadow: 0 20px 50px rgba(0, 0, 0, 0.16); }
```

Minimal shadows — Resend's aesthetic is flat and clean. Let borders and whitespace define structure.

## 7. Do's and Don'ts

Do show a code snippet as the first thing on every feature page. Do use mono font for all email addresses, message IDs, and API keys. Do surface bounce and complaint rates prominently — they matter for deliverability. Do not use excessive decoration. Do not hide domain authentication status.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Email log summary, domain status |
| Tablet | `768px` | Email log table, basic analytics |
| Desktop | `1200px` | Full dashboard: logs, domains, analytics, and API explorer |

Documentation reading happens on all devices. Dashboard management is desktop-primary.

## 9. Agent Prompt Guide

Design like Resend: clean black CTAs, code-first documentation surfaces, dark mono code blocks, email-log table with status dots, minimal whitespace-driven layout, and DX-obsessed email API hierarchy.
