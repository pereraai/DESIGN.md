# Design System Inspired by Horizon Blue Cross Blue Shield

## 1. Visual Theme & Atmosphere

Horizon Blue's design system embodies trust, accessibility, and professional healthcare authority. The visual language combines a deep, commanding blue palette with clean, legible typography and ample whitespace to create an approachable yet authoritative presence. The design prioritizes clarity and ease of navigation, reflecting the organization's commitment to making complex health insurance information understandable and actionable for diverse audiences. The interface balances corporate professionalism with human-centered warmth through generous spacing, high contrast, and purposeful imagery featuring real people in relatable healthcare scenarios.

**Key Characteristics**
- Deep institutional blue conveys stability and medical authority
- Clean, high-contrast layouts prioritize accessibility and readability
- Generous whitespace reduces cognitive load on complex healthcare topics
- Roboto typography ensures consistent, legible communication across devices
- Action-oriented design with clear, persistent call-to-action buttons
- Human-centered imagery paired with direct, conversational copy
- Trust-focused color choices avoid overwhelming or alarming users

## 2. Color Palette & Roles

### Primary
- **Primary Blue** (`#00468B`): Core brand color for primary CTAs, headings, and trusted actions; most frequently used for establishing brand presence
- **Primary Blue Variant** (`#11468B`): Subtle variation used in specific interactive contexts and secondary brand applications

### Accent Colors
- **Accent Blue** (`#00529B`): Enhanced contrast variant for specific emphasis and navigation states
- **Blue Alternate** (`#00468C`): Precise shade used for consistency in particular component contexts
- **Alert Red** (`#AC1B1B`): Error states, alerts, and critical information requiring immediate attention

### Interactive
- **Button Blue** (`#11468B`): Primary button backgrounds and interactive elements (RGB 17, 70, 139)
- **Light Button Background** (`#E5ECF3`): Secondary button backgrounds and low-emphasis interactive states
- **Link Blue** (`#00468B`): Default link color for navigation and inline actions

### Neutral Scale
- **Text Dark** (`#292929`): Primary text color for body copy, headings, and high-contrast readable content
- **Text Black** (`#000000`): Maximum contrast text for critical information and accessibility-critical content
- **White** (`#FFFFFF`): Primary background and text on dark/blue surfaces

### Surface & Borders
- **Light Surface** (`#E7EAEE`): Subtle background tints for secondary content areas
- **Light Blue Surface** (`#E5ECF3`): Light backgrounds for secondary buttons and calm content zones
- **Border Gray** (`#DDDDDD`): Dividers, borders, and subtle visual separation

## 3. Typography Rules

### Font Family
**Primary:** Roboto, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif
**Secondary:** Roboto, system-ui, sans-serif
**Fallback:** Arial, sans-serif

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| Display / H1 | Roboto | 48px | 700 | 56px | 0px | Hero headlines, primary page title |
| Heading / H2 | Roboto | 24px | 700 | 36px | 0px | Section headings, major content breaks |
| Heading / H3 | Roboto | 19px | 700 | 28px | 0px | Subsection headings, card titles |
| Body | Roboto | 16px | 400 | 24px | 0px | Primary body text, paragraph content |
| Body Strong | Roboto | 16px | 700 | 24px | 0px | Emphasis within body text, labels |
| Button | Roboto | 16px | 400 | 24px | 0px | Button text, interactive labels |
| Caption | Roboto | 14px | 400 | 20px | 0px | Small descriptive text, disclaimers |
| Code | Roboto Mono | 14px | 400 | 20px | 0px | Technical text, phone numbers |

### Principles
- Maintain strict hierarchy with three heading levels to prevent cognitive overload in healthcare content
- Body text at 16px ensures accessibility compliance (WCAG AA) and legibility on all screen sizes
- Bold body text (`#292929`, weight 700) emphasizes key healthcare terms without color changes
- Line heights of 1.5x font size (24px for 16px text) support readability for complex medical information
- No letter spacing adjustments required; system default provides optimal legibility with Roboto
- Use 700 weight sparingly for emphasis; default to 400 weight for body content to reduce visual noise

## 4. Component Stylings

### Buttons

#### Primary Button
```
Background: #11468B (RGB 17, 70, 139)
Text Color: #FFFFFF
Font: Roboto, 16px, weight 400
Padding: 10px 20px
Border Radius: 4.8px
Border: 2px solid #11468B
Line Height: 24px
Height: Auto (minimum 44px touch target)
Hover State: Background #00468B, darken slightly
Active State: Background #003D7A, increase shadow
Focus State: Outline 2px solid #E5ECF3 offset 2px
```

