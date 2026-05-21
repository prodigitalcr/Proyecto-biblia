---
name: Sacred Minimalist
colors:
  surface: '#111318'
  surface-dim: '#111318'
  surface-bright: '#37393e'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e8'
  on-surface-variant: '#c6c5d5'
  inverse-surface: '#e2e2e8'
  inverse-on-surface: '#2f3035'
  outline: '#908f9e'
  outline-variant: '#454653'
  surface-tint: '#bdc2ff'
  primary: '#bdc2ff'
  on-primary: '#131e8c'
  primary-container: '#818cf8'
  on-primary-container: '#101b8a'
  inverse-primary: '#4953bc'
  secondary: '#e9c349'
  on-secondary: '#3c2f00'
  secondary-container: '#af8d11'
  on-secondary-container: '#342800'
  tertiary: '#c1c7cf'
  on-tertiary: '#2b3137'
  tertiary-container: '#90969d'
  on-tertiary-container: '#282f35'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e0e0ff'
  primary-fixed-dim: '#bdc2ff'
  on-primary-fixed: '#000767'
  on-primary-fixed-variant: '#2f3aa3'
  secondary-fixed: '#ffe088'
  secondary-fixed-dim: '#e9c349'
  on-secondary-fixed: '#241a00'
  on-secondary-fixed-variant: '#574500'
  tertiary-fixed: '#dde3eb'
  tertiary-fixed-dim: '#c1c7cf'
  on-tertiary-fixed: '#161c22'
  on-tertiary-fixed-variant: '#41474e'
  background: '#111318'
  on-background: '#e2e2e8'
  surface-variant: '#333539'
typography:
  display-lg:
    fontFamily: Newsreader
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Newsreader
    fontSize: 36px
    fontWeight: '400'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Newsreader
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
  headline-sm:
    fontFamily: Newsreader
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 30px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 26px
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.03em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

This design system embodies a sense of quiet authority, sanctuary, and intellectual focus. It is designed for high-end editorial platforms, mindfulness applications, or premium developer tools where deep work and long-form consumption are prioritized.

The aesthetic is a fusion of **Minimalism** and **Glassmorphism**, executed with a somber, cinematic palette. It avoids the clinical coldness of pure black by utilizing a deep, atmospheric base. The emotional response is intended to be one of calm, security, and prestige. Every element is intentional, with significant negative space to allow content to "breathe" within its digital sanctuary.

## Colors

The palette is anchored by **Sanctuary Navy** (#0A0C10), providing a void-like depth that reduces eye strain. 

- **Primary (Indigo):** Used for interactive states, primary actions, and focus indicators. It provides a cool, spiritual energy.
- **Secondary (Gold):** Reserved for high-value highlights, achievement markers, or subtle branding accents. It adds a "sacred" warmth to the dark environment.
- **Neutrals:** Text utilizes **Silver Mist** (off-white) for high legibility without the harshness of pure white. Secondary text transitions into a muted slate to establish hierarchy.
- **Overlays:** Instead of solid gray fills, surfaces are built using semi-transparent white or indigo washes to create a sense of glass-like layering.

## Typography

The typographic system creates a tension between the traditional and the technical.

- **Headlines (Newsreader):** A sophisticated serif that brings a literary, authoritative character. Use "Display" sizes for editorial moments with tighter letter spacing.
- **Body (Inter):** Chosen for its exceptional readability in dark mode. The line height is intentionally generous (1.6x+) to prevent text "haloing" and ensure a comfortable reading rhythm.
- **Labels (Geist):** A monospaced/technical sans-serif used for metadata, buttons, and UI controls. It provides a precise, modern counterpoint to the organic serif headlines.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** for content-heavy sections and a **Fluid Logic** for interactive dashboards.

- **Rhythm:** An 8px linear scale is used. However, "Sacred" layouts should favor the larger end of the scale (48px+) to create an expansive, premium feel.
- **Desktop:** 12-column grid, 1200px max-width, centered. Margins should be generous to draw the eye to the center.
- **Mobile:** 4-column grid with 20px side margins. Large display type should scale down to prevent awkward wrapping while maintaining its serif elegance.

## Elevation & Depth

Depth is conveyed through **Tonal Layering** and **Backdrop Blurs** rather than traditional drop shadows.

- **The Base:** The bottom-most layer is the solid Sanctuary Navy (#0A0C10).
- **Surfaces:** Floating cards or modals use a semi-transparent white overlay (3-8% opacity) with a `backdrop-filter: blur(12px)`. This creates a "frosted glass" effect that feels integrated into the environment.
- **Outlines:** To define boundaries without adding visual weight, use 1px inner borders with a low-opacity silver or indigo tint.
- **Glow:** High-priority elements (like a selected state or gold accent) may use a soft, ultra-diffused outer glow (`spread: 20px`, `opacity: 0.1`) in the color of the accent.

## Shapes

The shape language is "Soft" yet disciplined. While the brand is minimalist, sharp corners are avoided to maintain the "sanctuary" feeling. 

- **Standard Elements:** Buttons and input fields use a 4px (0.25rem) radius.
- **Large Containers:** Cards and modals use an 8px (0.5rem) radius.
- **Interactive States:** Subtle transitions in corner radius (e.g., from 4px to 6px) can be used to signal hover states in tandem with color shifts.

## Components

- **Buttons:** Primary buttons use a solid Indigo fill with White text. Secondary buttons are "Ghost" style with a 1px Silver border and Silver text. Use Gold text only for "Premium" or "Call to Action" triggers.
- **Input Fields:** Backgrounds should be a shade darker than the surface they sit on, using a 1px Indigo border only when focused.
- **Cards:** Use the Glassmorphism approach defined in Elevation. Cards should have no shadow, relying on the 3% white overlay and 1px border to separate from the background.
- **Chips/Tags:** Small, capitalized Geist labels with a very subtle Indigo background (10% opacity) and 1px border.
- **Lists:** Separated by thin, 0.05 opacity Silver dividers. Increase vertical padding to 16px per item to maintain the "minimalist" airy feel.
- **Accents:** Use small "Gold" pips (4px circles) next to list items or headings to denote "Featured" or "New" content.