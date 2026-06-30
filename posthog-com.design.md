# Design System Inspired by PostHog

## 1. Visual Theme & Atmosphere

PostHog's design system embodies a sophisticated, developer-first aesthetic rooted in warm, earthy neutrals and refined typography. The visual language balances professional minimalism with personality through a carefully curated beige-to-charcoal palette, creating an approachable yet authoritative presence. The system prioritizes clarity and usability for technical audiences, with generous whitespace, readable type scales, and purposeful accent colors that guide attention without overwhelming. A subtle warmth permeates the design—particularly through the use of cream and warm grays—while deep charcoals ground the interface with stability and trust. This is a design system for builders: clean, intentional, and designed to stay out of the way while users focus on their work.

**Key Characteristics**

- Warm, earthy neutral palette with intentional color restraint
- High contrast for legibility and accessibility in technical contexts
- Developer-focused typography hierarchy using Open Runde and IBM Plex Sans Variable
- Minimal ornamentation with emphasis on functional design
- Generous spacing and breathing room between elements
- Purposeful use of accent colors (blue, orange, warning yellows) for interactive states and status
- Confidence-building depth through subtle shadows and elevation

## 2. Color Palette & Roles

### Primary

- **Deep Charcoal** (`#23251D`): Primary text color for headings and high-priority content; conveys authority and focus
- **Warm Taupe** (`#4D4F46`): Secondary text, neutral body copy, and default interactive states; warm and approachable
- **Pure Black** (`#000000`): Critical text, borders, and high-contrast accents; used sparingly for maximum impact

### Accent Colors

- **Bright Blue** (`#2F80FA`): Primary call-to-action, links, and interactive highlights; signals action and trust
- **Warm Amber** (`#F1A82C`): Warning and attention states; draws focus without alarm
- **Danger Red** (`#E92F2F`): Error states and critical warnings; semantic danger indicator
- **Burnt Orange** (`#F54E00`): Secondary error and alert indicator; used in conjunction with red for emphasis
- **Lime Green** (`#00FF00`): Success and positive confirmation states; validates completed actions

### Interactive

- **Link Blue** (`#2F80FA`): Underlined links and navigational elements; distinct from body text
- **Button Amber** (`#CD8407`): Primary button backgrounds and call-to-action containers; warm and inviting
- **Button Border** (`#B17816`): Button borders and secondary interactive affordances; slightly darker than button fill

### Neutral Scale

- **Light Gray** (`#EEEFE9`): Subtle backgrounds, disabled states, and minimal contrast areas
- **Pale Gray** (`#BFC1B7`): Dividers, borders, and light separators
- **Medium Gray** (`#B6B7AF`): Icons, secondary content, and tertiary text
- **Mid Gray** (`#9EA096`): Form placeholders, hints, and deemphasized content
- **Charcoal Gray** (`#73756B`): Secondary headings and medium-contrast text
- **Dark Gray** (`#65675E`): Body text and standard content
- **Stone Gray** (`#374151`): Dark neutral for high-contrast applications

### Surface & Borders

- **Cream** (`#E1D7C2`): Off-white surface backgrounds and warm highlights; alternative to pure white
- **White** (`#FFFFFF`): Primary surface, cards, modals, and container backgrounds
- **Transparent Black** (`#0000`): Used for overlay and transparency effects with full opacity fallbacks

## 3. Typography Rules

### Font Family

**Primary: Open Runde**
- Used for headlines, display text, and brand-prominent content
- Fallback stack: `Open Runde, system-ui, -apple-system, sans-serif`

**Secondary: IBM Plex Sans Variable**
- Used for body copy, UI text, and interactive elements
- Fallback stack: `IBM Plex Sans Variable, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif`

**Monospace: Source Code Pro, ui-monospace**
- Used for code blocks, terminal output, and technical content
- Fallback stack: `Source Code Pro, ui-monospace, "Courier New", monospace`

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| Display / H1 | Open Runde | 24px | 800 | 32px | 0px | Bold brand statement; maximum visual hierarchy |
| Heading / H2 | Open Runde | 24px | 700 | 32px | 0px | Section headlines; strong visual weight |
| Subheading / H3 | Open Runde | 16px | 700 | 24px | 0px | Card titles and subsection headers |
| Body / Paragraph | IBM Plex Sans Variable | 15px | 400 | 22.5px | 0px | Standard reading text; optimal for longer content |
| UI / Label | IBM Plex Sans Variable | 13px | 500 | 13px | 0px | Button text, form labels, and small UI elements |
| Link | IBM Plex Sans Variable | 16px | 400 | 24px | 0px | Navigational links and inline hyperlinks |
| Code / Technical | Source Code Pro | 14px | 500 | 20px | 0px | Inline and block code; higher weight for clarity |
| Code / Inline | ui-monospace | 13px | 400 | 18.85px | 0px | Terminal commands and code snippets |

