# Stytch Design System
> Authentication and identity platform with a clean enterprise aesthetic — deep navy, electric purple accents, and security-first UI patterns.

---

## 1. Visual Theme & Atmosphere
Stytch communicates trust, security, and developer confidence. The palette is anchored in deep navy with electric purple-blue accents — authoritative without being cold. UI is clean and conversion-optimized: authentication flows are frictionless, developer documentation is scannable, and every component signals reliability. The aesthetic bridges the gap between enterprise security and modern developer experience.

## 2. Color Palette & Roles
| Token | Hex | Role |
|-------|-----|------|
| `--color-primary` | `#7B5EA7` | Brand purple, CTAs |
| `--color-primary-dark` | `#6347A0` | Hover/active primary |
| `--color-primary-light` | `#F3F0F9` | Light backgrounds, badges |
| `--color-accent` | `#4F87F7` | Links, secondary highlights |
| `--color-navy` | `#1B1F3B` | Deep navy, dark surfaces |
| `--color-navy-light` | `#252A4B` | Elevated dark panels |
| `--color-success` | `#22C55E` | Auth success, verified |
| `--color-error` | `#EF4444` | Auth failure, invalid |
| `--color-warning` | `#F59E0B` | Rate limits, caution |
| `--color-neutral-900` | `#111827` | Headings, primary text |
| `--color-neutral-600` | `#4B5563` | Body text |
| `--color-neutral-400` | `#9CA3AF` | Secondary labels |
| `--color-neutral-200` | `#E5E7EB` | Borders, dividers |
| `--color-neutral-50` | `#F9FAFB` | Page backgrounds |
| `--color-white` | `#FFFFFF` | Card surfaces |

## 3. Typography Rules
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', monospace;
--font-size-xs: 12px;
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-md: 17px;
--font-size-lg: 21px;
--font-size-xl: 28px;
--font-size-2xl: 36px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--line-height-tight: 1.25;
--line-height-base: 1.5;
```
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero Title | 36px | 700 | 1.2 |
| Page Title | 28px | 700 | 1.25 |
| Section Header | 21px | 600 | 1.3 |
| Card Title | 17px | 600 | 1.4 |
| Body | 15px | 400 | 1.5 |
| Label / Meta | 13px | 500 | 1.4 |
| Code / Mono | 13px | 400 | 1.5 |
| Caption | 12px | 400 | 1.4 |

## 4. Component Stylings
```css
/* Primary Button */
.button-primary {
  background: #7B5EA7;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;
  padding: 10px 20px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.15s ease;
}
.button-primary:hover { background: #6347A0; }

/* Auth Form Container */
.auth-container {
  background: #FFFFFF;
  border: 1px solid #E5E7EB;
  border-radius: 12px;
  padding: 32px;
  max-width: 420px;
  width: 100%;
  box-shadow: 0 4px 24px rgba(0,0,0,0.08);
}

/* Magic Link / OTP Input */
.otp-input {
  width: 48px;
  height: 56px;
  border: 2px solid #E5E7EB;
  border-radius: 8px;
  text-align: center;
  font-size: 20px;
  font-weight: 700;
  color: #111827;
  transition: border-color 0.15s;
}
.otp-input:focus {
  outline: none;
  border-color: #7B5EA7;
  box-shadow: 0 0 0 3px rgba(123,94,167,0.15);
}

/* Provider Button (SSO / OAuth) */
.button-provider {
  display: flex;
  align-items: center;
  gap: 10px;
  width: 100%;
  background: #FFFFFF;
  border: 1.5px solid #E5E7EB;
  border-radius: 8px;
  padding: 10px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #111827;
  cursor: pointer;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.button-provider:hover {
  border-color: #7B5EA7;
  box-shadow: 0 2px 8px rgba(123,94,167,0.12);
}

/* Input */
.input {
  border: 1.5px solid #E5E7EB;
  border-radius: 8px;
  padding: 10px 14px;
  font-size: 15px;
  font-family: var(--font-sans);
  color: #111827;
  background: #FFFFFF;
  width: 100%;
  transition: border-color 0.15s;
}
.input:focus {
  outline: none;
  border-color: #7B5EA7;
  box-shadow: 0 0 0 3px rgba(123,94,167,0.15);
}

/* Security Badge */
.security-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: 100px;
  font-size: 12px;
  font-weight: 600;
  background: rgba(34,197,94,0.1);
  color: #16A34A;
  border: 1px solid rgba(34,197,94,0.2);
}
```

## 5. Layout Principles
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-xs` | `4px` | Icon gaps |
| `--spacing-sm` | `8px` | Inline padding |
| `--spacing-md` | `16px` | Input field spacing |
| `--spacing-lg` | `24px` | Form sections |
| `--spacing-xl` | `32px` | Card padding |
| `--spacing-2xl` | `48px` | Page sections |
| `--auth-max-width` | `420px` | Max width for auth forms |
| `--radius-sm` | `6px` | Badges, chips |
| `--radius-md` | `8px` | Buttons, inputs |
| `--radius-lg` | `12px` | Auth containers, cards |

## 6. Depth & Elevation
```css
.shadow-form { box-shadow: 0 4px 24px rgba(0,0,0,0.08); }
.shadow-card { box-shadow: 0 2px 12px rgba(0,0,0,0.06); }
.shadow-modal { box-shadow: 0 16px 48px rgba(0,0,0,0.14); }
.shadow-provider-hover { box-shadow: 0 2px 8px rgba(123,94,167,0.12); }
```

## 7. Do's and Don'ts
**Do:**
- Keep auth flows to a single focused element per screen
- Show progress indicators in multi-step auth flows
- Use green success states immediately after verified actions
- Provide clear error messages with actionable recovery steps
- Use provider brand logos at the correct aspect ratios in OAuth buttons

**Don't:**
- Don't ask for more information than necessary in auth flows
- Don't use generic "Something went wrong" errors — always specify the issue
- Don't use red for anything other than actual auth failure states
- Don't put navigation or marketing content near auth forms

## 8. Responsive Behavior
| Breakpoint | Min Width | Behavior |
|------------|-----------|----------|
| Mobile | 320px | Auth form full-width, centered vertically |
| Tablet | 768px | Auth form centered with padding, max 420px |
| Desktop | 1024px | Split-screen: brand/marketing left, auth form right |
| Wide | 1440px | Same as desktop with expanded marketing panel |

## 9. Agent Prompt Guide
```
You are designing for Stytch — an authentication and identity platform.
Primary brand color is purple (#7B5EA7) on white cards and forms.
Deep navy (#1B1F3B) is used for dark surfaces and hero backgrounds.
Auth forms are centered, max 420px wide, white cards with subtle shadow and border radius 12px.
OTP/magic inputs use large bold numbers with purple focus rings.
Provider OAuth buttons are white with thin borders, using brand logos at left.
Security and success states use green (#22C55E) badge-style indicators.
Tone is trustworthy, conversion-focused, and security-forward.
```
