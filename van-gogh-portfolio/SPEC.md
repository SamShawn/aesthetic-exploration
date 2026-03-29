# Van Gogh Portfolio - Specification

## Project Overview
- **Project Name:** Van Gogh Portfolio
- **Type:** Personal portfolio homepage
- **Core Functionality:** An immersive, living canvas that channels Van Gogh's Post-Impressionist vision—where every scroll is a brushstroke, every interaction ignites color, and the page itself becomes a window into the artist's turbulent, beautiful soul.
- **Target Users:** Art enthusiasts, potential clients, creative collaborators seeking a portfolio that transcends mere presentation

## UI/UX Specification

### Layout Structure
- **Hero Section:** Full viewport with swirling starfield background, artist avatar area
- **Content Cards:** Asymmetric, organically placed with varying rotations
- **Section Flow:** Single page with dramatic scroll progression
- **Responsive breakpoints:**
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px

### Visual Design

#### Color Palette (Van Gogh's Emotional Spectrum)
- **Deep Cobalt:** `#0047AB` (starry night sky)
- **Midnight Blue:** `#1a1a2e` (shadows)
- **Cadmium Yellow:** `#E3A01B` (sun, stars, warmth)
- **Golden Ochre:** `#CC7722` (wheat, earth)
- **Burnt Sienna:** `#A0522D` (autumn warmth)
- **Olive Green:** `#4a5d23` (cypress)
- **Cream Canvas:** `#f5f0e1` (canvas base)
- **Text Dark:** `#1a1a1a`
- **Text Light:** `#f5f0e1`

#### Typography
- **Heading Font:** "Playfair Display", serif (dramatic, expressive)
- **Accent Font:** "Caveat", cursive (handwritten feel for signatures/decorations)
- **Body Font:** "Source Serif Pro", serif
- **Hero Title:** 72px (desktop), 42px (mobile), font-weight 700
- **Section Headings:** 36px, font-weight 600
- **Body Text:** 18px, line-height 1.8

#### Spacing System
- **Section Padding:** 140px vertical (desktop), 80px (mobile)
- **Card Padding:** 48px (desktop), 24px (mobile)
- **Element Margins:** 32px / 48px / 64px

#### Visual Effects

##### Impasto (Thick Paint Texture)
- Multiple layered box-shadows simulating paint buildup
- CSS filter with subtle texture overlay
- Cards have visible "paint edge" effect

##### Swirling Motion Background
- Canvas-based animated starfield with swirling paths
- Multiple layers of rotating star "spirals"
- Slow, hypnotic rotation (60s cycle)
- Subtle glow on stars

##### Expressive Linework Borders
- Irregular, hand-drawn SVG borders
- Varying stroke widths (2-6px)
- Dark outline with slight "tremble" in the line

##### Canvas Texture
- Base layer with subtle canvas grain
- Background has painted quality

### Components

#### 1. Animated Starfield Background (Canvas)
- Swirling vortex pattern mimicking Starry Night
- Multiple spiral arms with varying opacity
- Twinkling stars at different sizes
- Subtle color variation (blue to yellow)

#### 2. Hero Card
- Floating, slightly tilted (2deg rotation)
- Thick impasto border
- Canvas texture background
- Decorative brushstroke elements

#### 3. Navigation (Minimal)
- Floating pill-style nav
- Brush stroke underline on hover
- Semi-transparent with backdrop blur

#### 4. Content Sections
- **About:** Personal story card with asymmetric placement
- **Projects:** Cards with varying rotations (-3deg to 3deg)
- **Contact:** Prominent call-to-action with dramatic styling

#### 5. Brush Stroke Decorations
- Decorative swirl elements in corners
- Small painted "stars" as decorative elements

### Animations

#### Page Load (2s sequence)
- Stars fade in with pulse
- Hero card rises from below with scale
- Navigation fades in last
- Easing: cubic-bezier(0.4, 0, 0.2, 1)

#### Scroll Animations
- Cards parallax at different speeds
- Swirl background rotates continuously
- Content reveals with fade + slight upward motion

#### Hover Effects
- Cards: scale(1.03) + increased saturation
- Buttons: brush stroke "thickens"
- Links: underline draws in from left

#### Ambient
- Continuous star swirl (CSS transform)
- Subtle canvas grain animation
- Twinkling stars (random opacity change)

## Functionality Specification

### Core Features
1. **Swirling starfield animation** via Canvas 2D
2. **Impasto border effects** via layered box-shadows
3. **Asymmetric card placement** with subtle rotations
4. **Custom cursor** (paintbrush icon via CSS)
5. **Smooth scroll navigation**
6. **Parallax scrolling** for depth

### User Interactions
- Scroll → parallax + content reveal
- Hover on cards → scale + saturation boost
- Hover on buttons → brush stroke thickening
- Click nav → smooth scroll to section

### Edge Cases
- Reduced motion: disable animations, show static swirl
- No JS: static but textured fallback
- Small screens: simplified background

## Acceptance Criteria
1. ✓ Background has convincing swirling star motion
2. ✓ Cards feel like painted canvas with thick borders
3. ✓ Color palette hits Van Gogh's emotional spectrum
4. ✓ Typography has dramatic, expressive quality
5. ✓ Hover states feel like adding more paint
6. ✓ Custom cursor reinforces artistic theme
7. ✓ Page feels alive and turbulent, not static
8. ✓ Works beautifully on mobile