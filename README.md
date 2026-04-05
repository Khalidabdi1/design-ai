# Design AI Systems

**Curated collection of DESIGN.md files capturing design systems from popular websites.**

Drop one into your project and let AI coding agents build matching UI.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![DESIGN.md Count](https://img.shields.io/badge/DESIGN.md%20count-27-10b981?style=classic)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## What is DESIGN.md?

[DESIGN.md](https://stitch.withgoogle.com/docs/design-md/overview/) is a plain-text design system document that AI agents read to generate consistent UI. It's just a markdown file - no Figma exports, no JSON schemas, no special tooling.

| File | Who reads it | What it defines |
|------|-------------|-----------------|
| `AGENTS.md` | Coding agents | How to build the project |
| `DESIGN.md` | Design agents | How the project should look and feel |

---

## What's Inside Each DESIGN.md

Every file follows the Stitch DESIGN.md format with extended sections:

| # | Section | What it captures |
|---|---------|-----------------|
| 1 | Visual Theme & Atmosphere | Mood, density, design philosophy |
| 2 | Color Palette & Roles | Semantic name + hex + functional role |
| 3 | Typography Rules | Font families, full hierarchy table |
| 4 | Component Stylings | Buttons, cards, inputs, navigation with states |
| 5 | Layout Principles | Spacing scale, grid, whitespace philosophy |
| 6 | Depth & Elevation | Shadow system, surface hierarchy |
| 7 | Do's and Don'ts | Design guardrails and anti-patterns |
| 8 | Responsive Behavior | Breakpoints, touch targets, collapsing strategy |
| 9 | Agent Prompt Guide | Quick color reference, ready-to-use prompts |

---

## How to Use

1. Copy a site's `DESIGN.md` into your project root
2. Tell your AI agent to use it
3. Get pixel-perfect UI that matches the design system

---

## Collection

### Social Media (8)

| Company | Description |
|---------|-------------|
| [**X (Twitter)**](design-md/x/) | Microblogging platform. Dark mode dominant, blue accent, minimalist |
| [**TikTok**](design-md/tiktok/) | Short video platform. Vibrant cyan/pink gradient, neon accents on dark |
| [**Reddit**](design-md/reddit/) | Community forums. Orange-red (#FF4500) accent, card-based layout |
| [**Discord**](design-md/discord/) | Community chat platform. Blurple (#5865F2) accent, gaming aesthetic |
| [**LinkedIn**](design-md/linkedin/) | Professional network. Corporate blue (#0A66C2), structured layouts |
| [**Snapchat**](design-md/snapchat/) | Messaging app. Yellow (#FFFC00) branding, playful UI |
| [**Threads**](design-md/threads/) | Text-based social. Clean black/white, Instagram-adjacent design |
| [**Mastodon**](design-md/mastodon/) | Decentralized social. Purple (#6364FF) accent, open-source aesthetic |

### E-commerce & Retail (6)

| Company | Description |
|---------|-------------|
| [**Amazon**](design-md/amazon/) | Everything store. Orange (#FF9900) accent, dense product layouts |
| [**Shopify**](design-md/shopify/) | E-commerce platform. Green (#008060) accent, Polaris design system |
| [**Etsy**](design-md/etsy/) | Handmade marketplace. Orange-coral (#F56400), artisan aesthetic |
| [**eBay**](design-md/ebay/) | Auction marketplace. Blue (#3665F3), multicolor logo |
| [**Target**](design-md/target/) | Retail chain. Red (#CC0000) bullseye branding, clean shopping UI |
| [**Walmart**](design-md/walmart/) | Retail giant. Blue (#0071DC) and yellow (#FFC220), utility-focused |

### Travel & Hospitality (1)

| Company | Description |
|---------|-------------|
| [**Booking.com**](design-md/booking/) | Hotel reservations. Deep blue (#003580), yellow CTAs, trust-focused |

### Food & Delivery (2)

| Company | Description |
|---------|-------------|
| [**DoorDash**](design-md/doordash/) | Food delivery. Red (#FF3008) accent, restaurant-focused |
| [**Starbucks**](design-md/starbucks/) | Coffee chain. Green (#00704A) siren, warm inviting UI |

### Gaming (6)

| Company | Description |
|---------|-------------|
| [**Steam**](design-md/steam/) | Gaming platform. Dark blue (#1b2838), cyan accent (#66c0f4) |
| [**Epic Games**](design-md/epicgames/) | Game store. Dark theme, blue (#0074e4), cinematic imagery |
| [**PlayStation**](design-md/playstation/) | Console gaming. Blue (#003791) accent, premium gaming |
| [**Xbox**](design-md/xbox/) | Console gaming. Green (#107C10) accent, Fluent Design |
| [**Nintendo**](design-md/nintendo/) | Gaming company. Red (#E60012), playful, family-friendly |
| [**Twitch**](design-md/twitch/) | Game streaming. Purple (#9146FF), live content focus |

### Developer Tools & Platforms (4)

| Company | Description |
|---------|-------------|
| [**GitHub**](design-md/github/) | Code hosting. Primer design system, octicon icons, developer-first |
| [**Vercel**](design-md/vercel/) | Deployment platform. Black-white precision, Geist font |
| [**Supabase**](design-md/supabase/) | Firebase alternative. Emerald green (#3ECF8E), code-first |
| [**OpenAI**](design-md/openai/) | AI research. Clean white/dark, ChatGPT green (#10a37f) |

### AI & Machine Learning (1)

| Company | Description |
|---------|-------------|
| [**Anthropic**](design-md/anthropic/) | AI safety company. Warm terracotta (#DA7756), editorial layout |

---

## Request a DESIGN.md

[Open a GitHub issue](https://github.com/your-username/design-ai-systems/issues/new?template=design-md-request.yml) to request a DESIGN.md generation for a website.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

- **Improve existing files**: Fix wrong colors, missing tokens, weak descriptions
- **Add new companies**: Follow the 9-section format
- **Report issues**: Let us know if something looks off

---

## License

MIT License - see [LICENSE](LICENSE)

This repository is a curated collection of design system documents extracted from public websites. All DESIGN.md files are provided "as is" without warranty. The extracted design tokens represent publicly visible CSS values. We do not claim ownership of any site's visual identity. These documents exist to help AI agents generate consistent UI.