#### Secondary Button
```
Background: #E5ECF3
Text Color: #00468B (RGB 0, 70, 139)
Font: Roboto, 16px, weight 700
Padding: 10px 20px
Border Radius: 4.8px
Border: 2px solid #E5ECF3
Line Height: 24px
Height: 48px
Hover State: Background #D0E0F0, darken slightly
Active State: Background #B8D4E8
Focus State: Outline 2px solid #11468B offset 2px
```

#### Ghost Button (Transparent)
```
Background: Transparent (rgba(0, 0, 0, 0))
Text Color: #00468B
Font: Roboto, 16px, weight 400
Padding: 0px 0px
Border Radius: 0px
Border: None
Line Height: 24px
Hover State: Text color #11468B, add underline
Active State: Text color #003D7A
Focus State: Outline 2px solid #00468B offset 2px
```

#### CTA Button (Full Width)
```
Background: #11468B
Text Color: #FFFFFF
Font: Roboto, 16px, weight 400
Padding: 10px 20px
Border Radius: 4.8px
Border: 2px solid #11468B
Line Height: 24px
Height: 48px
Width: 100% (responsive)
Hover State: Background #00468B
Active State: Background #003D7A
Focus State: Outline 2px solid #E5ECF3 offset 2px
```

### Cards & Containers

#### Standard Card
```
Background: #FFFFFF
Border: 1px solid #E7EAEE
Border Radius: 0px (no radius for Horizon aesthetic)
Padding: 24px 32px
Box Shadow: 0px 1px 4px rgba(0, 0, 0, 0.12)
Text Color: #292929
Font: Roboto, 16px, weight 400, line-height 24px
```

#### Light Background Card
```
Background: #E5ECF3
Border: None
Border Radius: 0px
Padding: 24px 32px
Box Shadow: None
Text Color: #292929
Font: Roboto, 16px, weight 400, line-height 24px
```

#### Hero Section Container
```
Background: Linear gradient or image overlay with blue tint
Min Height: 440px
Padding: 48px 60px
Text Color: #292929 (body) / #00468B (headings)
Display: Flex, aligned left with image right
```

### Inputs & Forms

#### Text Input
```
Background: #FFFFFF
Border: 2px solid #E7EAEE
Border Radius: 4.8px
Padding: 12px 16px
Font: Roboto, 16px, weight 400, line-height 24px
Text Color: #292929
Placeholder Color: #999999
Focus State: Border 2px solid #00468B, outline none
Hover State: Border 2px solid #CCCCCC
Active State: Border 2px solid #00468B
```

#### Form Label
```
Font: Roboto, 16px, weight 700, line-height 24px
Text Color: #292929
Margin Bottom: 8px
Required Indicator: Color #AC1B1B, font weight 700
```

#### Checkbox / Radio
```
Size: 20px × 20px
Border: 2px solid #E7EAEE
Background: #FFFFFF
Border Radius: 4.8px (checkbox) / 50% (radio)
Checked State: Background #00468B, border 2px solid #00468B
Focus State: Outline 2px solid #00468B offset 2px
```

### Navigation

#### Top Navigation Bar
```
Background: #FFFFFF
Border Bottom: 1px solid #E7EAEE
Padding: 16px 32px
Height: 70px (including logo space)
Flex Layout: Logo left, nav items center, CTA right
```

#### Navigation Item (Inactive)
```
Font: Roboto, 16px, weight 400
Text Color: #292929
Padding: 8px 16px
Border Bottom: 3px solid transparent
Hover State: Border bottom 3px solid #00468B, text #00468B
```

#### Navigation Item (Active)
```
Font: Roboto, 16px, weight 400
Text Color: #00468B
Border Bottom: 3px solid #00468B
Padding: 8px 16px
```

#### Primary CTA Button (Header)
```
Background: #00468B
Text Color: #FFFFFF
Font: Roboto, 16px, weight 700
Padding: 10px 24px
Border Radius: 4.8px
Border: 2px solid #00468B
Height: 44px
Hover State: Background #003D7A
Focus State: Outline 2px solid #E5ECF3 offset 2px
```

### Links

#### Inline Link (Body)
```
Font: Roboto, 16px, weight 400
Text Color: #00468B
Text Decoration: Underline (optional, show on hover)
Cursor: Pointer
Hover State: Color #11468B, text decoration underline
Active State: Color #003D7A
Focus State: Outline 2px solid #00468B offset 2px
```

