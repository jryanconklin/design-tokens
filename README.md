# Design Tokens Demo

A clean, foundational set of design tokens for demonstration and reference purposes.

## Overview

This repository contains a minimal design token system organized in JSON format. These tokens represent the building blocks of a design system and can be used as:

- A reference for creating your own design system
- Source files for Style Dictionary or other token transformation tools
- Documentation for design and development teams
- A starting point for brand-specific token libraries

## Token Categories

- **Colors** (`color.tokens.json`) - Neutral palette with black and white
- **Spacing** (`spacing.tokens.json`) - Base-8 spacing scale (0-192px)
- **Typography** - Font families, sizes, weights, letter spacing, and line heights
  - `font.tokens.json` - Font families, sizes, and weights
  - `letter-spacing.tokens.json` - Letter spacing scale
  - `line-height.tokens.json` - Line height scale
- **Borders** (`border.tokens.json`) - Border widths and radius values
- **Radius** (`radius.tokens.json`) - Border radius scale
- **Shadows** (`shadow.tokens.json`) - Elevation system for depth
- **Breakpoints** (`breakpoint.tokens.json`) - Responsive design breakpoints
- **Duration** (`duration.tokens.json`) - Animation and transition timing
- **Animation** (`animation.tokens.json`) - Rotation and easing functions
- **Opacity** (`opacity.tokens.json`) - Transparency scale
- **Z-Index** (`z-index.tokens.json`) - Stacking order for UI layers

## Project Structure

```
.
├── design-tokens/
│   └── src/
│       ├── animation.tokens.json
│       ├── border.tokens.json
│       ├── breakpoint.tokens.json
│       ├── color.tokens.json
│       ├── duration.tokens.json
│       ├── font.tokens.json
│       ├── letter-spacing.tokens.json
│       ├── line-height.tokens.json
│       ├── opacity.tokens.json
│       ├── radius.tokens.json
│       ├── shadow.tokens.json
│       ├── spacing.tokens.json
│       └── z-index.tokens.json
├── .gitignore
└── README.md
```

## Usage

These token files are plain JSON and can be:

1. **Imported directly** into your build tools or token transformation pipeline
2. **Used with Style Dictionary** - Add a `config.json` to transform into CSS, SCSS, JavaScript, etc.
3. **Referenced in design tools** like Figma using plugins that support design tokens
4. **Copied and customized** for your specific brand needs

### Example Token Structure

```json
{
  "spacing": {
    "4": {
      "value": 32,
      "type": "dimension"
    }
  }
}
```

## Design Principles

- **Base-8 spacing system** - All spacing values are multiples of 8px
- **Semantic naming** - Token names describe purpose, not specific values
- **Platform-agnostic** - Generic format compatible with token transformation tools
- **Minimal but complete** - Covers essential design system categories without overwhelming complexity
- **Demo-friendly** - Simple structure for learning and reference

## Next Steps

To use these tokens in production:

1. **Add brand colors** - Replace or extend the neutral palette with your brand colors
2. **Implement Style Dictionary** - Transform tokens into platform-specific formats
3. **Add semantic tokens** - Create component-level tokens that reference these foundation tokens
4. **Version control** - Track changes to maintain consistency across your design system

## Resources

- [Style Dictionary](https://styledictionary.com/) - Transform tokens into any platform format
- [Design Tokens W3C Community Group](https://www.w3.org/community/design-tokens/) - Token format specifications
- [Design Tokens (Figma Plugin)](figma.com/community/plugin/888356646278934516) - Export variables to/from Figma

## License

MIT - Feel free to use, modify, and distribute as needed.
