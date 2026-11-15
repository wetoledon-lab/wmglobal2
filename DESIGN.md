---
name: Industrial Integrity
colors:
  surface: '#f7fafc'
  surface-dim: '#d7dadc'
  surface-bright: '#f7fafc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f6'
  surface-container: '#ebeef0'
  surface-container-high: '#e5e9eb'
  surface-container-highest: '#e0e3e5'
  on-surface: '#181c1e'
  on-surface-variant: '#44474c'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eef1f3'
  outline: '#74777d'
  outline-variant: '#c4c6cd'
  surface-tint: '#4f6074'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#0b1d2e'
  on-primary-container: '#74859b'
  inverse-primary: '#b7c8df'
  secondary: '#226488'
  on-secondary: '#ffffff'
  secondary-container: '#9bd6ff'
  on-secondary-container: '#185e81'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#181c21'
  on-tertiary-container: '#81848a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d3e4fc'
  primary-fixed-dim: '#b7c8df'
  on-primary-fixed: '#0b1d2e'
  on-primary-fixed-variant: '#38485b'
  secondary-fixed: '#c7e7ff'
  secondary-fixed-dim: '#93cdf6'
  on-secondary-fixed: '#001e2e'
  on-secondary-fixed-variant: '#004c6d'
  tertiary-fixed: '#e0e2e9'
  tertiary-fixed-dim: '#c4c6cd'
  on-tertiary-fixed: '#181c21'
  on-tertiary-fixed-variant: '#44474c'
  background: '#f7fafc'
  on-background: '#181c1e'
  surface-variant: '#e0e3e5'
  surface-glass: rgba(255, 255, 255, 0.7)
  border-technical: '#e5e9eb'
  industrial-navy-container: '#1a2b3c'
  on-surface-muted: '#44474c'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: '0'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  button:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  gutter-desktop: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  container-max: 1280px
  section-gap: 80px
---

## Brand & Style

This design system is engineered for high-performance SPAs in the energy and construction sectors. The brand personality is authoritative, precise, and structurally sound, evoking the reliability of heavy engineering. 

The aesthetic is a hybrid of **Industrial Minimalism** and **Glassmorphism**. It utilizes a "precision-engineered" look characterized by generous white space, sharp execution, and technical clarity. While the core is rooted in corporate stability, the UI incorporates modern SPA elements like translucent overlays and smooth transitions to signify a forward-thinking, data-driven platform. The result is a UI that feels like a sophisticated digital control room: institutional strength paired with operational efficiency.

## Colors

The palette is derived from heavy industry, maritime engineering, and architectural blueprints.

- **Primary (Industrial Navy):** The anchor of the system. Used for high-level navigation, primary actions, and brand-heavy components. It represents depth and corporate authority.
- **Secondary (Technical Blue):** Used for iconography, interactive states, and progress indicators. It provides a modern, high-tech contrast to the navy.
- **Tertiary (Technical Gray):** A cool, metallic neutral used for borders, secondary labels, and disabled states to reinforce the "steel" aesthetic.
- **Neutral (Structural White/Gray):** Backgrounds utilize a crisp `#FFFFFF` for content areas and `#F7FAFC` for page scaffolding.

For the SPA experience, **Glassmorphism** is applied using `surface-glass` with a `backdrop-filter: blur(12px)` on sticky headers and floating sidebars to maintain context during scroll.

## Typography

Typography focuses on legibility and technical precision.

- **Headlines:** Hanken Grotesk provides a sharp, contemporary corporate look. Large sizes use tight letter-spacing to feel "constructed" and impactful.
- **Body:** Inter is the workhorse for technical descriptions, ensuring maximum readability across varying pixel densities.
- **Labels & Data:** JetBrains Mono is utilized for technical data points, serial numbers, and system statuses. This monospaced choice evokes engineering accuracy and data-driven reliability.
- **SPA Motion:** Type transitions during view changes should use a subtle vertical slide (4px) combined with an opacity fade to maintain a high-performance feel.

## Layout & Spacing

The layout utilizes a **Fixed Grid** model for desktop to maintain a controlled, professional environment, transitioning to a fluid model for mobile.

- **Grid System:** A 12-column grid is standard. SPA views should align technical components strictly to the grid to reinforce the "structured" brand nature.
- **SPA Fluidity:** Use `scroll-behavior: smooth` for internal linking. To support high-performance interactions, layout shifts must be minimized by reserving space for dynamic content.
- **Breakpoints:**
  - **Mobile:** < 768px (1-column, 20px margins).
  - **Tablet:** 768px - 1024px (6-column, 32px margins).
  - **Desktop:** > 1024px (12-column, 64px margins, 1280px max-container).
- **Rhythm:** An 8px base unit (linear scale) governs all padding and margins to ensure a mathematical, "engineered" balance.

## Elevation & Depth

To maintain a "solid" industrial feel, this system avoids traditional, heavy shadows.

- **Tonal Layering:** Depth is primarily created by stacking surfaces. White containers are placed on `#F7FAFC` backgrounds, separated by 1px `border-technical` outlines.
- **SPA Glassmorphism:** For floating elements like modal overlays or dropdown menus, use a semi-transparent white (`surface-glass`) with a backdrop blur. This allows the user to see the "infrastructure" of the app underneath the current interaction.
- **Low-Contrast Outlines:** Mimic technical drawings by using thin, high-precision borders instead of diffused shadows.
- **Subtle Interaction Shadows:** A very tight, low-opacity shadow (blur: 4px, opacity: 0.05) is permitted only on "lifted" states, such as a card being hovered in a dashboard.

## Shapes

The shape language is "Soft-Industrial." Geometry is primarily rectangular and architectural, avoiding organic or pill-shaped curves.

- **Component Radius:** A strict 4px (0.25rem) radius is applied to buttons and input fields to soften the industrial edge just enough for digital comfort.
- **Container Radius:** Larger containers and cards use 8px (0.5rem) to provide a clear framing of content.
- **Strictness:** Do not use full-round (pill) buttons. The UI must feel like it was assembled from precision-cut components.

## Components

### Buttons
- **Primary:** Industrial Navy background, white text, 4px radius. Use a subtle brightness shift (10%) on hover.
- **Secondary:** Technical Blue background. Used for supporting actions like "View Specs."
- **Ghost/Glass:** `surface-glass` with a 1px border for tertiary actions on dark backgrounds.

### Cards & Containers
- White background, 1px `#E5E9EB` border, 8px radius. 
- **Accent:** Incorporate a 4px solid Industrial Navy left-border on header cards to denote administrative hierarchy.

### Input Fields
- Boxy and stable. Use `#FFFFFF` backgrounds with a 1px Technical Gray border. Upon focus, the border transitions to Technical Blue with a subtle 2px outer glow of the same color. Labels use `body-sm` and are always visible above the field.

### Status Indicators
- Use the `label-caps` (JetBrains Mono) font. 
- **Success/Active:** Muted Sage Green.
- **Warning/Pending:** Industrial Amber.
- **Danger/Offline:** Technical Red.
- Keep colors desaturated to maintain a professional, grounded aesthetic.

### Industrial Icons
- 2px stroke weight, non-filled (outline) style. Icons should be sized to a 24px bounding box and colored Technical Blue to differentiate them from primary text content.