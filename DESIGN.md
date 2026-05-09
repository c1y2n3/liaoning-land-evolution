---
name: Liaoning Land Evolution
colors:
  surface: '#00161f'
  surface-dim: '#00161f'
  surface-bright: '#043e52'
  surface-container-lowest: '#001018'
  surface-container-low: '#001f2a'
  surface-container: '#002330'
  surface-container-high: '#002e3e'
  surface-container-highest: '#003a4c'
  on-surface: '#bee9ff'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#bee9ff'
  inverse-on-surface: '#003546'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#a6e6ff'
  on-secondary: '#003543'
  secondary-container: '#14d1ff'
  on-secondary-container: '#00566b'
  tertiary: '#ffffff'
  on-tertiary: '#412d00'
  tertiary-container: '#ffdea6'
  on-tertiary-container: '#815e11'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#b7eaff'
  secondary-fixed-dim: '#4cd6ff'
  on-secondary-fixed: '#001f28'
  on-secondary-fixed-variant: '#004e60'
  tertiary-fixed: '#ffdea6'
  tertiary-fixed-dim: '#edc06b'
  on-tertiary-fixed: '#271900'
  on-tertiary-fixed-variant: '#5e4200'
  background: '#00161f'
  on-background: '#bee9ff'
  surface-variant: '#003a4c'
typography:
  display-title:
    fontFamily: Noto Serif
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  city-heading:
    fontFamily: Noto Serif
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  body-elegant:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '300'
    lineHeight: '1.8'
    letterSpacing: 0.01em
  metric-value:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: -0.01em
  metric-label:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.1em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  safe-margin: 48px
  gutter: 24px
  panel-padding: 32px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The brand personality of this design system is authoritative, visionary, and cinematic. It bridges the gap between complex geospatial data and high-end editorial storytelling. The target audience—provincial planners and investors—should feel they are interacting with a premium intelligence tool rather than a standard utility dashboard.

The style is a synthesis of **Minimalism** and **Glassmorphism**, treated with the spatial discipline of a luxury magazine. It avoids the cluttered "NASA-style" dashboard aesthetic in favor of an airy, "floating" interface that prioritizes the GIS map as the primary hero. The experience should feel like a digital exhibition of Liaoning's economic evolution: clean, tech-forward, and deeply immersive.

## Colors

The palette is anchored by a **Deep Slate-Teal** neutral (#1f5064), moving away from pure black to a sophisticated, cool-toned petrol base that provides rich depth for the GIS map. **Pure White** is used aggressively for primary typography to ensure high-contrast readability against the dark, tinted background.

Accent colors are used sparingly for data-driven highlights: **Tech Blue** represents modernization and liquidity, while **Muted Gold** (a refined brass tone) is reserved for premium land parcels and high-value economic metrics. Background elements utilize a layered transparency model, using semi-translucent glass effects rather than solid fills to maintain the cinematic "floating" quality.

## Typography

This design system employs a three-tier typographic hierarchy to achieve its editorial aesthetic:

1.  **Main Titles (Serif):** Uses **Noto Serif**. Large, bold serif characters for city and province names provide a sense of heritage and institutional weight.
2.  **Body Text (Sans-serif):** Uses **Manrope**. Set with light weights and generous line heights to provide an "airy" feel, reminiscent of high-end travel journals.
3.  **Data Metrics (Digital):** Uses **Space Grotesk**. This geometric font brings a futuristic, technical edge to numerical land price data, ensuring metrics look precise and modern.

For all Chinese text, Noto Serif SC and Noto Sans SC are the standard to maintain the classic-meets-modern editorial balance.

## Layout & Spacing

The layout utilizes a **12-column fluid grid** with exceptionally wide safe margins (48px) to prevent UI elements from crowding the edges of the screen. 

There are no solid sidebars. Instead, the design system relies on a "Floating Node" philosophy where UI components (data cards, legends, search bars) are anchored to the grid corners or floating in designated zones with at least 20px of clearance from one another. Fine, elegant vertical grid lines are rendered in the background at 5% opacity, serving as subtle visual anchors that guide the eye without obstructing the map.

## Elevation & Depth

Depth is conveyed through **Glassmorphism** rather than traditional shadows. Every floating element uses a `backdrop-filter: blur(25px)` to create a frosted glass effect, visually separating the UI from the underlying GIS map while allowing the deep teal map colors to bleed through subtly.

Borders are critical for definition: use ultra-fine (0.5px to 1px) strokes with a white-to-transparent linear gradient. This creates a "light-catching" edge effect that makes panels look like thin sheets of suspended glass. No heavy ambient shadows are used; instead, a very soft, large-radius glow (15% opacity Tech Blue) may be used behind primary data points to suggest importance.

## Shapes

The shape language is fluid and organic. A **Pill-shaped (1rem)** roundedness is applied to all primary floating panels to create a futuristic, soft-tech aesthetic. 

Interactive elements like buttons or input fields utilize even higher rounding (up to 3rem for larger components) to achieve a "pill" profile, differentiating them from static information cards. Elements such as map markers or data indicators should use geometric primitives—circles or diamonds—to maintain the minimalist, futuristic feel.

## Components

### Floating Glass Cards
The core container for all data. Must have a backdrop blur, a fine 1px border, and a 1rem corner radius. No solid background color; only a 10% white tint over the deep teal base.

### Cinematic Metrics
Data points should be displayed with the label in a small, wide-spaced sans-serif above the value in the futuristic digital font. The value should have a subtle outer glow if the land price evolution is positive.

### Ghost Buttons
Primary actions use pill-shaped ghost buttons with a thin white border. On hover, the button fills with a soft 15% white tint and the border glows slightly.

### Editorial Lists
Lists of land parcels should use generous vertical spacing and fine horizontal dividers (0.5px opacity). Instead of bullet points, use small Gold or Blue circles to match the rounded aesthetic.

### Timeline Scrubber
A minimalist horizontal line at the bottom of the screen with pill-shaped active markers. The active year should be highlighted with a vertical Gold line and a larger Serif font.

### Search & Filters
A single, floating pill-shaped input at the top center. It should be highly translucent, only becoming more opaque when focused, with a fully rounded profile.