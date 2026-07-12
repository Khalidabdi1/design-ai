# Auth0 Design System
> Identity and authentication platform with a clean enterprise aesthetic — dark navy brand, orange accents, and security-infrastructure UI patterns.

---

## 1. Visual Theme & Atmosphere
Auth0 (by Okta) is enterprise identity infrastructure. The design communicates trust, scale, and technical depth. A dark navy brand anchors the visual identity, punctuated by an orange accent that brings energy and highlights key developer actions. Documentation and dashboards are clean and information-dense without feeling bureaucratic. The Universal Login page — the most-seen Auth0 UI — is pristine white and conversion-optimized.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#EB5424` | Brand orange, CTAs |
| `--color-primary-dark` | `#C94519` | Hover/active primary |
| `--color-primary-light` | `#FEF0EB` | Light badge backgrounds |
| `--color-navy` | `#16214D` | Brand navy, dark surfaces |
| `--color-navy-mid` | `#1E2E6B` | Elevated navy elements |
| `--color-bg-base` | `#FFFFFF` | Main content background |
| `--color-bg-subtle` | `#F8F9FC` | Section backgrounds |
| `--color-bg-dark` | `#0D1533` | Dark hero/sidebar surfaces |
| `--color-text-primary` | `#1A1F36` | Headings, primary text |
| `--color-text-secondary` | `#4A5568` | Body, labels |
| `--color-text-muted` | `#9AA5B1` | Meta, placeholders |
| `--color-border` | `#DDE1EB` | Default borders |
| `--color-success` | `#22C55E` | Authorized, passing |
| `--color-error` | `#EF4444` | Auth failure, error |
| `--color-warning` | `#F59E0B` | Deprecated, caution |

## 3. Typography Rules
```css
--font-sans: 'Inter', 'Aeonik', -apple-system, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 12px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 22px;
--font-size-xl: 30px;
--font-size-2xl: 40px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.2;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero Title | 40px | 700 | 1.2 |
| Page Title | 30px | 700 | 1.25 |
| Section Header | 22px | 600 | 1.3 |
| Card Title | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.5 |
| Label | 13px | 500 | 1.4 |
| Code | 13px | 400 | 1.5 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #EB5424;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  padding: 11px 22px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s;
}
.button-primary:hover { background: #C94519; }

/* Universal Login Form */
.login-form {
  background: #FFFFFF;
  border: 1px solid #DDE1EB;
  border-radius: 8px;
  padding: 40px 36px;
  max-width: 400px;
  width: 100%;
  box-shadow: 0 4px 24px rgba(0,0,0,0.07);
}
.login-form__logo {
  text-align: center;
  margin-bottom: 28px;
}
.login-form__title {
  font-size: 22px;
  font-weight: 700;
  color: #1A1F36;
  text-align: center;
  margin-bottom: 24px;
}

/* Input */
.input {
  border: 1.5px solid #DDE1EB;
  border-radius: 6px;
  padding: 11px 14px;
  font-size: 15px;
  color: #1A1F36;
  background: #FFFFFF;
  width: 100%;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #EB5424;
  box-shadow: 0 0 0 3px rgba(235,84,36,0.12);
}

/* Social Login Button */
.button-social {
  display: flex;
  align-items: center;
  gap: 10px;
  width: 100%;
  background: #FFFFFF;
  border: 1.5px solid #DDE1EB;
  border-radius: 6px;
  padding: 10px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #1A1F36;
  cursor: pointer;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.button-social:hover {
  border-color: #9AA5B1;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
}

/* Tenant Card */
.tenant-card {
  background: #FFFFFF;
  border: 1px solid #DDE1EB;
  border-radius: 8px;
  padding: 20px;
  cursor: pointer;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.tenant-card:hover {
  border-color: #EB5424;
  box-shadow: 0 4px 16px rgba(0,0,0,0.07);
}

/* Status Badge */
.status-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 9px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
}
.status-badge--active { background: rgba(34,197,94,0.1); color: #16A34A; }
.status-badge--error { background: rgba(239,68,68,0.1); color: #DC2626; }
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Tight gaps |
| `--spacing-sm` | `8px` | Form field spacing |
| `--spacing-md` | `16px` | Card padding |
| `--spacing-lg` | `24px` | Section gaps |
| `--spacing-xl` | `40px` | Form inner padding |
| `--login-max-width` | `400px` | Universal login form width |
| `--radius-sm` | `4px` | Badges |
| `--radius-md` | `6px` | Buttons, inputs, cards |

## 6. Depth & Elevation
```css
.shadow-login { box-shadow: 0 4px 24px rgba(0,0,0,0.07); }
.shadow-card { box-shadow: 0 2px 8px rgba(0,0,0,0.05); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Keep the Universal Login form centered at max 400px width
- Show social login buttons with provider logos at a consistent 20px size
- Use the orange accent for primary CTAs and focus rings
- Navy dark surfaces (#16214D) for hero sections and the sidebar

**Don't:**
- Don't mix orange (primary) with red (error) in close proximity
- Don't add marketing copy inside the login form — keep it conversion-focused
- Don't use the navy brand color for text on white backgrounds

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Login form full-width with horizontal padding |
| Tablet | 768px | Centered form at max 400px |
| Desktop | 1024px | Split: dark left panel + login form right |
| Wide | 1440px | Wider left panel with brand content |

## 9. Agent Prompt Guide
```
You are designing for Auth0 — enterprise identity and authentication platform.
Primary brand orange (#EB5424) for CTAs, input focus rings, and hover borders.
Dark navy (#16214D) for hero sections, sidebars, and marketing backgrounds.
The Universal Login form is white, centered, max 400px, with subtle border and shadow.
Social login buttons are white with 1.5px borders and provider logos.
Status badges use semantic pill styles: green=active, red=error.
Typography is Inter at 15px base; monospace for all tokens and config values.
Tone is enterprise-trustworthy, security-forward, and developer-approachable.
```
