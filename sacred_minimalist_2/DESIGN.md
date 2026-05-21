---
name: Sacred Minimalist
colors:
  surface: '#fff8f5'
  surface-dim: '#f3d4bf'
  surface-bright: '#fff8f5'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff1e9'
  surface-container: '#ffeadc'
  surface-container-high: '#ffe3d0'
  surface-container-highest: '#fcddc7'
  on-surface: '#28180b'
  on-surface-variant: '#464555'
  inverse-surface: '#3f2d1e'
  inverse-on-surface: '#ffede3'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#545f73'
  on-secondary: '#ffffff'
  secondary-container: '#d5e0f8'
  on-secondary-container: '#586377'
  tertiary: '#4a4842'
  on-tertiary: '#ffffff'
  tertiary-container: '#626059'
  on-tertiary-container: '#dedbd2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#d8e3fb'
  secondary-fixed-dim: '#bcc7de'
  on-secondary-fixed: '#111c2d'
  on-secondary-fixed-variant: '#3c475a'
  tertiary-fixed: '#e6e2d9'
  tertiary-fixed-dim: '#c9c6be'
  on-tertiary-fixed: '#1c1c17'
  on-tertiary-fixed-variant: '#484741'
  background: '#fff8f5'
  on-background: '#28180b'
  surface-variant: '#fcddc7'
  sanctuary-navy: '#0f172a'
  linen-light: '#fdf9f0'
  linen-sepia: '#f4ecd8'
  indigo-accent: '#6366f1'
typography:
  scripture-display:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  scripture-display-mobile:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  scripture-body:
    fontFamily: Literata
    fontSize: 20px
    fontWeight: '400'
    lineHeight: '1.7'
  scripture-verse-num:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.05em
  ui-header:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: -0.01em
  ui-label:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '800'
    lineHeight: '1'
    letterSpacing: 0.15em
  ui-button:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
  ui-body:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  page-margin-mobile: 1.5rem
  page-margin-desktop: 4rem
  reader-max-width: 720px
  gutter: 1rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
  stack-lg: 3rem
---

## Brand & Style

This design system embodies the "Sacred Minimalist" aesthetic—a bridge between the timeless reverence of the Reina Valera 1960 scriptures and modern digital clarity. The brand personality is serene, scholarly, and intentional. It aims to evoke a sense of "digital sanctuary," removing the noise of the modern world to allow the Word to remain the sole focus.

The visual style leans into **Minimalism** enriched with **Tactile** and **Glassmorphic** layers. It utilizes heavy whitespace to create "breathing room" for contemplation. The interface avoids aggressive digital tropes, opting instead for soft textures, organic roundedness, and subtle depth to make the app feel like a physical, premium object held in the hand.

## Colors

The "Deep Sanctuary" palette is designed for long-form spiritual immersion. 

- **Primary (Indigo):** Used sparingly for meaningful actions, selection highlights, and active states. It represents the "modern" bridge to the scripture.
- **Secondary (Deep Navy):** Provides a grounding, authoritative weight for headers and structural elements.
- **Tertiary (Linen/Sepia):** The primary canvas for reading. This soft, off-white tone reduces eye strain and mimics the warmth of physical parchment.
- **Neutral (Earth Tone):** A deep brown-gray used for body text in the sepia mode to maintain a soft contrast ratio that is more comfortable than pure black on white.

The design system defaults to a "Linen" light mode but transitions seamlessly into a true dark mode (using `sanctuary-navy`) for evening devotion.

## Typography

Typography is the cornerstone of this design system. We employ a dual-system approach:

1.  **Scripture Serif:** `Literata` (or `Crimson Pro`) is used for the Word. It is a high-readability serif designed for digital screens, offering a warm, bookish feel. `Playfair Display` is reserved for book titles and major section headers to provide editorial elegance.
2.  **UI Sans:** `Inter` handles all functional requirements. It is used for navigation, verse numbers, labels, and settings to provide a clean, modern counterpoint to the traditional serif text.

**Hierarchy Rules:**
- Scripture text should always have a `leading-relaxed` (1.7x) line height to ensure the eye doesn't tire during long chapters.
- Verse numbers are treated as UI elements: small, bold, and anchored to the `Inter` family to keep them distinct from the narrative text.

## Layout & Spacing

The layout philosophy follows a **Fixed-Width Reader** model centered within a fluid container. This ensures that even on large tablets or foldable screens, line lengths remain optimal for reading (between 60-75 characters).

**Grid & Rhythm:**
- **Reader Column:** Max-width of `720px`. Content is centered with generous side margins to create a "focus zone."
- **Vertical Rhythm:** We use a `stack` scale based on `1rem`. Scripture paragraphs are separated by `stack-md`, while new chapters or books use `stack-lg`.
- **Mobile Reflow:** On mobile, margins shrink to `1.5rem` to maximize screen real estate, while maintaining a single-column flow. Interactive elements like the "Floating Action Button" (for search or navigation) sit in the safe areas at the bottom of the screen.

## Elevation & Depth

To maintain the "Sacred" aesthetic, depth is used subtly and meaningfully. We avoid harsh shadows in favor of **Tonal Layers** and **Glassmorphism**.

- **Surfaces:** The primary reading surface is flat. Secondary panels (like a verse study drawer or book selector) use a "Linen-Sepia" tone to distinguish themselves.
- **Glassmorphism:** Bottom navigation bars and floating control widgets (font sizing, theme toggles) use a high-blur backdrop filter (glass effect) with a very thin white or navy border (10% opacity). This allows the scripture to "glow" through the controls without obstructing the view.
- **Ambient Shadows:** Only used for floating buttons or active cards. Shadows should be ultra-diffused (32px+ blur) with a tint of the `primary` color at 5-10% opacity.

## Shapes

The shape language is **Organic and Rounded**. We move away from sharp, technical corners to evoke the feeling of smooth river stones or high-end stationery.

- **UI Elements:** Buttons and input fields use `rounded-lg` (1rem).
- **Containers:** Cards and bottom sheets use `rounded-xl` (1.5rem) or `rounded-2xl` (3rem) for a friendly, soft appearance.
- **Selection:** When a verse is selected, the highlight should have soft, rounded terminals rather than hard blocks.

## Components

### Buttons
Primary buttons are pill-shaped (`rounded-full`) using the `indigo-600` background. Secondary buttons use a transparent background with a soft `linen-sepia` border.

### Scripture Chips
Used for chapter numbers or cross-references. These are small, non-intrusive capsules with high-tracking `Inter` labels.

### The Reader Card
The main scripture container. It features no borders or shadows by default, appearing as a continuous scroll of paper. When "Focus Mode" is active, all other UI components fade to 20% opacity.

### Floating Controls
A glassmorphic "pill" that sits at the bottom of the viewport. It houses font-size adjustment, theme switching, and audio playback. It uses a `backdrop-blur-md` and a subtle 1px border.

### Verse Selection
Selected verses are highlighted with a soft `indigo-accent` at 10% opacity with 4px rounded corners at the start and end of the selection block.

### Search Bar
A deep-inset field with `rounded-xl` corners, using a search icon from a thin-stroke library to maintain the minimalist weight.