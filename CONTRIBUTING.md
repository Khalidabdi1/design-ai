# Contributing to Design AI Systems

Thank you for your interest in contributing to the Design AI Systems collection! This document provides guidelines for contributing.

## How to Contribute

### Improving Existing DESIGN.md Files

1. **Fork the repository**
2. **Make your changes**
   - Fix incorrect color values
   - Update outdated typography information
   - Add missing component styles
   - Improve descriptions
3. **Submit a Pull Request**

### Adding New Companies

Before adding a new company, please [open an issue](https://github.com/Khalidabdi1/design-ai/issues/new?template=design-md-request.yml) to discuss.

#### DESIGN.md Structure

Every DESIGN.md file must include these 9 sections:

```markdown
# Design System: [Company Name]

## 1. Visual Theme & Atmosphere
[Mood, density, design philosophy]

## 2. Color Palette & Roles
[Semantic name + hex + functional role]

## 3. Typography Rules
[Font families, full hierarchy table]

## 4. Component Stylings
[Buttons, cards, inputs, navigation with states]

## 5. Layout Principles
[Spacing scale, grid, whitespace philosophy]

## 6. Depth & Elevation
[Shadow system, surface hierarchy]

## 7. Do's and Don'ts
[Design guardrails and anti-patterns]

## 8. Responsive Behavior
[Breakpoints, touch targets, collapsing strategy]

## 9. Agent Prompt Guide
[Quick color reference, ready-to-use prompts]
```

#### File Structure

Each company should have its own directory:

```
design-md/
└── [company-name]/
    ├── DESIGN.md
    ├── preview.html
    └── preview-dark.html
```

### Quality Standards

- **Accuracy**: All design tokens must be extracted from the actual website
- **Completeness**: Include all 9 sections
- **Clarity**: Descriptions should be clear and actionable for AI agents
- **Consistency**: Follow the established format and style

### Extracting Design Tokens

When documenting a design system:

1. **Colors**: Use browser DevTools to extract exact hex/rgba values
2. **Typography**: Note font families, sizes, weights, line-heights, letter-spacing
3. **Spacing**: Document the spacing scale used
4. **Shadows**: Copy exact box-shadow values
5. **Border Radius**: Note all radius values used

### Preview HTML Files

Each company should include:

- `preview.html` - Light mode visual catalog
- `preview-dark.html` - Dark mode visual catalog

These should demonstrate:
- Color swatches
- Typography scale
- Button variants
- Card components
- Input fields
- Navigation elements

## Code of Conduct

- Be respectful and constructive
- Focus on improving the quality of design documentation
- Credit original design systems appropriately

## Questions?

Open an issue if you have questions about contributing.
