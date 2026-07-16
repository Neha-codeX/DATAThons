---
name: Kavach Sentinel
colors:
  surface: '#11131b'
  surface-dim: '#11131b'
  surface-bright: '#373942'
  surface-container-lowest: '#0c0e16'
  surface-container-low: '#1a1b23'
  surface-container: '#1e1f27'
  surface-container-high: '#282932'
  surface-container-highest: '#33343d'
  on-surface: '#e2e1ed'
  on-surface-variant: '#c4c5d7'
  inverse-surface: '#e2e1ed'
  inverse-on-surface: '#2e3039'
  outline: '#8e90a0'
  outline-variant: '#434655'
  surface-tint: '#b7c4ff'
  primary: '#b7c4ff'
  on-primary: '#002682'
  primary-container: '#1d4ed8'
  on-primary-container: '#cad3ff'
  inverse-primary: '#2151da'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#4cd7f6'
  on-tertiary: '#003640'
  tertiary-container: '#006577'
  on-tertiary-container: '#75e3ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b7c4ff'
  on-primary-fixed: '#001551'
  on-primary-fixed-variant: '#0039b5'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#acedff'
  tertiary-fixed-dim: '#4cd7f6'
  on-tertiary-fixed: '#001f26'
  on-tertiary-fixed-variant: '#004e5c'
  background: '#11131b'
  on-background: '#e2e1ed'
  surface-variant: '#33343d'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.02em
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  container-padding: 24px
  gutter: 16px
  section-gap: 40px
---

## Brand & Style
The design system embodies a high-authority, futuristic command center aesthetic tailored for state-level law enforcement intelligence. The brand personality is "Vigilant Intelligence"—combining the traditional authority of the police force with cutting-edge AI capabilities.

The visual style is a refined **Glassmorphism**, creating a sense of depth and data density without overwhelming the operator. The interface utilizes a "dark-first" architecture to minimize eye strain during long-duration surveillance and analysis shifts. The aesthetic draws from military-grade software interfaces: precise, clean, and uncompromisingly functional, yet elevated by vibrant digital accents that signify active AI processing.

## Colors
The palette is rooted in deep, nocturnal blues to establish a "Command Center" foundation. 
- **Primary & Accent Blues:** Used for primary actions, navigational cues, and brand presence.
- **Cyber Cyan & AI Purple:** Reserved for "active intelligence" states, data visualizations, and highlighting AI-driven insights.
- **Functional Colors:** High-saturation tokens for Success, Warning, and Danger are used sparingly against the dark backdrop to ensure immediate cognitive recognition of alerts.
- **Backgrounds:** `#081120` serves as the base layer, with `#0D1B2A` used for elevated container surfaces.

## Typography
This design system employs a tri-font strategy to balance impact, readability, and technical precision.
- **Space Grotesk:** Applied to all major headings and display titles. It should be set with tight tracking (letter-spacing) to reinforce the "tightly-knit" intelligence aesthetic.
- **Inter:** The workhorse for all descriptive text, reports, and administrative forms. It ensures maximum legibility across dense data views.
- **JetBrains Mono:** Exclusively for telemetry, coordinates, timestamps, and numerical statistics. The monospaced nature allows for tabular alignment of changing data points without layout shifting.

## Layout & Spacing
The system utilizes a **fluid-to-fixed grid** hybrid. 
- **Desktop:** 12-column grid with 24px gutters.
- **Tablet:** 8-column grid with 16px gutters.
- **Mobile:** 4-column grid with 16px gutters.

Spacing follows a strict 4px/8px modular scale. High-density views (dashboards) should use the 4px increments to maximize information density, while editorial or login views should use the larger 8px/16px steps to allow for "breathable" minimalism. Internal container padding is standardized at 24px for desktop cards.

## Elevation & Depth
Depth is communicated through **Glassmorphism** rather than traditional shadows.
- **Surface Layer:** Standard containers use a 6% opacity white fill with a `40px` backdrop blur. 
- **Borders:** Every glass element is defined by a "hairline" `1px` border at 8% white opacity, simulating the edge of a glass pane.
- **Z-Axis Hierarchy:** Higher elevation layers are indicated by increasing the border opacity (up to 15%) and the fill opacity (up to 10%), rather than adding drop shadows.
- **Signature Glow:** Critical active elements may have a subtle outer glow using the `Accent Blue` or `AI Purple` to suggest the element is "powered on."

## Shapes
The shape language combines geometric structural forms with ergonomic interaction points. 
- **Containers:** All dashboard cards, modal windows, and information panels use a `20px` corner radius. 
- **Interactive Elements:** Buttons, pills, and status chips use a `rounded-full` (pill) shape. This contrast between the structured "frames" of the UI and the "soft" interactive nodes makes the actionable areas of the interface immediately distinguishable from the data displays.

## Components
- **Buttons:** Primary buttons use the `Signature Gradient` with white text. Secondary buttons are ghost-style with the hairline white border.
- **Chips & Tags:** Small, pill-shaped markers using `JetBrains Mono`. For AI-generated tags, use a gradient border.
- **Cards:** The primary glass container. They should never have a solid background. Background imagery or maps should be visible through the blur.
- **Input Fields:** Semi-transparent dark fills (30% black) with the signature hairline border. The border should animate to `Cyber Cyan` on focus.
- **Status Indicators:** Use a pulsing animation for "Live" or "Active" states. 
- **Data Tables:** High-density, utilizing `JetBrains Mono` for all cell content, with row separators at 5% white opacity. No vertical borders.