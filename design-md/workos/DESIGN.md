# WorkOS Design System

> Enterprise auth design with confident blue identity, SSO-first surfaces, admin portal clarity, and B2B-ready integration UX.

---

## 1. Visual Theme & Atmosphere

WorkOS should feel enterprise-ready, developer-friendly, and trustworthy. The design language communicates Single Sign-On, SCIM provisioning, fine-grained authorization, Admin Portal, and the infrastructure that makes apps enterprise-grade.

- Mood: enterprise-ready, developer-friendly, reliable, professional
- Density: medium, with SSO connection tables, directory sync dashboards, organization management, and audit log surfaces
- Character: confident blue brand, clean white enterprise surfaces, dark sidebar navigation, compliance-ready clarity

## 2. Color Palette & Roles

| Token | Hex | Role |
|-------|-----|------|
| `--wos-blue` | `#6363F1` | Primary brand CTA and active connection |
| `--wos-blue-dark` | `#4E4ECC` | Hover and active states |
| `--wos-indigo` | `#3730A3` | Navigation sidebar and dark surfaces |
| `--wos-green` | `#16A34A` | SSO active and provisioning synced |
| `--wos-amber` | `#D97706` | Connection pending and review needed |
| `--wos-red` | `#DC2626` | Connection failed and deprovisioned |
| `--wos-purple` | `#7C3AED` | Fine-grained authorization accent |
| `--surface-card` | `#FFFFFF` | Connection and organization cards |
| `--surface-bg` | `#F8FAFC` | Dashboard background |
| `--surface-sidebar` | `#1E1B4B` | Deep indigo sidebar |
| `--text-primary` | `#111827` | Organization names and labels |
| `--border-default` | `#E2E8F0` | Panel and row borders |

Blue is the primary action and brand signal. The connection-status scale (green/amber/red) must be strictly consistent — it communicates whether enterprise customers can actually log in.

## 3. Typography Rules

```css
--font-sans: Inter, ui-sans-serif, system-ui, -apple-system, sans-serif;
--font-mono: "JetBrains Mono", "SF Mono", Menlo, monospace;
```

| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Page Title | 28px | 700 | 1.1 |
| Section Title | 22px | 600 | 1.2 |
| Org Name | 15px | 600 | 1.3 |
| Body | 15px | 400 | 1.6 |
| Code / Client ID | 13px | 400 | 1.5 |
| Connection Status | 12px | 600 | 1.35 |
| Label | 12px | 600 | 1.35 |

## 4. Component Stylings

```css
.button-primary {
  min-height: 38px;
  padding: 0 16px;
  border: none;
  border-radius: 8px;
  background: #6363F1;
  color: #FFFFFF;
  font: 600 14px/1 Inter, sans-serif;
}

.connection-card {
  border: 1px solid #E2E8F0;
  border-radius: 10px;
  background: #FFFFFF;
  padding: 16px 20px;
  display: flex;
  align-items: center;
  gap: 14px;
}

.org-row {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  border-bottom: 1px solid #E2E8F0;
}

.connection-status {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 3px 10px;
  border-radius: 999px;
  font: 600 12px/1.4 Inter, sans-serif;
}

.code-value {
  font: 400 13px/1 "JetBrains Mono", monospace;
  padding: 3px 8px;
  border-radius: 4px;
  background: #F1F5F9;
  color: #475569;
}
```

## 5. Layout Principles

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | `8px` | Connection row spacing |
| `--space-4` | `16px` | Card rhythm |
| `--space-6` | `24px` | Section padding |
| `--space-10` | `40px` | Dashboard section gaps |

Organizations list is the primary surface. Each org expands to show its SSO connections, directory sync, and audit logs. API keys and client IDs always display in mono with a copy button.

## 6. Depth & Elevation

```css
.shadow-card   { box-shadow: 0 1px 4px rgba(17, 24, 39, 0.06); }
.shadow-panel  { box-shadow: 0 8px 24px rgba(99, 99, 241, 0.10); }
.shadow-modal  { box-shadow: 0 20px 50px rgba(17, 24, 39, 0.16); }
```

Clean, flat surfaces with minimal shadow — enterprise tools convey reliability through precision, not decoration.

## 7. Do's and Don'ts

Do always show connection status with a color indicator and a text label. Do display client IDs and API keys in mono with one-click copy. Do surface organization count and active SSO connections on the dashboard. Do not use blue for failed connection states. Do not hide the audit log — enterprise customers require it for compliance.

## 8. Responsive Behavior

| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | `0px` | Organization list with connection status |
| Tablet | `768px` | Organization table with SSO status columns |
| Desktop | `1200px` | Full dashboard: orgs + connections + directory sync + audit log |

Enterprise auth management is a desktop workflow. Mobile for monitoring only.

## 9. Agent Prompt Guide

Design like WorkOS: confident blue CTAs, deep indigo sidebar, SSO-connection status scale, organization management tables, mono API key display, enterprise-ready clean surfaces, and B2B auth infrastructure hierarchy.