### Principles

- **Hierarchy through weight, not size**: Open Runde's generous weight range (400–800) enables clear hierarchy without drastic size jumps
- **Warm and approachable**: Font choices prioritize human readability over sterile minimalism
- **Monospace consistency**: Code content uses consistent monospace stacks for technical credibility
- **Line height breathing room**: 1.5× minimum line height ensures comfortable reading in body copy and longer-form content
- **Size discipline**: Limited to 7 distinct sizes across the entire system; reduces CSS bloat and maintains visual coherence

## 4. Component Stylings

### Buttons

#### Primary Button
- **Background**: `#CD8407` (warm amber)
- **Text Color**: `#23251D` (deep charcoal)
- **Padding**: `8px 16px`
- **Font Size**: `13px`
- **Font Weight**: `500`
- **Font Family**: `IBM Plex Sans Variable`
- **Border Radius**: `4px`
- **Border**: `1px solid #B17816`
- **Height**: `32px`
- **Line Height**: `13px`
- **Hover State**: background `#B17816`, slight scale transform `1.02`
- **Active State**: background `#9D5E0D`, shadow inset `inset 0 2px 4px rgba(0,0,0,0.2)`
- **Disabled State**: background `#EEEFE9`, color `#9EA096`, cursor `not-allowed`

#### Secondary Button
- **Background**: `rgba(0,0,0,0)` (transparent)
- **Text Color**: `#23251D` (deep charcoal)
- **Padding**: `8px 16px`
- **Font Size**: `13px`
- **Font Weight**: `500`
- **Font Family**: `IBM Plex Sans Variable`
- **Border Radius**: `4px`
- **Border**: `1px solid #4D4F46`
- **Height**: `32px`
- **Line Height**: `13px`
- **Hover State**: background `rgba(77, 79, 70, 0.05)`, border `1px solid #23251D`
- **Active State**: background `rgba(77, 79, 70, 0.1)`
- **Disabled State**: border `1px solid #EEEFE9`, color `#9EA096`

#### Ghost Button (Tertiary)
- **Background**: `rgba(0,0,0,0)` (transparent)
- **Text Color**: `#4D4F46` (warm taupe)
- **Padding**: `2px 8px`
- **Font Size**: `13px`
- **Font Weight**: `500`
- **Font Family**: `IBM Plex Sans Variable`
- **Border Radius**: `4px`
- **Border**: `0px solid transparent`
- **Height**: `28px`
- **Line Height**: `13px`
- **Hover State**: background `rgba(77, 79, 70, 0.08)`, text color `#23251D`
- **Active State**: background `rgba(77, 79, 70, 0.12)`

### Cards & Containers

#### Standard Card
- **Background**: `#FFFFFF` (white)
- **Padding**: `16px 32px`
- **Border Radius**: `0px` (sharp edges for modern aesthetic)
- **Border**: `1px solid #BFC1B7` (pale gray divider)
- **Shadow**: `0px 4px 12px rgba(0, 0, 0, 0.08)`
- **Text Color**: `#374151` (stone gray for body content)
- **Font Size**: `15px`
- **Line Height**: `22.5px`

#### Elevated Card (Modal / Overlay)
- **Background**: `#FFFFFF`
- **Padding**: `24px 32px`
- **Border Radius**: `0px`
- **Border**: `1px solid #BFC1B7`
- **Shadow**: `0px 20px 25px -5px rgba(0, 0, 0, 0.1), 0px 8px 10px -6px rgba(0, 0, 0, 0.1)`
- **Text Color**: `#374151`

#### Code / Terminal Card
- **Background**: `#1E1F23` (near-black for contrast)
- **Padding**: `16px`
- **Border Radius**: `4px`
- **Border**: `1px solid #374151`
- **Text Color**: `#FFFFFF` (white for code contrast)
- **Font Family**: `Source Code Pro`
- **Font Size**: `14px`
- **Line Height**: `20px`

### Inputs & Forms

