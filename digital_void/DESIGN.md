---
name: Digital Void
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#b9ccb2'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#84967e'
  outline-variant: '#3b4b37'
  surface-tint: '#00e639'
  primary: '#ebffe2'
  on-primary: '#003907'
  primary-container: '#00ff41'
  on-primary-container: '#007117'
  inverse-primary: '#006e16'
  secondary: '#99d688'
  on-secondary: '#003a00'
  secondary-container: '#1e5416'
  on-secondary-container: '#8cc77b'
  tertiary: '#fcf8f8'
  on-tertiary: '#313030'
  tertiary-container: '#dfdcdb'
  on-tertiary-container: '#626060'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#72ff70'
  primary-fixed-dim: '#00e639'
  on-primary-fixed: '#002203'
  on-primary-fixed-variant: '#00530e'
  secondary-fixed: '#b5f3a2'
  secondary-fixed-dim: '#99d688'
  on-secondary-fixed: '#002200'
  on-secondary-fixed-variant: '#1b5114'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c9c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474646'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  headline-lg:
    fontFamily: JetBrains Mono
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.6'
  label-lg:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
  code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  grid-cols: '12'
---

## Brand & Style
The design system is a high-fidelity tribute to the digital frontier, inspired by terminal interfaces and early cyberpunk aesthetics. It targets developers, security researchers, and enthusiasts who appreciate a focused, distraction-free environment that prioritizes raw data and technical precision.

The style is a fusion of **Brutalism** and **Modern Terminal** aesthetics. It rejects organic shapes in favor of a rigid, high-tech grid. The emotional response is one of total immersion, authority, and "under-the-hood" access. Surfaces are treated as digital voids, where light only exists as phosphorus data emitted from a CRT screen.

## Colors
The palette is strictly high-contrast and optimized for dark environments to reduce eye strain and maximize the "hacker" aesthetic.

- **Primary (#00FF41):** The "Matrix Green." Used for all active text, primary actions, and critical data indicators. It represents the phosphor glow of a terminal.
- **Secondary (#003B00):** A deep, muted green used for subtle borders, inactive states, and decorative grid lines.
- **Tertiary (#008F11):** An intermediate green used for hover states and secondary information.
- **Neutral/Surface (#000000):** Pure black serves as the foundation to ensure the primary green has maximum visual impact.
- **Surface-Elevated (#0D0D0D):** A charcoal tint used sparingly for layering components that must sit "above" the base void.

## Typography
Typography is the core of this design system. By utilizing **JetBrains Mono** across all levels, we reinforce the monospaced, systematic nature of a code editor. 

Headlines should be rendered in the primary green with a subtle text-shadow to simulate CRT "bleeding." Smaller labels should use uppercase styling with increased letter spacing to provide a structured, utilitarian feel. All text must be legible against the pure black background, strictly adhering to the primary and secondary green shades.

## Layout & Spacing
The layout follows a **Strict Fluid Grid** based on 4px increments. Everything aligns to a vertical and horizontal rhythm that mimics terminal line heights.

- **Grid:** A 12-column system is used for desktop, collapsing to 4 columns on mobile.
- **Borders:** Instead of margins, use thin 1px borders in secondary green to define sections, creating a "windowed" terminal effect.
- **Density:** High density is preferred. Elements should be packed tightly but aligned perfectly to the 4px grid to maintain a professional, technical appearance.

## Elevation & Depth
In this design system, depth is not conveyed through shadows or Z-axis height, but through **Color Intensity and Glow**.

- **Base Layer:** Pure black (#000000).
- **Secondary Layer:** Deep charcoal (#0D0D0D) with a 1px border of secondary green (#003B00).
- **Glow Effects:** Critical elements and active states use a "phosphor glow"—a drop shadow with 0 offset and a small blur (4px to 8px) using the primary green at 50% opacity.
- **Scanlines:** A global overlay of faint, horizontal transparent lines (2px height) can be applied to the entire viewport to enhance the retro-hardware feel.

## Shapes
The shape language is **Strictly Geometric and Sharp**. 

There are no rounded corners in this design system. Every button, input, card, and modal must have 90-degree angles. This reinforces the digital, non-organic nature of the interface. Geometric icons and box-drawing characters (┌, ┐, └, ┘) should be used to frame content areas.

## Components

### Buttons
Buttons are rectangular containers with a 1px border.
- **Primary:** Primary green text and border. On hover, the background fills with primary green and text flips to black.
- **Ghost:** Secondary green border and text. No background.

### Input Fields
Inputs are defined by a 1px bottom border or full sharp-edged box. The cursor should be a solid primary green block that blinks, mimicking a terminal prompt.

### Cards
Cards use a pure black background with a 1px secondary green border. Headers of cards are separated by a horizontal 1px line. There is no shadow; depth is suggested by the border contrast.

### Lists
Lists should be prefixed with characters like `>` or `$` to maintain the command-line interface feel. Inactive items use secondary green, while the active/selected item uses primary green with a subtle glow.

### Terminal Output (Special Component)
A dedicated container for data streams. It uses a slightly smaller font size (12px) and can include "scrolling text" animations for status updates. Use primary green for success, and a high-contrast amber (#FFB000) for warnings—avoiding standard reds to keep the palette focused.