#### Link (Footer / Light Background)
```
Font: Roboto, 16px, weight 400
Text Color: #FFFFFF
Text Decoration: None
Hover State: Text decoration underline
Active State: Opacity 0.8
```

## 5. Layout Principles

### Spacing System
**Base Unit:** 4px
**Scale:** 4px, 8px, 12px, 16px, 20px, 24px, 28px, 32px, 40px, 48px, 60px, 96px

**Usage Context:**
- **4–8px:** Tight internal spacing within components (e.g., icon/text pairs)
- **12–16px:** Standard padding for form inputs, small cards, icon buttons
- **20–24px:** Default card padding, section spacing
- **28–32px:** Large component padding, major content separators
- **40–48px:** Section margins, hero/featured content separation
- **60–96px:** Full page section breaks, major layout shifts

### Grid & Container
- **Max Width:** 1440px (full width observed in extraction)
- **Column Strategy:** 12-column grid with gutters of 16px–32px depending on viewport
- **Container Padding:** 32px on desktop, 20px on tablet, 16px on mobile
- **Section Patterns:** Full-width hero sections, centered content containers (max 1200px), split-layout content-image pairs

### Whitespace Philosophy
Generous whitespace is core to Horizon's healthcare messaging. Content areas use minimum 24px padding; sections are separated by 48–96px margins. This prevents cognitive overload when presenting complex insurance information and creates visual hierarchy through breathing room rather than visual clutter. Pair large whitespace with strategic imagery to humanize healthcare content.

### Border Radius Scale
- **0px:** Cards, containers, major layout blocks (Horizon aesthetic prefers sharp edges)
- **4.8px:** Buttons, inputs, small interactive elements
- **8px:** Modal dialogs, secondary containers (if used)
- **50%:** Circular elements (avatars, radio buttons, toggle switches)

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| **Flat (None)** | `box-shadow: none` | Cards on primary background, flat button variants, form inputs |
| **Raised (Subtle)** | `box-shadow: rgba(0, 0, 0, 0.12) 0px 1px 4px 0px` | Standard cards, default state components |
| **Elevated (Modal)** | `box-shadow: rgba(0, 0, 0, 0.5) 0px 2.67px 8px 0px` | Modals, popovers, dropdown menus, floating content |
| **Interactive Hover** | `box-shadow: rgba(0, 0, 0, 0.16) 0px 2px 6px 0px` | Buttons on hover, card hover states |

**Shadow Philosophy:**
Horizon uses minimal elevation, relying primarily on color and typography for hierarchy. Shadows are subtle and used sparingly to avoid distraction in healthcare content. Only modal overlays and floating elements receive stronger elevation. Transitions on shadow changes should use 200ms ease-out for smooth, professional feel. Avoid harsh shadows that create visual anxiety; healthcare design requires calm, trustworthy visuals.

## 7. Do's and Don'ts

### Do
- Use **#00468B** and **#11468B** consistently for all primary actions and trust-building elements
- Maintain 16px minimum font size for body text to ensure accessibility and readability
- Apply generous padding (24px minimum) within cards to create breathing room
- Use bold (`weight: 700`) sparingly—only for headings, labels, and emphasis
- Ensure all interactive elements have clear focus states with 2px outlines
- Place CTAs prominently with full-width treatment on mobile, auto width on desktop
- Use high-contrast text (dark text on light backgrounds, light text on dark)
- Test all button and link hover states for visual feedback
- Keep navigation simple and persistent; healthcare users need orientation
- Include descriptive link text; avoid "click here" in insurance contexts

### Don't
- Don't use color alone to convey meaning (e.g., don't rely only on red for errors; add text)
- Don't apply shadows to standard cards; keep flat for clarity
- Don't mix multiple accent colors; stick to primary blue and strategic red for alerts
- Don't use font weights heavier than 700; avoid visual heaviness
- Don't create buttons smaller than 44px height (accessibility touch target minimum)
- Don't break the typography hierarchy with arbitrary sizing
- Don't add decorative borders; Horizon uses clean, minimal borders only where needed
- Don't use light gray text (`#CCCCCC`) on white; minimum contrast fails WCAG AA
- Don't left-align CTAs in mobile layouts; use full width for thumb accessibility
- Don't apply multiple box-shadows to the same element; use single shadow only

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| **Mobile** | 320px – 639px | Single column, full-width buttons, 16px padding, collapsed navigation (hamburger menu) |
| **Tablet** | 640px – 1023px | Two-column layouts where appropriate, 20px padding, expanded but simplified navigation |
| **Desktop** | 1024px – 1440px | Full 12-column grid, 32px padding, horizontal navigation, multi-column content |
| **Large Desktop** | 1440px+ | Max-width container (1440px), centered with side margins |

