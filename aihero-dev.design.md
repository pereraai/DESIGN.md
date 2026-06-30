# Design System Inspired by AI Hero

## 1. Visual Theme & Atmosphere

AI Hero's design system embodies bold, forward-thinking minimalism with energetic accents that capture the essence of modern tech education. The visual language combines clean typography with striking geometric color blocks—particularly vibrant yellow and blue—creating a dynamic yet professional aesthetic. The system prioritizes clarity and accessibility, using generous whitespace and high-contrast text to ensure legibility while maintaining a contemporary, approachable feel. Subtle neutrals anchor the design, allowing key calls-to-action to command attention. This is a design system built for developers: no-nonsense, purposeful, and optimized for both desktop learning environments and mobile interaction.

**Key Characteristics**
- Bold geometric color blocking with primary yellow (#FFCF77) as the hero accent
- Clean, modern sans-serif typography (Geist) with generous line heights
- High contrast and minimal ornamentation for professional clarity
- Neutral palette anchored by black, white, and warm grays
- Large interactive targets and generous padding for accessibility
- Asymmetrical hero layouts balanced by centered content sections
- Technology-forward color accents (electric blue) paired with warm earth tones

## 2. Color Palette & Roles

### Primary
- **Hero Yellow** (`#FFCF77`): Dominant accent for CTAs, highlights, and visual emphasis; used extensively in hero graphics and key interactive elements
- **Deep Black** (`#000000`): Primary text and strong contrast; headlines and primary content
- **Pure White** (`#FFFFFF`): Primary background, card surfaces, and light text on dark backgrounds

### Accent Colors
- **Electric Blue** (`#0550AE`): Secondary accent for links, interactive states, and supporting visual elements
- **Vibrant Red** (`#FF3B00`): High-energy accent occasionally used for standout visual elements
- **Dark Amber** (`#321B01`): Warm tertiary accent for supporting design elements

### Interactive
- **Link Blue** (`#0550AE`): Standard hyperlink color
- **Danger Red** (`#D2483A`): Error states, destructive actions, and warnings
- **Warning Amber** (`#FFAD28`): Warning states and cautionary alerts

### Neutral Scale
- **Dark Gray 1** (`#0D1117`): Very dark neutral for subtle backgrounds and borders
- **Dark Gray 2** (`#191919`): Dark mode backgrounds and high-contrast overlays
- **Medium Gray 1** (`#6E7681`): Secondary text and muted content
- **Medium Gray 2** (`#8B949E`): Tertiary text and disabled states
- **Light Gray 1** (`#E8E8E8`): Subtle borders and dividers
- **Light Gray 2** (`#EAEEF2`): Light backgrounds and subtle surfaces
- **Light Gray 3** (`#E7E6E4`): Warm light neutral for soft backgrounds

### Surface & Borders
- **Off-White** (`#F6F8FA`): Lightest background surface, hero sections
- **Border Gray** (`#6E7781`): Standard border color for form inputs and containers
- **Subtle Border** (`rgba(0, 0, 0, 0.15)`): Light borders on white backgrounds

## 3. Typography Rules

### Font Family
**Primary:** Geist, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif

Geist is a modern, geometric sans-serif optimized for screen display with excellent readability at all sizes. All fallbacks maintain the clean, contemporary aesthetic.

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|---|---|
| Display (H1) | Geist | 60px | 400 | 63px | 0px | Hero headlines; bold presence |
| Heading 1 (H2) | Geist | 36px | 500 | 45px | 0px | Section titles; prominent hierarchy |
| Heading 2 (H3) | Geist | 30px | 600 | 37.5px | 0px | Subsection titles; strong emphasis |
| Body (Paragraph) | Geist | 24px | 300 | 30px | 0px | Long-form content; high contrast |
| Body Text | Geist | 16px | 400 | 24px | 0px | Standard body copy; default reading |
| Link (Large) | Geist | 18px | 600 | 18px | 0px | Navigation links; clickable text |
| Button / Label | Geist | 14px | 400 | 20px | 0px | Form inputs, buttons, captions |
| Label (Small) | Geist | 14px | 500 | 14px | 0px | Form labels, metadata |
| Code / Monospace | Geist | 14px | 400 | 20px | 0px | Code blocks, technical content |

### Principles
- **Generous Line Heights:** All text uses 1.25–1.5× size for breathing room and legibility
- **Weight Variation:** Light (300) for body; Regular (400) for standard text; Medium (500) and Semi-Bold (600) for emphasis
- **Contrast First:** High contrast between text and background ensures accessibility
- **Purposeful Sizing:** Display type at 60px commands hero sections; body at 16–24px supports comfortable reading
- **Font Weight as Hierarchy:** Weight increases as importance increases, reducing need for size variation

## 4. Component Stylings

### Buttons

#### Primary Button
- **Background:** `#000000`
- **Text Color:** `#FFFFFF`
- **Font Size:** `16px`
- **Font Weight:** `600`
- **Padding:** `0px 32px`
- **Height:** `62px`
- **Border Radius:** `0px`
- **Border:** `none`
- **Box Shadow:** `rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px`
- **Hover:** Background darkens to `#0D0D0D`; shadow intensifies slightly
- **Active:** Background becomes `#000000` with reduced shadow
- **Disabled:** Background `#E8E8E8`; text color `#8B949E`

#### Secondary Button
- **Background:** `#FFFFFF`
- **Text Color:** `#000000`
- **Font Size:** `14px`
- **Font Weight:** `400`
- **Padding:** `8px 20px`
- **Height:** `62px`
- **Border Radius:** `0px`
- **Border:** `1px solid #E8E8E8`
- **Box Shadow:** `none`
- **Hover:** Background `#F6F8FA`; border color `#6E7681`
- **Active:** Background `#EAEEF2`

#### Ghost Button (Icon/Minimal)
- **Background:** `transparent`
- **Text Color:** `#000000`
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Padding:** `8px 12px`
- **Height:** `64px`
- **Border Radius:** `2.8px`
- **Border:** `none`
- **Box Shadow:** `none`
- **Hover:** Background `rgba(0, 0, 0, 0.05)`
- **Active:** Background `rgba(0, 0, 0, 0.1)`

#### Text Link Button
- **Background:** `transparent`
- **Text Color:** `#000000`
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Padding:** `0px 20px`
- **Height:** `62px`
- **Border:** `none`
- **Hover:** Text color becomes `#0550AE`
- **Active:** Text color `#0550AE` with underline

### Cards & Containers

#### Content Card
- **Background:** `#FFFFFF`
- **Border:** `1px solid #E8E8E8`
- **Border Radius:** `0px`
- **Padding:** `24px` to `48px` (varies by card type)
- **Box Shadow:** `none` (clean, flat aesthetic)
- **Hover:** Subtle border color shift to `#6E7681`

#### Hero Section Container
- **Background:** `#FFFFFF` or `#F6F8FA`
- **Padding:** `64px` to `80px` vertically; responsive horizontally
- **Border:** `none`
- **Max Width:** `1200px` centered
- **Rounded Corners:** `0px` (sharp, modern edges)

#### Overlay / Modal Card
- **Background:** `#FFFFFF`
- **Border:** `1px solid #EAEEF2`
- **Padding:** `40px` to `56px`
- **Box Shadow:** `0px 20px 25px rgba(0, 0, 0, 0.1), 0px 8px 10px rgba(0, 0, 0, 0.06)`
- **Border Radius:** `0px`

### Inputs & Forms

#### Text Input
- **Background:** `#FFFFFF`
- **Text Color:** `#000000`
- **Font Size:** `16px`
- **Font Weight:** `400`
- **Padding:** `8px 28px`
- **Height:** `62px`
- **Border:** `1px solid rgba(0, 0, 0, 0.15)`
- **Border Radius:** `0px`
- **Focus:** Border color `#0550AE`; box shadow `0px 0px 0px 3px rgba(5, 80, 174, 0.1)`
- **Disabled:** Background `#F6F8FA`; text color `#8B949E`; border color `#E8E8E8`
- **Error:** Border color `#D2483A`

#### Select / Dropdown
- **Background:** `#FFFFFF`
- **Text Color:** `#000000`
- **Font Size:** `16px`
- **Padding:** `8px 28px`
- **Height:** `62px`
- **Border:** `1px solid rgba(0, 0, 0, 0.15)`
- **Border Radius:** `0px`
- **Focus:** Border color `#0550AE`
- **Hover:** Border color `#6E7681`

#### Form Label
- **Font Size:** `14px`
- **Font Weight:** `500`
- **Color:** `#000000`
- **Margin Bottom:** `8px`
- **Line Height:** `14px`

#### Checkbox / Radio
- **Size:** `20px × 20px`
- **Border:** `2px solid #6E7681`
- **Border Radius:** `2px` (checkbox); `50%` (radio)
- **Background (Checked):** `#000000`
- **Focus:** Outline `2px solid #0550AE` with `4px` offset

### Navigation

#### Top Navigation Bar
- **Background:** `#FFFFFF`
- **Height:** `62px`
- **Padding:** `0px 32px`
- **Border Bottom:** `1px solid #E8E8E8`
- **Flex:** Horizontally spaced with logo on left, nav links center, auth/icons right

#### Navigation Link
- **Font Size:** `14px` to `18px` (depends on position)
- **Font Weight:** `400` to `600`
- **Color (Default):** `#000000`
- **Color (Hover):** `#0550AE`
- **Color (Active):** `#0550AE` with underline
- **Padding:** `0px 20px`
- **Transition:** `color 200ms ease`

#### Breadcrumb
- **Font Size:** `14px`
- **Font Weight:** `400`
- **Color (Current):** `#000000`
- **Color (Previous):** `#6E7681`
- **Separator:** `/` or `>`
- **Margin:** `0px 8px` between items

### Badges & Tags

#### Badge (Primary)
- **Background:** `#FFCF77`
- **Text Color:** `#000000`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 12px`
- **Border Radius:** `2.8px`
- **Display:** `inline-block`

#### Badge (Secondary)
- **Background:** `#F6F8FA`
- **Text Color:** `#6E7681`
- **Font Size:** `12px`
- **Font Weight:** `500`
- **Padding:** `4px 12px`
- **Border Radius:** `2.8px`
- **Border:** `1px solid #E8E8E8`

#### Status Badge (Warning)
- **Background:** `#FFAD28`
- **Text Color:** `#000000`
- **Font Size:** `12px`
- **Font Weight:** `600`
- **Padding:** `4px 12px`
- **Border Radius:** `2.8px`

#### Status Badge (Error)
- **Background:** `#D2483A`
- **Text Color:** `#FFFFFF`
- **Font Size:** `12px`
- **Font Weight:** `600`
- **Padding:** `4px 12px`
- **Border Radius:** `2.8px`

## 5. Layout Principles

### Spacing System

**Base Unit:** `4px`

**Scale:**
- `4px` — Micro spacing within components (icon gaps, tight padding)
- `8px` — Small gaps between elements
- `12px` — Form field spacing
- `16px` — Standard padding for buttons, inputs, cards
- `20px` — Medium gaps between sections
- `24px` — Card padding, article margins
- `32px` — Large gaps, section separators
- `40px` — Generous padding for containers
- `48px` — Hero section padding
- `56px` — Large section dividers
- `64px` — Hero/section padding
- `80px` — Extra-large section spacing

**Usage Contexts:**
- Micro spacing (`4px`, `8px`) — Icon margins, inline element gaps
- Component padding (`16px`, `24px`) — Button, card, input spacing
- Section spacing (`32px`, `48px`, `64px`, `80px`) — Page-level rhythm
- External margins — Top/bottom: `32px`–`64px`; left/right: responsive

### Grid & Container

- **Max Width:** `1200px` for main container content
- **Column Strategy:** 12-column flexible grid; collapses to 4 columns (tablet) and 1 column (mobile)
- **Horizontal Padding:** `32px` on desktop; `24px` on tablet; `16px` on mobile
- **Section Patterns:**
  - **Full-Width Hero:** Extends edge-to-edge; internal content max `1200px` centered
  - **Alternating Content:** Text left, image right; reverses on tablet
  - **Centered Content:** Content max `1000px` centered with symmetrical white space
  - **Card Grid:** 2–3 columns on desktop; 1 column on mobile; gap `32px`

### Whitespace Philosophy

Whitespace is generously used to create breathing room and guide visual hierarchy. Large vertical gaps (`48px`–`80px`) between major sections reduce cognitive load. Horizontal padding on containers ensures text doesn't touch edges. Within components, consistent padding ratios (e.g., 1:1 for horizontal/vertical on buttons) create visual balance. The system avoids cramped layouts; negative space is treated as a design element.

### Border Radius Scale

- `0px` — Buttons, cards, inputs, navigation (sharp, modern aesthetic)
- `2.8px` — Badge and small component accents
- `4px` — Subtle roundness on secondary badges and focus states
- `0.8px` — Minimal rounding on link styles
- Circular (`50%` or very large px value) — Avatar images, circular icons

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (L0) | No shadow, clean edges | Cards, buttons, inputs, default state |
| Raised (L1) | `rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px` | Primary buttons on hover, interactive elevation |
| Modal (L2) | `0px 20px 25px rgba(0, 0, 0, 0.1), 0px 8px 10px rgba(0, 0, 0, 0.06)` | Modals, overlay cards, floating elements |
| Floating (L3) | `0px 50px 100px rgba(0, 0, 0, 0.15), 0px 15px 35px rgba(0, 0, 0, 0.2)` | Tooltips, dropdowns, top-level menus |

**Shadow Philosophy**

AI Hero uses minimal elevation through understated shadows. The primary shadow (`0px 20px 25px -5px` with `10%` opacity) creates subtle depth without overwhelming the clean aesthetic. Shadows are reserved for interactive states (button hover) and layered components (modals), maintaining a modern, flat-leaning design. No shadow is used by default; depth is suggested through borders and proximity rather than heavy shadow effects.

## 7. Do's and Don'ts

### Do

- **Use `#FFCF77` (Hero Yellow) for key CTAs** — Draw user attention to primary actions; it's the system's most recognizable accent
- **Pair bold typography with generous whitespace** — Let headlines breathe with large line heights and surrounding space
- **Maintain `0px` border radius on major components** — Buttons, cards, inputs should be sharp-edged for the modern aesthetic
- **Prioritize black-on-white contrast** — Default to pure `#000000` text on `#FFFFFF` backgrounds for maximum readability
- **Use `16px`–`24px` type sizes for body content** — Ensures comfortable reading on all devices without zooming
- **Leverage the 12-column grid with generous gaps** — Creates rhythm and alignment without rigidity
- **Apply focus states with `#0550AE` blue** — Consistent visual feedback for keyboard navigation and accessibility
- **Stack sections with `48px`–`80px` vertical gaps** — Establishes clear visual hierarchy between sections
- **Use system font stack with Geist as primary** — Ensures performance and modern appearance across browsers

### Don't

- **Avoid using warm accent colors for error states** — Reserve red (`#D2483A`) for errors; yellow is for success/emphasis only
- **Don't use border radius > `4px` on main components** — The design system intentionally uses sharp edges; rounded corners dilute the modern aesthetic
- **Avoid stacking shadows** — Don't combine multiple shadow layers; use a single, appropriate shadow per elevation level
- **Don't set text smaller than `14px`** — Violates accessibility standards; maintain minimum size for all interactive elements
- **Avoid high contrast color combinations other than black/white/blue** — Stick to the palette; unauthorized colors break visual coherence
- **Don't use full-width layouts without max-width constraints** — Always cap content at `1200px` to maintain readability on ultra-wide screens
- **Avoid padding < `16px` on interactive elements** — Buttons and inputs need adequate touch targets (minimum `44px` height)
- **Don't mix rounded and sharp corners within the same component group** — Maintain consistency (e.g., all buttons sharp, all icons rounded)
- **Avoid light gray text on white backgrounds** — Ensure minimum `4.5:1` contrast ratio for WCAG AA compliance

## 8. Responsive Behavior

### Breakpoints

| Breakpoint Name | Width | Key Changes |
|---|---|---|
| Mobile | 320px–767px | 1-column layout; `16px` horizontal padding; buttons full-width; font sizes -2px; simplified navigation (hamburger menu) |
| Tablet | 768px–1023px | 2-column grid; `24px` horizontal padding; buttons inline; primary nav visible; card grid becomes 2 columns |
| Desktop | 1024px–1439px | 3-column grid; `32px` horizontal padding; max-width `1200px`; full navigation; all sections use intended layout |
| Large Desktop | 1440px+ | Same as desktop; increased horizontal padding maintains `1200px` max-width; generous side margins |

### Touch Targets

- **Minimum Interactive Size:** `44px × 44px` (meets WCAG 2.5 level AAA)
- **Buttons:** `62px` height standard (exceeds minimum)
- **Form Inputs:** `62px` height with `28px` horizontal padding
- **Links:** `20px` horizontal padding minimum; `18px` font for navigation links
- **Icon Buttons:** `64px` square (3 cols for sidebar)
- **Spacing Between Targets:** `8px` minimum gap to prevent accidental taps

### Collapsing Strategy

- **Navigation:** Desktop horizontal nav → Tablet inline dropdown → Mobile hamburger menu (collapsed at 768px)
- **Hero Section:** Desktop: image right, text left; Tablet/Mobile: stacked vertically with image above
- **Card Grid:** Desktop 3-column → Tablet 2-column → Mobile 1-column (adjust gap from `32px` to `24px` on tablet, `16px` on mobile)
- **Alternating Layout:** Two-column alternating → Single column with consistent top-to-bottom flow
- **Typography:** H1: 60px (desktop) → 48px (tablet) → 36px (mobile); Body: 16px (desktop) → 14px (tablet) → 14px (mobile)
- **Padding:** Sections 64px–80px (desktop) → 40px–48px (tablet) → 24px–32px (mobile)
- **Horizontal Padding:** 32px (desktop) → 24px (tablet) → 16px (mobile)

## 9. Agent Prompt Guide

### Quick Color Reference

- **Primary CTA:** Deep Black (`#000000`) button background with Hero Yellow (`#FFCF77`) for supporting accents
- **Heading Text:** Deep Black (`#000000`)
- **Body Text:** Deep Black (`#000000`) on white; Medium Gray (`#6E7681`) for secondary
- **Background (Light):** Pure White (`#FFFFFF`) or Off-White (`#F6F8FA`)
- **Background (Dark):** Dark Gray (`#0D1117`) or Deep Black (`#191919`)
- **Interactive (Hover):** Electric Blue (`#0550AE`) for links; lighter shadow for buttons
- **Error/Warning:** Red (`#D2483A`) for error; Amber (`#FFAD28`) for warning
- **Borders:** Border Gray (`#6E7681`) or subtle `rgba(0, 0, 0, 0.15)`
- **Accent Highlights:** Hero Yellow (`#FFCF77`) in geometric blocks and CTA emphasis
- **Disabled State:** Light Gray (`#E8E8E8`) background; Medium Gray (`#8B949E`) text

### Iteration Guide

1. **Color First:** All interactive elements default to black (`#000000`) background with white text; use Hero Yellow (`#FFCF77`) and Electric Blue (`#0550AE`) as secondary accents only. Errors always use Red (`#D2483A`).

2. **Typography Lock:** Use Geist font stack exclusively. Maintain: Display at 60px (400 weight), H2 at 36px (500 weight), H3 at 30px (600 weight), Body at 16px–24px (300–400 weight). Line heights: body text minimum 1.25× size.

3. **Border Radius = 0:** All buttons, inputs, cards, and major components use `0px` border radius. Exceptions: badges (`2.8px`), icon buttons (micro-components, `2.8px`), and avatars (circular).

4. **Shadow Discipline:** Use no shadow by default. Apply only on hover (button): `rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px`. Modals: `0px 20px 25px rgba(0, 0, 0, 0.1), 0px 8px 10px rgba(0, 0, 0, 0.06)`.

5. **Component Height Standard:** Buttons and inputs: `62px`. Ensure `8px` vertical padding with content centered. Form labels: `14px` (500 weight).

6. **Spacing Rhythm:** Section gaps `48px`–`80px` (desktop). Content padding `24px`–`56px`. Horizontal page padding: `32px` (desktop), `24px` (tablet), `16px` (mobile). Grid gaps: `32px` on desktop; reduce by `8px` per breakpoint.

7. **Contrast & Accessibility:** All text must achieve minimum 4.5:1 contrast ratio (WCAG AA). Default to `#000000` on `#FFFFFF`. Disabled states use Medium Gray (`#8B949E`) with Light Gray background (`#F6F8FA`).

8. **Responsive Collapse:** Max-width container `1200px` centered. Breakpoints: 320px (mobile 1-col), 768px (tablet 2-col), 1024px (desktop 3-col). Adjust padding and font sizes proportionally; never stack borders.

9. **Interactive States:** Buttons: default white/black (secondary) or black/white (primary). Hover: slight shadow + border color shift. Focus: `2px solid #0550AE` outline with `4px` offset. Active: background intensifies. Disabled: `#E8E8E8` background + `#8B949E` text.

10. **Hero Section Pattern:** Full-width background (white or off-white), internal max-width `1200px` centered. Text left (align left), image/graphic right. Padding: `64px` top/bottom, responsive sides. On mobile, stack vertically (text above image).
