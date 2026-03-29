# Swiss Style Personal Portfolio - Specification

## Project Overview
- **Project Name:** Swiss Portfolio
- **Type:** Single-page personal homepage
- **Core Functionality:** A minimalist, grid-based portfolio showcasing a designer's work and expertise
- **Target Users:** Design agencies, potential clients, recruiters

## Design Philosophy
- **Swiss Style (International Typographic Style)** - Clean, objective, mathematically precise
- **Dieter Rams:** "Less but better" - every element must have purpose
- **Massimo Vignelli:** Grid systems and typography as the foundation

---

## UI/UX Specification

### Layout Structure

**Grid System:**
- 12-column CSS Grid
- Column gap: 24px
- Max container width: 1440px
- Side margins: 48px (desktop), 24px (tablet), 16px (mobile)

**Page Sections:**
1. **Navigation (fixed top)**
   - Height: 72px
   - Logo/name left-aligned
   - Navigation links right-aligned
   - Subtle bottom border

2. **Hero Section**
   - Full viewport height minus nav
   - Large display typography
   - Brief tagline
   - Optional subtle geometric accent

3. **Skills & Experience**
   - Two-column layout
   - Skills as minimal tags or list
   - Experience as timeline

4. **Projects Showcase**
   - Grid of project cards (3 columns desktop, 2 tablet, 1 mobile)
   - Project image + title + category

5. **Contact Footer**
   - Minimal contact information
   - CTA button
   - Social links

### Responsive Breakpoints
- **Desktop:** 1024px+
- **Tablet:** 768px - 1023px
- **Mobile:** < 768px

---

### Visual Design

**Color Palette:**
- Background: `#FFFFFF` (pure white)
- Primary Text: `#1A1A1A` (near black)
- Secondary Text: `#6B6B6B` (medium gray)
- Accent: `#002FA7` (International Klein Blue - KLAS)
- Border/Lines: `#E5E5E5` (light gray)

**Typography:**
- Primary Font: `Inter`, `Helvetica Neue`, `Helvetica`, sans-serif
- Display: 96px / 700 weight / -2px letter-spacing
- H1: 56px / 700 weight / -1px letter-spacing
- H2: 32px / 600 weight / -0.5px letter-spacing
- H3: 20px / 600 weight / 0
- Body: 16px / 400 weight / 0.5px letter-spacing
- Small: 14px / 400 weight / 0.5px letter-spacing

**Spacing System (8px base):**
- xs: 8px
- sm: 16px
- md: 24px
- lg: 48px
- xl: 80px
- xxl: 120px

**Visual Effects:**
- No shadows (flat design)
- No gradients
- 1px borders for separation
- Minimal hover states

---

### Components

**Navigation:**
- Logo: Text-based, bold
- Links: Uppercase, 12px, letter-spacing 1px
- Hover: Accent color

**Buttons:**
- Primary: Accent background, white text, no border-radius
- Padding: 16px 32px
- Hover: Slightly darker accent (#001F8A)

**Project Cards:**
- Aspect ratio: 4:3
- Border: 1px solid #E5E5E5
- Hover: Card lifts 4px, border becomes accent

**Tags:**
- Border: 1px solid #E5E5E5
- Padding: 8px 16px
- Font-size: 12px, uppercase

---

## Functionality Specification

### Core Features
1. Smooth scroll navigation
2. Responsive layout adaptation
3. Hover interactions on buttons and cards
4. Sticky navigation on scroll
5. Project card hover effects

### User Interactions
- Click nav link → smooth scroll to section
- Hover button → background color change
- Hover project card → lift + border color change
- Hover nav link → text color change

### Edge Cases
- Long project titles: truncate with ellipsis
- Missing project images: show placeholder color

---

## Acceptance Criteria

1. ✓ Page uses strict 12-column grid
2. ✓ All text is left-aligned
3. ✓ Only one accent color (Klein Blue) used sparingly
4. ✓ Typography creates clear visual hierarchy
5. ✓ Interactions are minimal and purposeful
6. ✓ Fully responsive across all breakpoints
7. ✓ Navigation scrolls smoothly to sections
8. ✓ Code is clean with comments