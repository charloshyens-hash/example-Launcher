---
name: Jiuyi Desktop
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bbc9cf'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#859399'
  outline-variant: '#3c494e'
  surface-tint: '#4cd6ff'
  primary: '#a4e6ff'
  on-primary: '#003543'
  primary-container: '#00d1ff'
  on-primary-container: '#00566a'
  inverse-primary: '#00677f'
  secondary: '#d1bcff'
  on-secondary: '#3c0090'
  secondary-container: '#7000ff'
  on-secondary-container: '#ddcdff'
  tertiary: '#ffd59c'
  on-tertiary: '#442b00'
  tertiary-container: '#feb127'
  on-tertiary-container: '#6b4700'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#b7eaff'
  primary-fixed-dim: '#4cd6ff'
  on-primary-fixed: '#001f28'
  on-primary-fixed-variant: '#004e60'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d1bcff'
  on-secondary-fixed: '#23005b'
  on-secondary-fixed-variant: '#5700c9'
  tertiary-fixed: '#ffddb1'
  tertiary-fixed-dim: '#ffba49'
  on-tertiary-fixed: '#291800'
  on-tertiary-fixed-variant: '#624000'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-time:
    fontFamily: Inter
    fontSize: 80px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.04em
  display-date:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
    letterSpacing: 0.1em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: '600'
    lineHeight: 12px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  margin-main: 24px
  gutter-grid: 16px
  dock-padding: 32px
  drawer-top-gap: 64px
---

## Brand & Style

The design system is a modern homage to classic launcher aesthetics, reimagined through a lens of contemporary minimalism and transparency. It targets power users who value both functional efficiency and aesthetic personalization. The brand personality is nostalgic but forward-thinking, emphasizing the user's wallpaper as the primary visual foundation.

The visual style is a hybrid of **Minimalism** and **Glassmorphism**. By utilizing high-quality background blurs and translucent layers, the UI maintains a sense of depth and hierarchy without ever fully obscuring the personalized canvas beneath. Interaction is centered around a singular, iconic focal point—the circular menu—creating a rhythmic, predictable user experience that feels lightweight and atmospheric.

## Colors

The color strategy centers on a "Vibrant Neon on Dark Glass" approach. 
- **Primary:** A high-energy Cyan/Teal (#00D1FF) serves as the main interactive accent, applied to the central menu button's stroke, active states, and the clock.
- **Secondary:** A deep Electric Violet (#7000FF) is used for secondary accents and gradient subtle-touches to add depth to glass surfaces.
- **Surface Strategy:** The design system defaults to a dark mode experience to maximize the "pop" of the primary accents. Backgrounds are not solid; they are dynamic dark overlays with 60% opacity and high-saturation background blurs (32px+), allowing the wallpaper's colors to bleed through and naturally tint the interface.

## Typography

This design system utilizes **Inter** exclusively to achieve a clean, systematic, and utilitarian feel that doesn't compete with app iconography. 

- **The Clock:** Uses `display-time` with a heavy weight and tight letter-spacing to create a bold, modern "hero" moment on the home screen.
- **App Labels:** Use `label-md` for the grid view, ensuring legibility against varied wallpaper backgrounds through the use of a subtle 1px soft black text-shadow.
- **Search & Headers:** Use `headline-md` for the drawer’s search-focused header to maintain a professional, structured hierarchy.

## Layout & Spacing

The layout follows a **Fixed Grid** model optimized for one-handed vertical interaction.
- **Home Screen:** A distraction-free zone where the central circular menu sits at the bottom-center "thumb zone."
- **App Drawer:** A 4x6 grid layout. Icons are spaced with a 16px gutter. The top of the drawer features a significant 64px gap (safe area) for the search bar and quick-action headers.
- **Safe Zones:** A universal 24px margin is maintained on the left and right edges to prevent UI elements from touching the screen bezel, ensuring a "floating" glass effect.

## Elevation & Depth

Depth in this design system is communicated through **Glassmorphism and Backdrop Blurs** rather than traditional shadows.

- **Level 0 (Base):** The full-screen wallpaper.
- **Level 1 (Intermediary):** The App Drawer and Gesture Menus. These use a semi-transparent dark fill with a `32px` background blur effect and a `1px` inner border (stroke) of white at `10%` opacity to define the edges.
- **Level 2 (Interactive):** The Central Circular Menu. This element features a more opaque fill and a vibrant `2px` primary-colored outer glow to signify its status as the primary navigation anchor.

## Shapes

The shape language is primarily **Rounded**, creating a soft and approachable feel.
- **Standard Containers:** App icons and cards use a `1rem` (16px) corner radius to match modern Android hardware curves.
- **Primary Action:** The central menu button is a perfect circle, creating a distinct visual break from the rectangular grid of app icons.
- **Search Bar:** Uses a fully pill-shaped (rounded-xl) geometry to differentiate functional input from static app containers.

## Components

### Central Menu Button
The heart of the design system. A circular button with a thick primary-colored stroke. Upon press, it expands into a radial menu or triggers a glass-morphic overlay. It should feature a "breathing" subtle animation when the launcher is idle.

### App Icons & Grid
Icons are displayed in a 4x6 grid. Labels are positioned underneath icons using `label-md`. In the drawer, icons should have a consistent scale; third-party icons are placed within a "squircle" glass container if they do not match the system's roundedness.

### Glass Search Header
A pill-shaped input field located at the top of the app drawer. It uses a `15%` white fill and `24px` backdrop blur. The text is `body-lg` with a primary-colored cursor.

### Translucent Lists
For settings or long-press menus, use horizontal dividers that are `1px` tall with `10%` white opacity. List items should have a minimum tap target of `48px` height.

### Gesture Overlays
Triggered by swipes (up for drawer, down for search). These overlays should slide in with a high-damping spring animation, instantly applying the background blur to the wallpaper to shift the user's focus.