#### Text Input
- **Background**: `#FFFFFF`
- **Border**: `1px solid #BFC1B7`
- **Border Radius**: `4px`
- **Padding**: `8px 12px`
- **Font Size**: `15px`
- **Font Family**: `IBM Plex Sans Variable`
- **Text Color**: `#23251D`
- **Placeholder Color**: `#9EA096` (mid gray)
- **Focus State**: border `2px solid #2F80FA`, outline `none`, box-shadow `0 0 0 3px rgba(47, 128, 250, 0.1)`
- **Disabled State**: background `#EEEFE9`, color `#9EA096`, cursor `not-allowed`

#### Form Label
- **Font Size**: `13px`
- **Font Weight**: `500`
- **Color**: `#23251D`
- **Font Family**: `IBM Plex Sans Variable`
- **Margin Bottom**: `4px`
- **Display**: `block`

#### Helper Text
- **Font Size**: `12px`
- **Color**: `#9EA096`
- **Font Weight**: `400`
- **Margin Top**: `4px`

#### Error State
- **Border Color**: `#E92F2F` (danger red)
- **Helper Text Color**: `#E92F2F`
- **Focus Box Shadow**: `0 0 0 3px rgba(233, 47, 47, 0.1)`

### Navigation

#### Primary Navigation (Header)
- **Background**: `rgba(0,0,0,0)` (transparent over page background)
- **Padding**: `0px 0px` (layout-dependent)
- **Height**: Auto (content-driven)
- **Font Size**: `16px`
- **Font Weight**: `400`
- **Font Family**: `IBM Plex Sans Variable`
- **Text Color**: `#000000` (pure black for navigation contrast)
- **Line Height**: `24px`

#### Navigation Link (Default)
- **Color**: `#4D4F46`
- **Text Decoration**: `none`
- **Font Size**: `16px`
- **Font Weight**: `400`
- **Padding**: `0px 0px`
- **Hover State**: color `#23251D`, text-decoration `underline`
- **Active State**: color `#2F80FA` (bright blue)

#### Navigation Link (Brand CTA)
- **Background**: `#CD8407` (warm amber)
- **Color**: `#23251D` (deep charcoal)
- **Padding**: `8px 16px`
- **Font Size**: `13px`
- **Font Weight**: `500`
- **Border Radius**: `6px`
- **Border**: `1px solid #B17816`
- **Height**: `32px`
- **Hover State**: background `#B17816`, shadow `0 2px 8px rgba(0,0,0,0.12)`

### Links (Inline)

#### Text Link
- **Color**: `#2F80FA` (bright blue)
- **Text Decoration**: `underline`
- **Font Size**: `15px`
- **Font Weight**: `400`
- **Cursor**: `pointer`
- **Hover State**: color `#1E63D8` (darker blue), text-decoration `underline`
- **Active State**: color `#1550BB`

### Status & Semantic Components

#### Badge / Tag
- **Background**: `#EEEFE9` (light gray)
- **Color**: `#374151` (stone gray)
- **Padding**: `4px 8px`
- **Font Size**: `12px`
- **Font Weight**: `500`
- **Border Radius**: `4px`
- **Success Variant**: background `rgba(0, 255, 0, 0.1)`, color `#00DD00` (bright green, slightly dimmed)
- **Warning Variant**: background `rgba(241, 168, 44, 0.1)`, color `#F1A82C`
- **Error Variant**: background `rgba(233, 47, 47, 0.1)`, color `#E92F2F`

#### Alert / Toast
- **Padding**: `12px 16px`
- **Border Radius**: `4px`
- **Font Size**: `14px`
- **Border Left**: `4px solid`
- **Success**: background `rgba(0, 255, 0, 0.05)`, border-left-color `#00FF00`, text color `#23251D`
- **Warning**: background `rgba(241, 168, 44, 0.05)`, border-left-color `#F1A82C`, text color `#23251D`
- **Error**: background `rgba(233, 47, 47, 0.05)`, border-left-color `#E92F2F`, text color `#23251D`

## 5. Layout Principles

### Spacing System

**Base Unit**: `4px`

**Spacing Scale**:
- `4px` — Tight internal spacing, micro-interactions
- `8px` — Button padding, small component gaps
- `12px` — Form label margins, small section spacing
- `16px` — Standard padding, card internals
- `24px` — Section margins, medium rhythm
- `32px` — Large padding, card padding, subsection breaks
- `48px` — Headline spacing, prominent breaks
- `64px` — Major section spacing, layout rhythm
- `120px` — Full-page section separation

