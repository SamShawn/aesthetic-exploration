# Ghibli Portfolio - Specification

## Project Overview
- **Project Name:** Ghibli Portfolio
- **Type:** Personal portfolio homepage
- **Core Functionality:** An interactive, storybook-like personal homepage that feels like opening a magical picture book - warm, healing, and full of wonder
- **Target Users:** Design-conscious visitors, potential clients, creative collaborators

## UI/UX Specification

### Layout Structure
- **Hero Section:** Full viewport with layered floating elements
- **Content Cards:** Organic, flowing arrangement with breathing space
- **Section Flow:** Single page with natural scroll progression
- **Responsive breakpoints:**
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px

### Visual Design

#### Color Palette (Ghibli-inspired)
- **Sky Gradient Top:** `#e8f4f8` (morning mist)
- **Sky Gradient Bottom:** `#fef9f3` (warm cream)
- **Grass Green:** `#7cb342` (meadow green)
- **Forest Green:** `#4a7c59` (deep forest)
- **Warm Brown:** `#a67c52` (earth brown)
- **Terracotta:** `#c47856` (pottery clay)
- **Cloud White:** `#ffffff`
- **Text Primary:** `#2d3a3a` (deep charcoal)
- **Text Secondary:** `#5a6b6b` (muted gray)
- **Accent Gold:** `#d4a574` (wheat gold)
- **Magic Glow:** `#fff8e7` (warm light)

#### Typography
- **Heading Font:** "Noto Serif JP", serif (手写感衬线)
- **Body Font:** "M PLUS Rounded 1c", sans-serif (圆润易读)
- **Hero Title:** 56px (desktop), 36px (mobile), font-weight 400
- **Section Headings:** 28px, font-weight 500
- **Body Text:** 16px, line-height 1.8

#### Spacing System
- **Section Padding:** 120px vertical (desktop), 80px (mobile)
- **Card Padding:** 40px (desktop), 24px (mobile)
- **Element Margins:** 24px / 32px / 48px

#### Visual Effects
- **Paper Texture:** Subtle canvas/handmade paper overlay
- **Watercolor Blur:** SVG filter for soft, painted edges
- **Organic Border Radius:** Irregular, hand-drawn feeling curves
- **Ambient Particles:** Floating dust motes, pollen, or fireflies

### Components

#### 1. Background Layers
- Gradient sky mimicking Ghibli's pastoral scenes
- Distant mountains silhouette (SVG)
- Floating clouds with parallax movement
- Grass/greenery at bottom
- Animated fireflies (optional, subtle)

#### 2. Hero Card
- Centered, floating above scene
- Hand-drawn style border
- Avatar illustration area (decorative)
- Name and title
- Tagline in warm, poetic language

#### 3. Navigation (Floating)
- Minimal, positioned like wind chimes
- Handwritten hover effect
- Smooth scroll anchors

#### 4. Content Sections
- **About Section:** Story-like introduction
- **Work/Projects:** Card-based project showcase
- **Contact:** Warm, inviting contact area

#### 5. Hand-drawn Decorations
- Little creatures (like soot sprites - ス垢)
- Floating leaves
- Stars that twinkle
- Small flowers

### Animations

#### Page Load
- Scene slowly fades in like sunrise
- Clouds drift in from sides
- Hero card gently descends
- Duration: 1.5s with ease-out

#### Scroll Animations
- Parallax: clouds move at different speeds
- Content cards fade up with subtle rotation
- Mountains shift slightly for depth

#### Hover Effects
- Cards rock gently like floating on water (3-5deg rotation)
- Warm glow emanates from behind
- Decorative elements react subtly

#### Ambient Animations
- Clouds: slow drift (20-60s cycle)
- Leaves: gentle sway
- Fireflies: random twinkling
- Grass: subtle wave motion

## Functionality Specification

### Core Features
1. **Parallax scrolling** with multiple depth layers
2. **Organic, non-linear layout** mimicking picture book
3. **Hand-drawn aesthetic** via CSS/SVG techniques
4. **Warm micro-interactions** throughout
5. **Responsive adaptation** maintaining the magical feel

### User Interactions
- Scroll → parallax layers move, content reveals
- Hover on cards → gentle rocking motion + glow
- Hover on nav → handwritten underline animation
- Click nav links → smooth organic scroll

### Edge Cases
- Reduced motion: disable parallax and ambient animations
- No JS: static but still beautiful fallback
- Small screens: simplified scene, touch-friendly

## Acceptance Criteria
1. ✓ Page feels like opening a storybook
2. ✓ All animations are smooth (60fps)
3. ✓ Color palette evokes Ghibli's warm, natural tones
4. ✓ Parallax creates genuine depth perception
5. ✓ Hover states feel organic and responsive
6. ✓ Typography complements hand-drawn aesthetic
7. ✓ Works beautifully on mobile
8. ✓ No harsh edges or overly geometric shapes