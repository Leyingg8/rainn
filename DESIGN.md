---
name: Apex Shield
colors:
  surface: '#f7fafe'
  surface-dim: '#d7dade'
  surface-bright: '#f7fafe'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f8'
  surface-container: '#ebeef2'
  surface-container-high: '#e5e8ec'
  surface-container-highest: '#e0e3e7'
  on-surface: '#181c1f'
  on-surface-variant: '#43474f'
  inverse-surface: '#2d3134'
  inverse-on-surface: '#eef1f5'
  outline: '#737780'
  outline-variant: '#c3c6d0'
  surface-tint: '#3d5f90'
  primary: '#001c3b'
  on-primary: '#ffffff'
  primary-container: '#02315f'
  on-primary-container: '#789ace'
  inverse-primary: '#a6c8ff'
  secondary: '#0060a9'
  on-secondary: '#ffffff'
  secondary-container: '#58a6fe'
  on-secondary-container: '#003b6a'
  tertiary: '#2a1800'
  on-tertiary: '#ffffff'
  tertiary-container: '#462b00'
  on-tertiary-container: '#d18900'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d5e3ff'
  primary-fixed-dim: '#a6c8ff'
  on-primary-fixed: '#001c3b'
  on-primary-fixed-variant: '#224776'
  secondary-fixed: '#d3e4ff'
  secondary-fixed-dim: '#a2c9ff'
  on-secondary-fixed: '#001c38'
  on-secondary-fixed-variant: '#004881'
  tertiary-fixed: '#ffddb5'
  tertiary-fixed-dim: '#ffb956'
  on-tertiary-fixed: '#2a1800'
  on-tertiary-fixed-variant: '#643f00'
  background: '#f7fafe'
  on-background: '#181c1f'
  surface-variant: '#e0e3e7'
  text-slate: '#2B3440'
  surface-pure: '#FFFFFF'
  border-subtle: '#DCE3EC'
  success-emerald: '#15803D'
  alert-crimson: '#B91C1C'
typography:
  headline-hero:
    fontFamily: Montserrat
    fontSize: 56px
    fontWeight: '800'
    lineHeight: 64px
    letterSpacing: -0.02em
  headline-hero-mobile:
    fontFamily: Montserrat
    fontSize: 36px
    fontWeight: '800'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-xl:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.015em
  headline-xl-mobile:
    fontFamily: Montserrat
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Montserrat
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-xl:
    fontFamily: Open Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Open Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Open Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Montserrat
    fontSize: 15px
    fontWeight: '700'
    lineHeight: 20px
    letterSpacing: 0.03em
  label-md:
    fontFamily: Montserrat
    fontSize: 13px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Montserrat
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.08em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-mobile: 1rem
  margin: 2.5rem
  margin-mobile: 1.25rem
  margin-desktop-max: 5rem
  space-2xs: 0.25rem
  space-xs: 0.5rem
  space-sm: 0.75rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
  space-2xl: 4rem
  space-3xl: 6rem
---

## Brand & Style

This design system establishes an architectural, steadfast, and weather-resilient identity tailored for residential and commercial property restoration. The brand personality balances unyielding structural authority with approachable optimism: steadfast protection against severe storms combined with the clarity and warmth of post-storm renewal. 

Targeted at homeowners facing urgent damage and property managers seeking proactive long-term maintenance, the interface projects dependability, speed, and precision craftsmanship. The aesthetic leans into Modern Corporate infused with Architectural Precision: crisp angled roofline geometry, sharp cutaway diagonals, generous breathable whitespaces reminiscent of open skies, and subtle thematic references to precipitation barriers and solar warmth. The design eschews generic contractor tropes in favor of an engineered, credential-first standard that breeds consumer trust.

## Colors

The palette balances environmental defense and post-storm clarity:
- **Navy (`#02315F`)**: The commanding structural baseline. Used for high-level headers, primary brand anchoring, master navigation surfaces, and primary trust elements.
- **Sky Blue (`#0172C6`)**: The dynamic atmospheric tone. Applied across secondary links, interactive hover indicators, icon backplates, and progress trackers.
- **Sun Gold (`#F0A81C`)**: The urgent warmth and conversion driver. Reserved strictly for primary calls-to-action (e.g., "Schedule Inspection", "Emergency Dispatch"), the mobile call bar, and two or three single-word highlights. All other icon backplates, labels, and decorative accents use Sky Blue or Inverse Primary (`#A6C8FF`) so the gold never reads as decorative filler.
- **Cloud (`#F3F6FA`)**: The expansive neutral canvas. Replaces sterile cool whites across section backdrops to diminish eye strain and create tactile separation between nested cards.
- **Slate (`#2B3440`)**: Engineered for WCAG AAA reading compliance. Applied to body typography, deep metadata, and structural outlines.

### Architectural Rules
- High-priority conversion flows require high contrast: pair Sun Gold with Navy text for accessibility compliance (`#02315F` on `#F0A81C` measures about 6.4:1, hover `#D89400` about 5.1:1).
- Avoid large flood-fills of Sun Gold; keep it hyper-focused on high-intent actions. Decorative use of the warm accent was removed in the professional color pass: backgrounds shifted to Sky/Crimson, and warm radial glows were retinted cool.

## Typography