**Usage Context**:
- **Buttons**: `8px` horizontal, `8px` vertical (32px height)
- **Cards**: `16px` internal, `24px` external gap
- **Forms**: `12px` label-to-input, `16px` field-to-field
- **Sections**: `48px`–`64px` between major content blocks

### Grid & Container

- **Max Width**: `1440px` (full desktop viewport support)
- **Standard Container**: `896px` (primary content width for readability)
- **Sidebar Layout**: 2-column (left: `240px` sidebar, right: content fluid)
- **Column Strategy**: 12-column grid at desktop; 6-column at tablet; single column mobile
- **Gutter**: `24px` between columns
- **Section Pattern**: Full-width hero (hero image + text overlay) → Container (grid content) → Full-width CTA → Footer

### Whitespace Philosophy

PostHog's spacing philosophy prioritizes breathing room and cognitive clarity. Whitespace is treated as an active design element—not empty space, but intentional silence that allows content to be parsed quickly. Sections are generously separated (48px–64px minimum), internal padding within cards is consistent (16px–32px), and text blocks never feel cramped. This approach supports the developer audience, who benefit from scannable layouts and clear content separation.

### Border Radius Scale

- `0px` — Cards, major containers, hero sections (sharp, contemporary aesthetic)
- `4px` — Buttons, inputs, code blocks, badges, alerts (subtle rounding, functional)
- `6px` — Navigation buttons, secondary interactive elements (slightly softer)
- `8px` — Large modals, overlays, accent containers (generous rounding, focus)

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| **None (Flat)** | No shadow, borders only | Text, buttons, flat lists, minimal surfaces |
| **Subtle** | `0px 4px 12px rgba(0, 0, 0, 0.08)` | Standard cards, form groups, slight lift |
| **Medium** | `0px 20px 25px -5px rgba(0, 0, 0, 0.1), 0px 8px 10px -6px rgba(0, 0, 0, 0.1)` | Modals, popovers, elevated surfaces |
| **Deep** | `0px 0px 6px 2px rgba(0, 0, 0, 0.2)` | Full-page overlays, critical modals, high-priority surfaces |

**Shadow Philosophy**

PostHog uses depth sparingly and purposefully. Shadows are soft, diffused, and applied to create subtle lift—never harsh or dramatic. This approach keeps the interface feeling lightweight and technical while still providing clear depth cues. Elevation is reserved for truly elevated UI (modals, popovers) rather than applied liberally. The `rgba(0, 0, 0, 0.08)–0.2` opacity range ensures shadows remain legible on both light and warm backgrounds, maintaining the earthy aesthetic while preserving contrast.

## 7. Do's and Don'ts

### Do

- **Use Open Runde for headlines** and brand-prominent display text; it carries authority and draws the eye
- **Prioritize the warm taupe (`#4D4F46`) and deep charcoal (`#23251D`)** for all body text and primary UI elements
- **Apply generous spacing** (24px–64px) between major sections; white space is your friend
- **Reserve bright blue (`#2F80FA`) exclusively for interactive elements** (links, active states, CTAs) to maintain focus hierarchy
- **Use semantic colors consistently**: green for success, amber for warning, red for error—every time, no exceptions
- **Keep buttons and interactive elements at least 32px tall** to ensure comfortable touch and click targets
- **Apply subtle shadows (0.08–0.1 opacity)** to cards and containers for gentle lift; avoid harsh drops
- **Maintain sharp borders (0px radius) on major containers** for a contemporary, built-for-builders aesthetic
- **Test color contrast ratios** (WCAG AA minimum 4.5:1 for text, 3:1 for graphics) to ensure accessibility
- **Use code blocks with monospace fonts** (`Source Code Pro` or `ui-monospace`) for technical content; never use proportional fonts for code

### Don't

- **Don't use pure white (`#FFFFFF`) as body text color**; always layer charcoal or taupe for legibility on light backgrounds
- **Don't apply rounded corners (>6px) to major UI containers**; the sharp aesthetic is intentional and core to brand identity
- **Don't mix Open Runde and IBM Plex Sans Variable** in the same logical section; use Open Runde for hierarchy, IBM Plex for body
- **Don't apply shadows to flat buttons or inline text links**; depth is reserved for elevated surfaces
- **Don't use accent colors (blue, orange, red) for body copy**; they are strictly for interactive and status states
- **Don't create spacing that breaks the 4px grid** (e.g., 13px, 27px); always use multiples of the 4px base unit
- **Don't exceed 40px of padding inside a card**; it becomes wasteful and breaks visual density
- **Don't apply multiple shadows to a single element**; layer shadows are for depth relationships only
- **Don't change link colors on hover to anything other than a darker shade of blue**; consistency is critical
- **Don't reduce font size below 12px** for any user-facing text; smaller text is inaccessible

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|------------|
| **Mobile** | `< 640px` | Single-column layout, `12px` section spacing, full-width cards, stack navigation vertically, reduce padding to `12px 16px` |
| **Tablet** | `640px – 1024px` | 2-column flexible layout, `24px` section spacing, standard button sizing maintained, sidebar if present becomes collapsible |
| **Desktop** | `1024px – 1440px` | Full 3-column capability, `32px–48px` section spacing, 896px container width, horizontal navigation active |
| **Wide** | `> 1440px` | Centered content with side gutters, max-container maintained, additional breathing room on sides |

