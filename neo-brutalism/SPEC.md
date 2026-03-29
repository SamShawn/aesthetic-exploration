# SPEC.md - Neo-Brutalist Personal Homepage

## Project Overview
- **Project Name:** NOISE//VOID - Experimental Portfolio
- **Type:** Single-page personal portfolio website
- **Core Functionality:** A visually striking personal homepage that challenges conventional web design with Neo-Brutalist aesthetics, featuring bold geometric forms inspired by Saul Bass and fluid organic shapes inspired by Zaha Hadid
- **Target Users:** Creative professionals, design enthusiasts, potential clients

## UI/UX Specification

### Layout Structure

**Page Sections:**
1. **Hero Section (100vh)** - Massive typography, asymmetric floating shapes
2. **Manifesto Section** - Text block with brutalist styling
3. **Works Preview** - Asymmetric image/text blocks
4. **Contact/CTA** - Bold interactive element

**Grid/Layout:**
- No traditional grid - pure asymmetry
- Elements intentionally overlap and break boundaries
- Titles overflow viewport boundaries deliberately
- Diagonal lines and organic curves break the horizontal flow

**Responsive Breakpoints:**
- Desktop: 1200px+ (full experience)
- Tablet: 768px-1199px (scaled, still bold)
- Mobile: <768px (stacked but still brutalist)

### Visual Design

**Color Palette:**
- Background: `#F5F0E8` (warm off-white/bone)
- Primary Black: `#0A0A0A` (near black)
- Accent Neon: `#BFFF00` (acid lime/neon green)
- Accent Purple: `#5B00B5` (deep electric purple)
- Secondary: `#FF3366` (hot pink for highlights)
- Text Dark: `#1A1A1A`

**Typography:**
- Display Font: "Bebas Neue" (bold, condensed, impactful)
- Body Font: "Space Mono" (monospace, raw, technical feel)
- Heading sizes: 12vw for main hero (massive, beyond viewport)
- Body: 16px-18px
- Accent text: all caps, bold

**Spacing System:**
- Margins: 5vw minimum, often more
- Negative space is intentional and dramatic
- Elements separated by diagonals and overlapping shapes

**Visual Effects:**
- Noise texture overlay (CSS grain)
- Thick 4-6px black strokes on containers
- Hard shadows (no blur, offset 8-12px)
- Glitch effect on hover/click (RGB split)
- SVG geometric shapes floating

### Components

**Hero Title:**
- Text: "CREATIVE"
- Size: 20vw, exceeding all boundaries
- Overlapped by geometric shapes
- Parallax movement on mouse

**Floating Shapes:**
- Circles with thick black borders
- Semi-transparent fills with neon colors
- SVG blobs in organic Zaha Hadid-inspired curves

**Navigation:**
- Minimal, corner-anchored
- Brutalist button style: thick border, hard shadow
- Hover: invert colors with glitch

**Manifesto Block:**
- Stark black box on light background
- Monospace text, justified
- Heavy black top border (12px)

**Interactive Elements:**
- Buttons: hard-edged, 6px black border, 12px offset shadow
- Hover: translate(-4px, -4px), shadow expands
- Click: glitch RGB split animation

### Animations (GSAP)

**Page Load:**
- Staggered reveal of hero elements
- Shapes float in from random positions
- Title letters animate in with scramble effect

**Mouse Interaction:**
- Parallax on hero shapes (different speeds)
- Cursor becomes custom (large dot or crosshair)

**Scroll Animations:**
- Elements slide in at dramatic angles
- Shapes rotate and scale on scroll

**Click/Hover:**
- Glitch effect: RGB channel separation
- Snap/jerk movements
- Color inversion flashes

## Functionality Specification

### Core Features
1. **Parallax Hero** - Mouse movement affects floating elements
2. **Glitch Buttons** - Click triggers glitch animation
3. **Noise Overlay** - Subtle animated grain texture
4. **Floating Shapes** - Continuous gentle movement
5. **Custom Cursor** - Replaces default cursor

### User Interactions
- Mouse move → parallax shift on elements
- Hover buttons → color invert + glitch
- Click anywhere → subtle screen shake
- Scroll → elements animate in from off-screen

### Edge Cases
- Reduced motion preference: disable animations
- No JS fallback: static but still styled

## Acceptance Criteria

1. ✅ Page loads with staggered animation sequence
2. ✅ Hero text exceeds viewport boundaries
3. ✅ Floating shapes respond to mouse position
4. ✅ Buttons show glitch effect on click
5. ✅ Noise texture visible across page
6. ✅ Color palette matches spec exactly
7. ✅ Typography uses Bebas Neue + Space Mono
8. ✅ GSAP animations are smooth (60fps)
9. ✅ Layout is asymmetric and breaks grid
10. ✅ Mobile still has bold visual impact