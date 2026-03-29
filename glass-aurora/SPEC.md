# Glass Aurora Portfolio - Specification

## Project Overview
- **Project Name:** Glass Aurora Portfolio
- **Type:** Personal portfolio homepage
- **Core Functionality:** Immersive glassmorphism portfolio with aurora background, showcasing personal brand with premium visual effects
- **Target Users:** Design-conscious visitors, potential clients, employers

## UI/UX Specification

### Layout Structure
- **Full viewport height** hero section with centered content
- **Card-based content** with glass effect floating in layers
- **Responsive breakpoints:**
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px

### Visual Design

#### Color Palette
- **Background Base:** `#0a0a0f` (deep space black)
- **Background Gradient Colors:**
  - Aurora Cyan: `#00d4ff`
  - Aurora Purple: `#7b2ff7`
  - Aurora Magenta: `#ff006e`
  - Aurora Teal: `#00f5d4`
- **Glass Card Background:** `rgba(255, 255, 255, 0.03)`
- **Glass Border:** `rgba(255, 255, 255, 0.08)`
- **Text Primary:** `#ffffff`
- **Text Secondary:** `rgba(255, 255, 255, 0.6)`
- **Accent Glow:** `#00d4ff` (cyan)
- **Accent Secondary:** `#7b2ff7` (purple)

#### Typography
- **Heading Font:** "Playfair Display", serif (elegant, editorial)
- **Body Font:** "DM Sans", sans-serif (clean, modern)
- **Hero Title:** 72px (desktop), 42px (mobile), font-weight 300
- **Section Headings:** 32px, font-weight 500
- **Body Text:** 16px, line-height 1.7

#### Spacing System
- **Card Padding:** 48px (desktop), 24px (mobile)
- **Section Margins:** 80px vertical
- **Element Spacing:** 16px / 24px / 32px

#### Visual Effects
- **Aurora Background:** Animated gradient blobs moving slowly (20-40s cycle)
- **Glass Effect:**
  - `backdrop-filter: blur(20px)`
  - Background: `rgba(255, 255, 255, 0.03)`
  - Border: `1px solid rgba(255, 255, 255, 0.08)`
  - Box-shadow: `0 8px 32px rgba(0, 0, 0, 0.3)`
- **Hover Glow:** Subtle cyan border glow animation (0.4s ease)
- **Noise Texture Overlay:** Subtle grain for depth

### Components

#### 1. Aurora Background
- Canvas-based animated gradient orbs
- 4-5 floating color blobs
- Slow, organic movement (perlin noise or sin/cos)
- Blur effect to create soft aurora feel

#### 2. Glass Card (Hero)
- Centered card with name, title, tagline
- Glassmorphism with subtle border glow
- Floating animation (subtle up/down)
- Hover: edge glow sweep effect

#### 3. Navigation
- Minimal top nav with glass effect
- Links: About, Work, Contact
- Hover: text glow

#### 4. Content Cards (About, Skills, Contact)
- Staggered grid layout
- Each card with glass effect
- Scroll-triggered fade-in and float-up animations
- Hover: subtle lift and glow

#### 5. Social Links
- Minimal icon row
- Glass button style
- Hover: scale + glow

### Animations

#### Page Load
- Staggered reveal: background → hero card → nav → other content
- Duration: 0.8s - 1.2s with easing
- Sequence delay: 0.1s between elements

#### Scroll Animations
- Elements fade in + translateY(30px → 0)
- Intersection Observer based
- Threshold: 0.2

#### Hover Effects
- Cards: translateY(-4px) + border glow
- Buttons: scale(1.02) + glow pulse
- Links: text-shadow glow

## Functionality Specification

### Core Features
1. **Responsive layout** adapting to all screen sizes
2. **Animated aurora background** with Three.js or canvas
3. **Glass morphism cards** with blur and transparency
4. **Smooth scroll behavior** with intersection animations
5. **Interactive hover states** with glow effects

### User Interactions
- Hover on cards → glow effect + slight lift
- Scroll → content fades in with stagger
- Click social links → external link opens
- Click nav links → smooth scroll to section (if multi-section)

### Edge Cases
- Reduced motion: disable animations if user prefers
- No JavaScript: basic content still visible
- Small screens: simplified background effect

## Acceptance Criteria
1. ✓ Aurora background animates smoothly (60fps target)
2. ✓ Glass cards have visible blur effect
3. ✓ Hover states show glow animation
4. ✓ Scroll animations trigger correctly
5. ✓ Responsive on mobile/tablet/desktop
6. ✓ Colors match specified palette
7. ✓ Typography uses specified fonts
8. ✓ Overall feel is premium and immersive