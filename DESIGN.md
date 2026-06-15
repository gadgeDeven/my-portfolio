---
name: Obsidian Kinetic
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
  on-surface-variant: '#b9cacb'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ebb2ff'
  on-secondary: '#520072'
  secondary-container: '#b600f8'
  on-secondary-container: '#fff6fc'
  tertiary: '#dcffe2'
  on-tertiary: '#00391d'
  tertiary-container: '#00f990'
  on-tertiary-container: '#006d3c'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ebb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#5bffa1'
  tertiary-fixed-dim: '#00e383'
  on-tertiary-fixed: '#00210e'
  on-tertiary-fixed-variant: '#00522c'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-desktop: 80px
  margin-mobile: 20px
  container-max: 1200px
---

## Brand & Style

This design system targets high-performance frontend engineering with a gamified, immersive edge. The aesthetic is built on **Glassmorphism** and **High-Contrast Modernism**, creating a digital environment that feels like a premium developer cockpit. 

The brand personality is authoritative yet energetic, designed to evoke a sense of technical mastery. By utilizing deep obsidian surfaces and vibrant neon accents, the UI creates a clear distinction between "static" information and "active" gamified elements like skill levels and experience progression. The overall mood is "high-fidelity technical elegance."

## Colors

The palette is optimized for a deep dark-mode experience.
- **Primary (Neon Blue):** Used for primary actions, current level indicators, and core interactive states.
- **Secondary (Vibrant Purple):** Reserved for "Epic" achievements, high-tier skills, and decorative gradients.
- **Tertiary (Neon Green):** Indicates success states, "Online" status, and completed quest-logs.
- **Neutral (Obsidian & Slate):** The foundational layers. The background is a near-black obsidian, while surfaces use semi-transparent slate to facilitate the glassmorphic effect.

All interactive elements should utilize a subtle outer glow (bloom) in their respective accent color to simulate a physical neon light source.

## Typography

The system utilizes **Geist** for its precision and modernist neutrality, ensuring high legibility in high-density data views. For technical metadata and "gamified" stats (e.g., lines of code, XP points), **JetBrains Mono** provides a distinct developer-centric flavor.

Headlines should use tight letter-spacing to appear impactful and architectural. All monospaced labels should be set in uppercase when used for categorization or small UI badges to enhance the "interface" feel.

## Layout & Spacing

The layout follows a **12-column fluid grid** for desktop, collapsing to a **4-column grid** for mobile. A strict 4px baseline rhythm ensures all elements align to a technical grid, reinforcing the high-performance engineering theme.

- **Desktop:** Wide margins to allow background blurs and "floating" glass cards to breathe.
- **Mobile:** Margins tighten significantly to maximize the viewport for content. 
- **Reflow:** Components like skill-grids should wrap into single columns on mobile, maintaining their card-based glass container style.

## Elevation & Depth

Depth is communicated through **Glassmorphism** rather than traditional shadows.
- **Base Layer:** Deep Obsidian (#020617) with a subtle grain texture.
- **Mid Layer (Cards):** Translucent Slate with a 20px backdrop-blur and a 1px inner border (white at 10% opacity) to catch "light" at the edges.
- **Top Layer (Modals/Popovers):** Higher transparency, increased backdrop-blur (40px), and a subtle primary-colored drop shadow (glow) to indicate focus.

Interaction triggers a "z-axis" shift: hovering over a card increases the opacity of the inner border and adds a faint outer glow in the primary neon color.

## Shapes

The design system employs **Soft (0.25rem)** roundedness to maintain a sharp, professional edge while avoiding the clinical harshness of 0px corners. 

- **Standard Elements:** 4px radius.
- **Large Cards/Containers:** 12px (rounded-lg) to soften the glass effect.
- **Progress Bars:** Fully rounded (pill) to represent fluid movement and "filling" of experience points.

## Components

### Buttons
Primary buttons use a solid primary color background with black text for maximum contrast. Secondary buttons are "ghost" style with a 1px primary border and a subtle hover-fill.

### Chips & Badges
Used for "Tags" or "Tech Stack." These should use the `label-mono` typography and a dark semi-transparent background with a border color corresponding to the technology category (e.g., Blue for React, Purple for CSS).

### Progress Bars (XP Trackers)
The container should be a dark hollow track. The fill should be a linear gradient from Secondary to Primary color, with a "glow" tip to indicate the current progress.

### Glass Cards
The primary container for portfolio projects. Must include a 1px top-left "light" border and a 1px bottom-right "shadow" border to create a 3D glass pane effect.

### Input Fields
Dark backgrounds with no borders except for the bottom edge. On focus, the bottom edge glows primary neon blue, and the label floats upwards using the monospaced font.