The type system blends the geometric authority of Montserrat with the human clarity of Open Sans:
- **Montserrat (Display & Headings)**: Provides bold structural impact reminiscent of structural engineering and modern architectural signage. Used for all headings, statistical metrics, key price indicators, and high-impact calls to action.
- **Open Sans (Reading & Interaction)**: Delivers neutral, highly legible rhythm across body narratives, customer disclaimers, insurance process descriptions, and input forms.
- **Uppercase Labels**: Category headers, cert badges, and kicker titles over hero elements use `label-caps` in uppercase styling to reinforce industrial durability.

## Layout & Spacing

The layout model utilizes a standard 12-column fluid grid system on desktop (max content boundary: 1280px) and collapses to 6 columns on tablet and 4 columns on mobile. 

### Rhythmic Rules
- **Roofline Angles & Geometry**: Visual section dividers and hero containers can leverage a precise 4-degree or 6-degree clipped diagonal cut (`clip-path: polygon(0 0, 100% 0, 100% calc(100% - 2.5vw), 0 100%)`), giving the appearance of an engineered gable roofline separating atmospheric content bands.
- **Vertical Modulation**: Section transitions alternate between Cloud (`#F3F6FA`) and Pure White (`#FFFFFF`) with generous `space-3xl` breathing room to project institutional scale and transparency.
- **Card Clustering**: Component clusters, such as service offering cards and multi-step damage claim workflows, preserve clean separation with `space-lg` gutters and `space-xl` block padding.

## Elevation & Depth

Visual depth is achieved through layered structural planes rather than deep drop shadows, matching the physical nature of multi-layered roofing systems:

1. **Ground Tier (Surface)**: Cloud (`#F3F6FA`) handles standard page canvases, providing a foundation against which white architectural cards rise.
2. **Level 1 (Stacked Deck)**: Pure White surfaces (`#FFFFFF`) framed by a subtle weather-seal border (`1px solid #DCE3EC`) and an ambient, blue-tinted drop shadow: `0 4px 16px -2px rgba(2, 49, 95, 0.06)`. Used for standard structural cards, inspection forms, and service panels.
3. **Level 2 (Active Shingle)**: Hovered state or elevated interaction cards. The ambient drop shadow expands: `0 12px 32px -4px rgba(2, 49, 95, 0.12)`, accented with a left-edge 4px Sky Blue indicator stripe to denote interactive readiness.
4. **Level 3 (Overlays & Emergency Prompts)**: Popovers, fast contact panels, and floating emergency call bars use `0 20px 40px -8px rgba(2, 49, 95, 0.20)` with high-contrast borders.

## Shapes

A soft-cornered geometry (Level 1: 0.25rem / 4px base radius) is paired with clean architectural angles. This subtle curvature prevents UI surfaces from feeling abrasive while retaining the crispness of blueprints and construction framing. 

- **Cards & Modules**: 4px base border radius. On primary feature banners, the top-right corner can be paired with an angled roofline clip or an asymmetric 16px radius to echo the upward pitch of a roof.
- **Buttons & Chips**: Formed with 4px to 6px radii to maintain a solid, tool-like feel. Pill shapes are restricted only to live status indicators (e.g., "Active Storm Alert").
- **Visual Motifs**: Circular icons mimic the Sun Gold motif, while directional water-repellent chevron arrows reflect rainfall runoff angles.

## Components

### Buttons
- **Primary CTA (Sun Gold)**: Background `#F0A81C`, text `#02315F`, font `label-lg`, radius 4px, height 48px, horizontal padding `space-xl`. Hover transitions to `#D89400` with subtle elevation. Always represents key conversions (e.g., "Claim Free Inspection").
- **Secondary Action (Navy)**: Background `#02315F`, text `#FFFFFF`, hover `#012344`. For institutional actions (e.g., "Explore Warranty", "View Certifications").
- **Outline / Rain Accent**: Background transparent, border `2px solid #0172C6`, text `#0172C6`. Hover shifts to `#0172C6` with white text.

### Inspection & Feature Cards
- Constructed on Pure White (`#FFFFFF`) with a 1px `#DCE3EC` border and 4px radius. 
- Headers feature Navy (`#02315F`) with micro-icons encased in a 10% opacity Sky Blue rounded container.
- Hover interactions raise elevation from Level 1 to Level 2 and expose an angled 4px Sky Blue left-border highlight.

### Certification & Badge Chips
- Compact pills designed for trust signifiers (e.g., "IICRC Certified", "Licensed & Insured").
- Cloud `#F3F6FA` fill, Navy `#02315F` typography (`label-caps`), bordered by `#DCE3EC`. When indicating storm-response status, switch to Sun Gold outline with gold-tinted fill.

### Form Inputs
- 48px height, 4px radius, Pure White background, framed by `1.5px solid #DCE3EC`.
- Text typed in Slate (`#2B3440`). Focused state transitions the border to Sky Blue (`#0172C6`) with an ambient 3px outer ring tinted to `rgba(1, 114, 198, 0.15)`. Labels use `label-md` in Navy.

### Emergency Dispatch Alert Bar
- Pinned banner at layout apex: Deep Navy background (`#02315F`) featuring a Sky Blue callout marker, a Sun Gold phone link, and bold uppercase status text (`label-caps`).