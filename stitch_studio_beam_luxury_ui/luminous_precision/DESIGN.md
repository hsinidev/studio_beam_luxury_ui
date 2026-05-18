---
name: Luminous Precision
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#d7c4ac'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#9f8e78'
  outline-variant: '#524533'
  surface-tint: '#ffba43'
  primary: '#ffd597'
  on-primary: '#432c00'
  primary-container: '#ffb000'
  on-primary-container: '#6a4700'
  inverse-primary: '#805600'
  secondary: '#c1c6d5'
  on-secondary: '#2b313c'
  secondary-container: '#414753'
  on-secondary-container: '#b0b5c3'
  tertiary: '#d3dbf3'
  on-tertiary: '#283042'
  tertiary-container: '#b7bfd6'
  on-tertiary-container: '#464e61'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffddaf'
  primary-fixed-dim: '#ffba43'
  on-primary-fixed: '#281800'
  on-primary-fixed-variant: '#614000'
  secondary-fixed: '#dde2f1'
  secondary-fixed-dim: '#c1c6d5'
  on-secondary-fixed: '#161c26'
  on-secondary-fixed-variant: '#414753'
  tertiary-fixed: '#dbe2fa'
  tertiary-fixed-dim: '#bec6dd'
  on-tertiary-fixed: '#131b2c'
  on-tertiary-fixed-variant: '#3f475a'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  headline-xl:
    fontFamily: Epilogue
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Epilogue
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Epilogue
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: '0'
  body-lg:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Space Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  spec-mono:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 24px
  margin: 64px
  container-max: 1440px
---

## Brand & Style

This design system is built for an audience that values technical mastery as much as aesthetic beauty. The brand personality is authoritative yet atmospheric, bridging the gap between a high-end fashion editorial and a precision engineering manual. 

The style utilizes **Minimalism** for layout and **Tactile** metaphors for interaction. By focusing on the "absence of light" (Midnight Blue) as a canvas, every interactive element becomes a source of illumination. The UI should evoke the feeling of standing in a darkened studio where only the necessary tools are spotlighted. Surfaces are not just containers; they are materials that react to light, using radial gradients to simulate light throw and soft amber glows to indicate activity and focus.

## Colors

The palette is intentionally restricted to amplify the impact of "light" within the interface.
- **Midnight Blue (#050A14):** The foundational void. Used for the primary background to ensure maximum contrast for light effects.
- **Warm Amber (#FFB000):** Represents the filament and the flame. This is used exclusively for interactive states, primary actions, and "active" lighting indicators.
- **Crisp White (#FFFFFF):** Used for primary typography to ensure absolute legibility against the deep background.
- **Deep Slate (#121A2B):** A secondary layer color used to create subtle depth and separation between UI sections without breaking the atmospheric darkness.

## Typography

The typographic hierarchy distinguishes between the emotional and the technical. 
- **Headings:** Use Epilogue for a bold, editorial feel. The high-contrast letterforms provide a sophisticated, luxury appearance that anchors the page.
- **Technical/Specs:** Use Space Grotesk for all body copy, data, and specifications. Its geometric, slightly mechanical nature reinforces the professional, "engineered" aspect of the hardware.
- **Tracking:** Increased letter-spacing is applied to small labels and specifications to mimic the look of etched metal equipment plates.

## Elevation & Depth

Depth in this system is conveyed through **Light Throw and Tonal Layers** rather than traditional drop shadows.
- **Base Layer:** Midnight Blue (#050A14).
- **Raised Surfaces:** Use a subtle gradient or a slightly lighter blue (#121A2B) with a 1px inner stroke in a low-opacity White to simulate a "beveled edge" of a physical device.
- **Light Accents:** Higher elevation elements (like active modals or cards) feature a soft Amber outer glow (bloom effect) with a very high blur radius (40px+) and low opacity (10-15%). 
- **Backdrop:** Use heavy background blurs (20px) on any translucent overlays to maintain the atmospheric quality while ensuring text legibility.

## Shapes

The shape language reflects professional studio gear: precise, durable, and functional.
- **Soft (Level 1):** A 0.25rem (4px) base radius is applied to buttons, inputs, and cards. This provides just enough softening to feel modern while maintaining the "hard" edge of professional aluminum and steel hardware.
- **Circular Elements:** Reserved strictly for knobs, lens representations, or status indicators to provide visual variety against the rectangular grid.

## Components

### Buttons
Interactive elements must feel like high-end hardware. 
- **Primary Action:** Solid Warm Amber background with Crisp White text. On hover, increase the "bloom" (outer glow) rather than changing the background color.
- **Secondary Action:** Midnight Blue background with a 1px Amber border. 

### Cards
Cards are treated as "light boxes." They should have a subtle radial gradient emanating from the top-left corner to simulate an off-screen light source hitting the surface. Soft Amber glows are used for "Selected" or "Active" card states.

### Inputs & Sliders
- **Inputs:** Dark backgrounds with a 1px "Deep Slate" border that glows Amber upon focus.
- **Sliders:** These are critical for a lighting brand. Use custom track styling that resembles a physical dimmer switch. The "thumb" of the slider should have a persistent Amber glow that intensifies as the value increases.

### Chips & Metadata
Use the `spec-mono` typography style for chips. They should have a background color only slightly lighter than the main background, with a high-contrast white border at 10% opacity.

### Hardware Knobs (Unique Component)
For technical adjustments (intensity, temperature), use a circular dial component with a knurled texture pattern (subtle CSS pattern) and a single Amber "indicator dot."