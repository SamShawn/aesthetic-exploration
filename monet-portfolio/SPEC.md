# Monet Portfolio - Specification

## Project Overview
- **Project Name:** Monet Portfolio
- **Type:** Personal portfolio homepage
- **Core Functionality:** An immersive, dreamlike digital experience channeling Claude Monet's Impressionist vision—where light dances across soft edges, colors blend like morning mist on water, and the page breathes with the quiet poetry of nature.
- **Target Users:** Art enthusiasts, potential clients, creative collaborators seeking a portfolio that embodies tranquility and artistic refinement

## UI/UX Specification

### Layout Structure
- **Hero Section:** Full viewport with animated gradient "water lily pond" background
- **Content Cards:** Floating, organic placement with gentle curves
- **Section Flow:** Single page with subtle scroll progression
- **Responsive breakpoints:**
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px

### Visual Design

#### Color Palette (Monet's Impressionist Spectrum)
- **Lavender Mist:** `#E6E6FA` (primary soft accent)
- **Mint Green:** `#98FF98` (nature, water lilies)
- **Soft Pink:** `#FFB6C1` (cherry blossoms, dawn)
- **Warm Buttercream:** `#FFFACD` (sunlight, warmth)
- **Cobalt Blue Shadow:** `#6B8DBB` (water, shadows)
- **Pale Lavender:** `#D8BFD8` (twilight)
- **Pearl White:** `#FDFAF6` (canvas base)
- **Text Primary:** `#2D3436` (soft charcoal)
- **Text Secondary:** `#636E72` (muted gray)

#### Typography
- **Heading Font:** "Playfair Display", serif (elegant, breathing)
- **Body Font:** "Cormorant Garamond", serif (refined, readable)
- **Hero Title:** 64px (desktop), 36px (mobile), font-weight 400
- **Section Headings:** 32px, font-weight 500
- **Body Text:** 18px, line-height 2, letter-spacing 0.02em

#### Spacing System
- **Section Padding:** 120px vertical (desktop), 60px (mobile)
- **Card Padding:** 48px (desktop), 24px (mobile)
- **Element Margins:** 24px / 40px / 64px
- **Border Radius:** Organic curves (24px - 48px)

#### Visual Effects

##### Ambient Gradient Background
- Multi-layered CSS gradient simulating water surface
- Colors slowly shift between dawn, midday, and dusk tones
- Animation cycle: 30 seconds
- Subtle wave-like motion via CSS transforms

##### Bokeh Light Spots
- 8-12 floating light orbs
- Varying sizes (40px - 200px)
- Soft blur (80px - 150px)
- Gentle floating animation (sine wave motion)
- Colors: warm buttercream, soft pink, lavender
- Opacity: 0.3 - 0.6

##### Glassmorphism Cards
- Background: rgba(253, 250, 246, 0.25)
- Backdrop-filter: blur(20px) saturate(180%)
- Border: 1px solid rgba(255, 255, 255, 0.4)
- Box-shadow: 0 8px 32px rgba(107, 141, 187, 0.15)
- Hover: blur increases to 30px, slight lift

##### Soft Blur Aesthetic
- All container edges use subtle blur
- No harsh borders or lines
- Text has slight text-shadow for depth

### Components

#### 1. Animated Water Surface Background
- Layered CSS gradients (3 layers)
- Slow color shift animation
- Subtle horizontal drift (translateX)

#### 2. Floating Bokeh Orbs
- Absolute positioned divs
- CSS animation: gentle float (8-20s cycle)
- Gaussian blur filter
- Random starting positions

#### 3. Hero Card
- Centered, slightly elevated
- Subtle entrance animation (fade + rise)
- Name in large Playfair Display
- Title/tagline in softer weight

#### 4. Content Cards (Glassmorphism)
- **About Card:** Brief bio, floating left
- **Projects Card:** Grid of work samples
- **Contact Card:** Gentle CTA with email link
- All with hover: lift + increased blur

#### 5. Decorative Elements
- Small blurred circles as light reflections
- Subtle dot patterns (water ripples)
- Minimal divider lines (gradient fade)

### Animations

#### Page Load (3s sequence)
- Background gradient fades in first (0s)
- Bokeh orbs appear sequentially (0.5s - 2s)
- Hero card rises with fade (1s delay)
- Content cards stagger in (1.5s - 2.5s)
- All animations use ease-out curves

#### Scroll Animations
- Cards parallax subtly (different speeds)
- Background color shifts subtly based on scroll
- Content reveals with fade + gentle rise

#### Hover Effects
- Cards: translateY(-8px) + blur increase
- Blur: 20px → 30px
- Box-shadow intensifies
- Transition: 0.6s cubic-bezier(0.4, 0, 0.2, 1)

#### Ambient
- Bokeh orbs: continuous gentle float
- Background: slow color gradient shift
- Subtle "breathing" on hero text

## Functionality Specification

### Core Features
1. **Animated gradient background** with color shifts
2. **Floating bokeh orbs** with blur and float
3. **Glassmorphism cards** with hover effects
4. **Smooth entrance animations** (staggered)
5. **Responsive design** (mobile-friendly)
6. **Subtle parallax** on scroll

### User Interactions
- Scroll → subtle parallax + content reveal
- Hover on cards → lift + blur increase
- Hover on links → gentle underline animation

### Edge Cases
- Reduced motion: disable animations, show static gradient
- No JS: static but beautiful fallback
- Small screens: simplified bokeh (fewer orbs)

## Acceptance Criteria
1. ✓ Background has dreamy, shifting gradient (water surface feel)
2. ✓ Bokeh orbs float organically with soft blur
3. ✓ Cards have glassmorphism with Monet's palette
4. ✓ Typography breathes with generous spacing
5. ✓ Hover effects feel like floating on water
6. ✓ Page load creates peaceful, staggered entrance
7. ✓ Overall feeling: quiet poetry, not loud
8. ✓ Works beautifully on mobile