### Touch Targets
- **Minimum Height:** 44px for all buttons and interactive elements
- **Minimum Width:** 44px for icon buttons
- **Spacing Between Targets:** 8px minimum to prevent accidental selection
- **Link Padding:** 8px vertical, 12px horizontal minimum for inline links
- **Form Inputs:** 44px height minimum, 12px horizontal padding

### Collapsing Strategy
- **Hero Sections:** Reduce image on mobile (stack image below text), decrease padding from 60px to 24px
- **Two-Column Layouts:** Stack vertically on tablet and below; order: text left, image below
- **Navigation:** Collapse to hamburger menu below 1024px; show 3–5 primary items in expanded state
- **Button Groups:** Stack vertically on mobile (full width), arrange horizontally on tablet+ with 12px gaps
- **Typography:** H1 remains 48px on all breakpoints; H2 reduces to 20px on mobile; body stays 16px
- **Spacing:** Reduce all section margins by 50% below 768px (e.g., 48px becomes 24px); maintain minimum 16px padding

## 9. Agent Prompt Guide

### Quick Color Reference
- **Primary CTA:** Primary Blue (`#00468B`) or Primary Blue Variant (`#11468B`)
- **Primary Button Background:** Primary Blue Variant (`#11468B`, RGB 17, 70, 139)
- **Secondary Button Background:** Light Blue Surface (`#E5ECF3`)
- **Heading Text:** Text Dark (`#292929`)
- **Body Text:** Text Dark (`#292929`)
- **Link Text:** Primary Blue (`#00468B`)
- **Alert / Error:** Alert Red (`#AC1B1B`)
- **Background (Primary):** White (`#FFFFFF`)
- **Background (Secondary):** Light Surface (`#E7EAEE`) or Light Blue Surface (`#E5ECF3`)
- **Border:** Border Gray (`#DDDDDD`) or Light Surface (`#E7EAEE`)
- **Shadows (Standard):** `rgba(0, 0, 0, 0.12) 0px 1px 4px 0px`
- **Shadows (Modal):** `rgba(0, 0, 0, 0.5) 0px 2.67px 8px 0px`

### Iteration Guide

1. **All buttons must meet 44px minimum height** for mobile accessibility; use padding to achieve this without increasing font size.

2. **Primary actions always use `#11468B` background** with `#FFFFFF` text; secondary actions use `#E5ECF3` background with `#00468B` text.

3. **Typography hierarchy is strict**: H1 (48px, 700), H2 (24px, 700), H3 (19px, 700), Body (16px, 400), Caption (14px, 400). Never deviate from these sizes.

4. **Card and container layouts use 0px border radius** for consistency with Horizon's institutional aesthetic; only small interactive elements (buttons, inputs) use 4.8px radius.

5. **All interactive elements require focus states**: 2px outline in a contrasting color (typically `#00468B` or `#E5ECF3`), offset 2px from element edge.

6. **Body text is always `#292929` at 16px with 24px line height**; do not reduce font size below 16px for body content to ensure WCAG AA accessibility.

7. **Form inputs use 2px borders** (not 1px) in `#E7EAEE` by default, transitioning to `#00468B` on focus; minimum padding is 12px.

8. **Shadows are minimal**: standard cards get `rgba(0, 0, 0, 0.12) 0px 1px 4px 0px` only; modals get `rgba(0, 0, 0, 0.5) 0px 2.67px 8px 0px`. All other content is flat.

9. **Mobile-first responsive strategy**: Base styles are mobile (single column, 16px padding, hamburger nav); add breakpoints at 768px and 1024px; desktop max-width is 1440px.

10. **Link color in body text is always `#00468B`** with underline on hover; links in footer/dark backgrounds are `#FFFFFF`. Never use other colors for links.

11. **Spacing uses an 8px-based scale**: 8px, 16px, 24px, 32px, 48px, 60px, 96px. Section margins are 48px minimum; padding is 24px minimum for content containers.

12. **Alert / error messaging uses `#AC1B1B`** with supporting text; never use color alone. Pair red with icon and clear descriptive message for clarity.
