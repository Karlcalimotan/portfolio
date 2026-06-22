---
name: Kinetic Syntax
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#bbcabf'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#86948a'
  outline-variant: '#3c4a42'
  surface-tint: '#4edea3'
  primary: '#4edea3'
  on-primary: '#003824'
  primary-container: '#10b981'
  on-primary-container: '#00422b'
  inverse-primary: '#006c49'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#ffb3af'
  on-tertiary: '#650911'
  tertiary-container: '#fc7c78'
  on-tertiary-container: '#711419'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#6ffbbe'
  primary-fixed-dim: '#4edea3'
  on-primary-fixed: '#002113'
  on-primary-fixed-variant: '#005236'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#ffdad7'
  tertiary-fixed-dim: '#ffb3af'
  on-tertiary-fixed: '#410005'
  on-tertiary-fixed-variant: '#842225'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  headline-xl:
    fontFamily: JetBrains Mono
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 16px
  section-gap: 120px
---

## Brand & Style
The design system is engineered for high-performance software professionals. It bridges the gap between functional IDE aesthetics and high-end editorial design. The brand personality is precise, technical, and forward-thinking, prioritizing clarity of information through a **Tech-Minimalist** lens.

The visual style utilizes a **Glassmorphic-Industrial** hybrid: 
- **Precision:** Thin, 1px strokes reminiscent of wireframes.
- **Depth:** Translucent layers that suggest a complex, multi-threaded architecture.
- **Focus:** Generous whitespace ensures that technical achievements and code samples remain the primary focal point.

## Colors
The palette is rooted in a deep, "Midnight Terminal" environment to reduce eye strain and emphasize vibrant accent colors.

- **Primary (Success Green):** An emerald hue representing active states, passing tests, and deployment success. Use for primary actions and "live" indicators.
- **Secondary (Logic Blue):** An electric blue used for links, data visualization, and subtle accents.
- **Neutrals:** A spectrum of slates and charcoals. The background is a near-black navy to provide more depth than pure black, while surfaces use a lighter slate for layered hierarchy.

## Typography
The typography strategy employs a "Functional Contrast" pairing:
- **JetBrains Mono** is utilized for headlines, labels, and technical metadata. This creates an immediate mental association with development environments and precise logic.
- **Inter** serves as the workhorse for long-form content, project descriptions, and experience narratives. It provides high legibility and a modern, neutral feel that balances the technicality of the monospace headers.
- **Hierarchy:** Use `label-caps` for tech-stack tags and section subtitles to create a distinct structural rhythm.

## Layout & Spacing
The design system follows a **Fluid 12-Column Grid** with a logic-based spacing scale (4px increments). 

- **Sectioning:** Large vertical gaps (120px+) are used between major portfolio sections to create an "uncluttered" atmosphere.
- **Mobile:** On mobile devices, margins shrink to 16px, and column spans typically collapse to a single-column stack.
- **Alignment:** All elements should align to the left to mirror the structure of a code editor (the "left-margin" bias).

## Elevation & Depth
Depth is communicated through **Refractive Glassmorphism** rather than traditional shadows.

- **Surface Tiers:** Background is the deepest layer. Cards sit on top with a 10-15% opacity white fill and a `backdrop-filter: blur(12px)`.
- **Borders:** Every container uses a 1px solid border. The border color should be a slightly lighter version of the surface color (e.g., Slate 700) with low opacity (30%) to simulate a "glass edge."
- **Interaction:** Hovering over a card should increase the border opacity and apply a very subtle, colored outer glow using the Primary or Secondary accent color.

## Shapes
Shapes in this design system are disciplined and "Soft-Technical." 

- **Standard Radius:** Use `0.25rem` (4px) for most UI elements (inputs, buttons, cards). This avoids the playfulness of high-roundedness while feeling more sophisticated than sharp 90-degree corners.
- **Consistency:** Maintain the same radius across all nested elements to preserve the "engineered" feel of the components.

## Components
### Project Cards
Constructed as glassmorphic containers. Headers use `headline-lg`. Include a "Footer" area within the card for `label-caps` tech-stack tags. Tags should have a subtle background tint and no border.

### Experience Timeline
A vertical line (1px, Slate 800) with `primary_color` nodes. Dates use `code-sm` to emphasize the chronological "logs" of the engineer's career.

### Buttons
- **Primary:** Solid `primary_color` with black text for maximum contrast. Sharp, 4px corners.
- **Ghost:** Transparent background with a `secondary_color` 1px border.

### Input Fields
Darker than the surface (`background_hex`), with a 1px slate border. Upon focus, the border shifts to `secondary_color` and the label (if using floating labels) uses the monospace font.

### Tech Stack Badges
Small, high-contrast pills. Use a monospace font at 12px. Backgrounds should be low-opacity versions of the accent colors (e.g., 10% Green for Node.js, 10% Blue for React).