---
name: GiftMate
colors:
  surface: '#fef8fa'
  surface-dim: '#ded9db'
  surface-bright: '#fef8fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f8f2f4'
  surface-container: '#f2ecee'
  surface-container-high: '#ece7e9'
  surface-container-highest: '#e7e1e3'
  on-surface: '#1d1b1d'
  on-surface-variant: '#5a4044'
  inverse-surface: '#323031'
  inverse-on-surface: '#f5eff1'
  outline: '#8e6f74'
  outline-variant: '#e3bdc3'
  surface-tint: '#bc004f'
  primary: '#b0004a'
  on-primary: '#ffffff'
  primary-container: '#d81b60'
  on-primary-container: '#fff2f3'
  inverse-primary: '#ffb2bf'
  secondary: '#843ab4'
  on-secondary: '#ffffff'
  secondary-container: '#cc80fd'
  on-secondary-container: '#580087'
  tertiary: '#735c00'
  on-tertiary: '#ffffff'
  tertiary-container: '#cca730'
  on-tertiary-container: '#4f3e00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd9de'
  primary-fixed-dim: '#ffb2bf'
  on-primary-fixed: '#3f0016'
  on-primary-fixed-variant: '#90003b'
  secondary-fixed: '#f4d9ff'
  secondary-fixed-dim: '#e4b5ff'
  on-secondary-fixed: '#2f004b'
  on-secondary-fixed-variant: '#6a1b9a'
  tertiary-fixed: '#ffe088'
  tertiary-fixed-dim: '#e9c349'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#574500'
  background: '#fef8fa'
  on-background: '#1d1b1d'
  surface-variant: '#e7e1e3'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
  title-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  base: 8px
  container-margin: 24px
  gutter: 16px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is centered on the concept of "The Art of Giving." It targets a discerning audience looking for thoughtful, high-end gift curation. The aesthetic blends **Modern Minimalism** with **Glassmorphism**, creating a digital experience that feels as premium as a physical gift box. 

The emotional response should be one of warmth, anticipation, and sophistication. To achieve this, the UI utilizes generous white space, soft-focus background blurs, and elegant transitions that mimic the unwrapping of a luxury item. Surfaces are layered to create a sense of depth and tactile quality without feeling heavy or industrial.

## Colors

The palette is anchored in a "Premium Rose" (Primary) and "Deep Amethyst" (Secondary), providing a rich, emotive foundation. "Champagne Gold" (Tertiary) is used sparingly for accents, iconography, and luxury indicators to denote high-value items or "editor's choice" selections.

The background is not a pure white but a very soft, warm neutral (`#FDF7F9`) to maintain an inviting atmosphere. Gradients should be used as subtle background washes—blending soft pinks and purples—to support the glassmorphic surfaces. Ensure a high contrast ratio for all text over these gradients by using a deep charcoal for body copy.

## Typography

This design system uses a high-contrast typographic pairing to signal luxury. **Playfair Display** is the voice of the brand, used for editorial headlines and featured gift titles. It should always be set with slightly tighter letter-spacing in larger formats.

**Inter** provides the functional backbone. It is used for all UI elements, descriptions, and metadata to ensure maximum readability on mobile devices. For secondary information or "eyebrow" text above headlines, use `label-caps` to create a structured, organized feel within the fluid, emotional layout.

## Layout & Spacing

This design system follows a **mobile-first fluid grid**. On mobile, use a 2-column or 1-column layout with 24px side margins to allow the content "room to breathe," reflecting the premium nature of the brand. 

For desktop, transition to a 12-column fixed grid (max-width 1200px). The spacing rhythm is based on an 8px scale, but vertical "stacks" should be generous (48px+) between major sections to prevent a cluttered, "discount" marketplace appearance. Use dynamic padding for glassmorphic cards, ensuring internal content never feels cramped against the rounded edges.

## Elevation & Depth

Depth is primarily communicated through **Glassmorphism** and soft, colored shadows. 

1.  **Glass Surfaces:** Use backdrop-filter (blur: 20px) with a semi-transparent white fill (opacity: 60-80%). Apply a very thin, 1px inner border in pure white (opacity: 30%) to simulate the edge of a glass pane.
2.  **Shadows:** Avoid pure black shadows. Use a "tinted ambient shadow" using the secondary purple or primary pink at 5-10% opacity, with a high blur radius (30px+) and a slight Y-offset to make cards feel like they are floating over the background gradients.
3.  **Imagery:** High-quality photography should have its own slight elevation, appearing "set into" the glass cards or floating slightly above them.

## Shapes

The shape language is extremely soft and approachable. The design system utilizes **Pill-shaped (3)** logic for almost all interactive and container elements. 

- **Primary Cards:** Use `rounded-3xl` (24px or 32px depending on size) to create a friendly, organic feel.
- **Buttons and Inputs:** Use full-radius "pill" shapes. 
- **Icons:** Should feature rounded terminals and soft corners to match the parent containers.
- **Images:** All gift imagery must feature a minimum 16px corner radius; never use sharp 0px corners for visual assets.

## Components

### Buttons
Primary buttons use a subtle linear gradient from Primary Pink to Secondary Purple (45-degree angle). Text is white, Medium weight. Hover states should slightly increase the shadow spread rather than changing the color drastically. Secondary buttons use the "Glass" style with a gold or purple outline.

### Glass Cards
The signature component. Used for gift products. Content includes a top-aligned image, followed by a headline in Playfair Display, and a price tag in Inter Bold. The card background must use the backdrop-blur effect.

### Chips/Tags
Small pill-shaped elements for "Occasions" or "Recipient Type." Use a soft pastel fill (`accent_pink_soft`) with Primary Pink text. No borders.

### Input Fields
Inputs are pill-shaped with a soft neutral fill and a 1px border that glows (Secondary Purple) when focused. Labels stay outside the field in `label-caps` style.

### Search & Filtering
The search bar is a prominent glassmorphic element at the top of the discovery feed, utilizing a "Champagne Gold" search icon to denote the "discovery" or "treasure hunt" aspect of the app.