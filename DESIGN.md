---
name: Obsidian Flux
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#d8ffe7'
  on-tertiary: '#003824'
  tertiary-container: '#65f2b5'
  on-tertiary-container: '#006d4a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
  obsidian-deep: '#050505'
  charcoal-surface: '#1A1A1A'
  neon-cyan: '#00F0FF'
  electric-violet: '#8B5CF6'
  soft-emerald: '#10B981'
  glass-stroke: rgba(255, 255, 255, 0.12)
typography:
  headline-xl:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  code-block:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.7'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  section-gap: 120px
---

## Brand & Style

This design system targets a high-performance, technical audience, specifically showcasing the expertise of a Senior Java Developer. The brand personality is rooted in precision, modern engineering, and creative problem-solving. It utilizes a **Glassmorphic** and **Modern Dark-Mode** aesthetic to create an environment that feels both sophisticated and high-tech.

The visual narrative centers on "depth through transparency." By layering translucent surfaces over deep, obsidian-toned backgrounds and accented with neon light sources, the UI mimics a futuristic heads-up display (HUD). The emotional response should be one of reliability (through structured layout) and cutting-edge innovation (through vibrant accents and glass effects).

Key stylistic pillars:
- **Depth:** Multi-layered backdrop blurs that create a sense of physical space.
- **Luminance:** Neon accents used sparingly to guide the eye toward critical technical achievements and CTAs.
- **Clarity:** Sharp, high-contrast typography that ensures technical documentation and code snippets are highly legible.

## Colors

The palette is anchored in a monochromatic dark spectrum, ranging from absolute black (`#050505`) to a deep charcoal (`#1A1A1A`). This provides the necessary "obsidian" canvas for glassmorphism to thrive. 

Vibrant accents—**Neon Cyan**, **Electric Violet**, and **Soft Emerald**—are used to categorize different aspects of the portfolio:
- **Neon Cyan (Primary):** Interactive elements, primary actions, and Java-related technical highlights.
- **Electric Violet (Secondary):** Architecture patterns, backend logic, and complex system diagrams.
- **Soft Emerald (Tertiary):** Success states, performance metrics, and "live" project indicators.

Transparency is a functional requirement: surfaces should use an 80% opacity fill of the surface color combined with a `backdrop-filter: blur(12px)`.

## Typography

The typography system uses a tri-font approach to balance editorial impact with technical utility. 

- **Geist** handles the heavy lifting for headlines, providing a sharp, geometric look that feels engineered. 
- **Inter** is used for body copy to ensure maximum readability during long-form project descriptions. 
- **JetBrains Mono** is reserved for labels, metadata, and code snippets, grounding the design in the developer's native environment.

Headlines should utilize tight letter-spacing to feel more "locked-in" and architectural. For mobile, headline sizes scale down significantly to maintain the grid's integrity.

## Layout & Spacing

The layout follows a **Fixed Grid** model on desktop (12 columns) and a **Fluid Grid** on mobile (4 columns). The rhythm is strictly 8px-based to mirror the precision of backend development.

- **Desktop:** A centered 1200px container with wide 48px margins to allow for "floating" glass elements that may slightly bleed outside the primary container.
- **Sectioning:** Large vertical gaps (120px) create breathing room between distinct portfolio sections (e.g., from "Experience" to "Open Source").
- **Reflow:** On tablet, the 12-column grid collapses to 8, and margins reduce to 32px. Mobile uses a singular column with heavy focus on vertical stacking of translucent cards.

## Elevation & Depth

Depth is achieved through **Glassmorphism** rather than traditional shadows. 

1.  **Base Layer:** Solid `#050505` background.
2.  **Middle Layer (Cards):** Background color of `rgba(26, 26, 26, 0.6)` with a `backdrop-filter: blur(16px)`. A 1px border using `glass-stroke` defines the edge.
3.  **Top Layer (Floating Actions):** `rgba(255, 255, 255, 0.05)` fill with a more intense `blur(24px)` and a subtle outer glow using the `primary-color` at 10% opacity.

Instead of shadows, use "Linear Light" strokes—thin gradients on the top-left borders of elements—to simulate a light source from the top-left corner.

## Shapes

The shape language is "Softly Geometric." Elements use a **0.5rem (8px)** base radius to feel modern and approachable without losing the professional, "square" feel of an IDE. 

- Large containers and cards use **1rem**.
- Buttons and interactive chips use **0.5rem**.
- Avoid pill-shaped buttons; maintaining a rectangular-but-soft silhouette reinforces the systematic nature of the developer's work.

## Components

### Translucent Cards
The core container for project details. Must feature the `backdrop-blur`, a subtle `glass-stroke` border, and a faint gradient background (top-left to bottom-right) using the primary accent color at 5% opacity.

### Floating Action Buttons (FAB)
Circular or soft-square buttons that float in the bottom-right. These should have a vibrant `neon-cyan` background with a high-contrast black icon to signal primary navigation or contact actions.

### Sleek Navigation
A top-docked, "detached" navigation bar. It should be a floating glass capsule with `backdrop-filter: blur(20px)`. Active links are highlighted with a tiny `electric-violet` dot underneath, rather than a full background change.

### Input Fields & Code Blocks
Input fields use a dark charcoal background with a 1px `neon-cyan` border on focus. Code blocks should mimic the "Carbon" aesthetic: a dark container with a header bar featuring three colored window controls (red, yellow, green) to evoke a terminal/IDE feel.

### Status Chips
Small, low-profile badges used for "Tech Stack" tags. They use a semi-transparent version of the accent colors (e.g., 10% Cyan fill with 100% Cyan text) to maintain hierarchy without cluttering the UI.