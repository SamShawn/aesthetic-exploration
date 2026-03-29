# Matisse-Inspired Portfolio - Specification

## Project Overview
- **Name:** Matisse Portfolio
- **Type:** Personal portfolio homepage
- **Core Functionality:** A visually striking portfolio page inspired by Henri Matisse's late cut-out art, featuring organic shapes, bold Fauvist colors, and playful interactions
- **Target Users:** Creative professionals seeking a unique, art-forward web presence

## UI/UX Specification

### Layout Structure
- **Hero Section:** Large asymmetric composition with organic shapes, name/title overlaid
- **About Section:** Organic-shaped card with flowing text
- **Projects Section:** Grid of irregularly-shaped project cards
- **Contact Section:** Bold CTA with decorative cut-out elements

### Visual Design

#### Color Palette (Matisse Fauvist)
- **Primary Red:** `#E63946` (Vivid Vermillion)
- **Primary Green:** `#2A9D8F` (Emerald Teal)
- **Primary Blue:** `#264653` (Deep Cobalt)
- **Accent Yellow:** `#F4A261` (Saffron Yellow)
- **Accent Orange:** `#E76F51` (Burnt Orange)
- **Background:** `#FDF6E3` (Warm Cream)
- **Dark Accent:** `#1D3557` (Midnight Blue)

#### Typography
- **Display Font:** "Permanent Marker" - for titles (hand-cut feel)
- **Body Font:** "Outfit" - clean sans-serif for readability

#### Spacing System
- Section padding: `120px` vertical
- Card padding: `32px`
- Element gaps: `24px`

#### Visual Effects
- All shapes use `clip-path` for organic cut-out forms
- Drop shadows: `8px 8px 0 rgba(0,0,0,0.15)` (hard edge, paper-like)
- No gradients - pure flat colors per Matisse philosophy

### Components

#### 1. Hero Banner
- Large organic blob shape (cobalt blue) as background
- Floating cut-out decorations (stars, leaves, abstract figures)
- Name in large display font
- Tagline with typewriter effect

#### 2. Navigation
- Floating organic-shaped nav bar
- Icons as simple cut-out shapes

#### 3. About Card
- Vermillion organic shape
- Handwritten-style description text
- Decorative cut-out accents

#### 4. Project Cards (3)
- Three irregular shapes in different colors (teal, orange, yellow)
- Each with project preview area
- Hover: rotate 5deg + scale 1.05

#### 5. Contact Button
- Large organic shape (midnight blue)
- Paper-toss animation on click

#### 6. Decorative Elements
- Scattered cut-out shapes: stars, leaves, circles, abstract figures
- All positioned with CSS, creating collage feel

### Interactions

#### Hover States
- Cards: `transform: rotate(3deg) scale(1.03)`
- Buttons: slight color shift + shadow expand
- Links: underline animation (wavy)

#### Click Effects
- Contact button: confetti burst (paper scraps)
- Nav items: ripple effect

#### Scroll Animations
- Parallax on decorative elements (different speeds)
- Fade-in for sections with stagger

## Functionality Specification

### Core Features
1. Smooth scroll navigation
2. Animated entrance for all elements
3. Interactive hover effects on all clickable elements
4. Confetti particle system on contact click
5. Parallax scroll on background decorations
6. Responsive layout (mobile-friendly)

### User Interactions
- Click nav links → smooth scroll to section
- Hover cards → lift and rotate effect
- Click contact → confetti explosion
- Scroll → parallax decorative elements

## Acceptance Criteria
1. Page loads with staggered entrance animations
2. All shapes appear as hand-cut organic forms
3. Colors match Matisse Fauvist palette exactly
4. Hover effects feel playful and tactile
5. Confetti animation triggers on contact button click
6. Parallax creates depth on scroll
7. Mobile responsive (stacked layout)
8. No standard geometric shapes - all organic