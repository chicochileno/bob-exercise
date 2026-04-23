---
name: Industrial Workshop System
colors:
  surface: '#0c1518'
  surface-dim: '#0c1518'
  surface-bright: '#323b3e'
  surface-container-lowest: '#070f12'
  surface-container-low: '#141d20'
  surface-container: '#182124'
  surface-container-high: '#232b2e'
  surface-container-highest: '#2d3639'
  on-surface: '#dbe4e8'
  on-surface-variant: '#c3c7ca'
  inverse-surface: '#dbe4e8'
  inverse-on-surface: '#293235'
  outline: '#8d9194'
  outline-variant: '#43474a'
  surface-tint: '#b8c9d3'
  primary: '#b8c9d3'
  on-primary: '#23333a'
  primary-container: '#37474f'
  on-primary-container: '#a4b5be'
  inverse-primary: '#506169'
  secondary: '#ffbf81'
  on-secondary: '#4a2800'
  secondary-container: '#ff9800'
  on-secondary-container: '#653900'
  tertiary: '#bbc8d0'
  on-tertiary: '#263238'
  tertiary-container: '#3a464c'
  on-tertiary-container: '#a7b4bb'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d4e5ef'
  primary-fixed-dim: '#b8c9d3'
  on-primary-fixed: '#0d1e25'
  on-primary-fixed-variant: '#394951'
  secondary-fixed: '#ffdcbe'
  secondary-fixed-dim: '#ffb870'
  on-secondary-fixed: '#2c1600'
  on-secondary-fixed-variant: '#693c00'
  tertiary-fixed: '#d7e4ec'
  tertiary-fixed-dim: '#bbc8d0'
  on-tertiary-fixed: '#111d23'
  on-tertiary-fixed-variant: '#3c494f'
  background: '#0c1518'
  on-background: '#dbe4e8'
  surface-variant: '#2d3639'
typography:
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Space Grotesk
    fontSize: 20px
    fontWeight: '500'
    lineHeight: '1.5'
    letterSpacing: '0'
  body-md:
    fontFamily: Space Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0.01em
  label-xl:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.05em
  button-text:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.02em
spacing:
  touch-target-min: 64px
  gutter: 24px
  margin: 32px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The design system is engineered for high-stakes, high-utility environments where speed, legibility, and physical interaction constraints are paramount. The brand personality is unapologetically functional, resilient, and authoritative—mirroring the heavy machinery found in a modern workshop. It evokes a sense of "tool-first" reliability, prioritizing quick scanning and error prevention under suboptimal conditions (low light, vibrations, or gloved hands).

Drawing heavily from **Brutalism** and **High-Contrast Bold** aesthetics, the style utilizes raw, unrefined structural elements. It avoids decorative fluff in favor of "caution-tape" logic: information is either critical or it is out of the way. The interface feels less like a software application and more like a physical control console.

## Colors

The palette is rooted in industrial safety standards. The primary dark gray (#37474F) serves as the "chassis," providing a low-glare background that hides digital "grime" and reduces eye strain in dim environments. Safety Orange (#FF9800) is the tactical accent, reserved strictly for primary actions, warnings, and active states to ensure they pierce through the interface.

A secondary darker surface (#263238) creates structural hierarchy, while high-visibility neutrals (#CFD8DC and #FFFFFF) ensure text remains legible against dark backgrounds. This high-contrast approach ensures that the interface remains functional even when viewed at an angle or on screens with significant glare.

## Typography

This design system utilizes **Space Grotesk** to achieve a technical, geometric feel that mimics laser-etched serial numbers and industrial labeling. Typography is treated as a structural component: it is oversized and heavy-set to ensure readability from several feet away.

Headlines use a condensed-style tight leading and heavy weights to command attention. Body text is slightly larger than standard (20px for large body) to compensate for potential visual obstructions. All labels and metadata use uppercase styling with increased letter spacing to emulate the aesthetic of stamped metal plates and industrial tags.

## Layout & Spacing

The layout is built on a rigid 8px grid, utilizing a **Fluid Grid** model that prioritizes "chunking" information into distinct modules. To accommodate "greasy fingers" and physical interaction in a workshop, the minimum touch target is strictly 64px—significantly larger than standard consumer interfaces.

Margins and gutters are wide to prevent accidental taps and to provide clear visual separation between distinct control groups. Information should be grouped into "Panel" units that stretch to fill the width of the viewport, ensuring that even on ruggedized tablets, the UI remains expansive and easy to navigate.

## Elevation & Depth

In this design system, depth is communicated through **Bold Borders** and tonal stacking rather than soft shadows. Shadows are avoided to prevent a "muddy" look on low-resolution industrial screens.

Instead, depth is created by:
1.  **Hard Outlines:** All interactive elements feature a 3px or 4px solid border.
2.  **Inset States:** To simulate a physical button being pressed, active states switch from a "protruding" border to an "inset" high-contrast fill.
3.  **Layered Z-Index:** Higher priority modals and alerts use a Safety Orange border and a darker background to "pop" forward from the base dark gray chassis.

## Shapes

The shape language is strictly **Sharp (0px)**. Elements are designed to look "machined" and "cut," reinforcing the rugged, industrial theme. Circles are reserved exclusively for status indicators (like LEDs) to create a clear visual distinction between structural containers and system health indicators.

Every button, input field, and card must have square corners. This architectural rigidity ensures that the interface feels like an extension of the physical hardware it controls.

## Components

**Buttons:**
Massive, rectangular blocks with a 4px solid border. Primary buttons use a Safety Orange fill with Black text. Secondary buttons are Dark Gray with an Orange border. The hover/tap state must trigger an immediate color inversion or a 100% brightness increase.

**Input Fields:**
Fields feature a "stamped" appearance with a thick bottom-only border or a full 3px frame. Labels are always positioned above the input, never as placeholders, to ensure context is never lost during data entry.

**Chips & Tags:**
Designed to look like physical equipment tags. They use heavy font weights and high-contrast backgrounds (Safety Orange or Bright White) to denote status or categories.

**Cards:**
Heavy-duty containers with a 2px border (#CFD8DC). Header sections within cards should be separated by a solid horizontal rule to maintain the "tabular" look of industrial logs.

**Iconography:**
Use "Heavy" or "Duo-tone" icons with thick strokes (minimum 2px). Icons must be paired with text labels whenever possible to eliminate ambiguity in high-pressure workshop environments.