### Touch Targets

- **Minimum height**: `44px` for all touch-interactive elements (buttons, links, form inputs)
- **Minimum width**: `44px` for square interactive elements (icon buttons, close buttons)
- **Minimum padding**: `8px` horizontal for small buttons and compact UI
- **Spacing between targets**: Minimum `8px` gap between adjacent touch areas to prevent mis-taps
- **Hover-only elements**: Never hide critical content behind hover states; always provide an alternative on mobile (e.g., expand on tap)

### Collapsing Strategy

- **Navigation**: Horizontal at desktop (16px spacing) → Hamburger menu at tablet (768px) → Collapsed drawer at mobile
- **Card layouts**: 3-column grid at desktop → 2-column at tablet (800px) → Single column at mobile (640px)
- **Padding**: `32px` desktop → `24px` tablet → `16px` mobile
- **Font sizes**: Hold at standard size until mobile (< 640px); consider reducing body to `14px` if extreme space constraints
- **Hero sections**: Full-height desktop with image + overlay → 60% height tablet → 40% height mobile with adjusted image
- **Modals**: Full-width minus gutters on mobile (16px each side); maintain max-width constraints on desktop

## 9. Agent Prompt Guide

### Quick Color Reference

- **Primary CTA**: Button Amber (`#CD8407`)
- **Interactive/Links**: Bright Blue (`#2F80FA`)
- **Background/Surface**: White (`#FFFFFF`)
- **Heading Text**: Deep Charcoal (`#23251D`)
- **Body Text**: Warm Taupe (`#4D4F46`)
- **Disabled/Secondary**: Light Gray (`#EEEFE9`)
- **Border**: Pale Gray (`#BFC1B7`)
- **Success**: Lime Green (`#00FF00`)
- **Warning**: Warm Amber (`#F1A82C`)
- **Error**: Danger Red (`#E92F2F`)

### Iteration Guide

1. **Always start with Open Runde for any headline** (h1, h2, h3); fallback to IBM Plex Sans Variable for body text. Never mix for the same hierarchical level.

2. **Every interactive element must be at least 32px tall** and use primary button amber (`#CD8407`) or ghost styling (`rgba(0,0,0,0)` background). Hover states scale to `1.02` and darken borders.

3. **Spacing always follows the 4px base unit scale**: use `8px`, `16px`, `24px`, `32px`, `48px`, or `64px` for margins and padding. Never improvise intermediate values.

4. **Cards and containers use 0px border radius** (sharp corners) and `1px solid #BFC1B7` borders with subtle shadow `0px 4px 12px rgba(0, 0, 0, 0.08)`. Exceptions only for code blocks and badges (4px).

5. **Text always maintains contrast**: body copy is either Warm Taupe (`#4D4F46`) or Stone Gray (`#374151`); never use colors below 5.5:1 WCAG contrast ratio on white backgrounds.

6. **Links are Bright Blue (`#2F80FA`) with underline by default**; on hover, shift to `#1E63D8` (darker blue). For navigational links, apply same color but may omit underline if in header context.

7. **Status colors are semantic and non-negotiable**: green for success, amber for warning, red for errors. Apply via background tint (10% opacity) + solid text color.

8. **Forms use 4px border radius** for inputs, 12px margin below labels, and focus state blue box-shadow `0 0 0 3px rgba(47, 128, 250, 0.1)`. Placeholder text is always Mid Gray (`#9EA096`).

9. **Mobile-first collapsing**: Design for 640px width first, then expand. Use hamburger navigation, single-column cards, 16px padding on mobile; maintain 32px button sizing throughout.

10. **Every UI element under 14px font size uses IBM Plex Sans Variable weight 500** (bolder for clarity at small size). Body copy and larger use weight 400.
