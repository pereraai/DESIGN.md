# DESIGN.md — Spotify

## Overview
Spotify's design system is built for immersive media consumption. The signature green is used sparingly — primarily for CTAs and the shuffle/play icon — while a near-black foundation lets album art become the visual hero. Circular, Spotify's custom typeface, gives all text a distinctive rounded warmth.

## Colors

### Primary Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `color-brand` | `#1DB954` | CTAs, play button, active states |
| `color-bg` | `#191414` | App background |
| `color-text` | `#FFFFFF` | Primary text |
| `color-text-sub` | `#B3B3B3` | Subdued text, metadata |
| `color-surface` | `#282828` | Cards, elevated surfaces |

### Neutral Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `color-base` | `#191414` | App background |
| `color-elevated` | `#282828` | Cards |
| `color-highlight` | `#3E3E3E` | Hover states |
| `color-subdued` | `#535353` | Player track |
| `color-text-subdued` | `#B3B3B3` | Secondary text |

### Semantic Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `color-positive` | `#1DB954` | Active, playing state |
| `color-negative` | `#E91429` | Remove from library |
| `color-warning` | `#FFA42B` | Warning, alerts |

## Typography

| Role | Family | Size | Weight | Line Height |
|------|--------|------|--------|-------------|
| Display | Circular | 64px | 900 | 1.1 |
| Heading | Circular | 32px | 700 | 1.2 |
| Body | Circular | 16px | 400 | 1.5 |
| Caption | Circular | 12px | 400 | 1.4 |
| Track Title | Circular | 14px | 700 | 1.3 |

## Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `space-1` | 4px | Track meta gaps |
| `space-2` | 8px | Card inner spacing |
| `space-4` | 16px | Grid gap |
| `space-6` | 24px | Section padding |
| `space-8` | 32px | Header spacing |

## Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| `radius-sm` | 4px | Album art corners |
| `radius-md` | 8px | Cards |
| `radius-full` | 9999px | Avatars, progress bar |

## Elevation

| Level | Value | Usage |
|-------|-------|-------|
| `shadow-card` | `0 4px 16px rgba(0,0,0,0.5)` | Hovered cards |
| `shadow-overlay` | `0 8px 24px rgba(0,0,0,0.7)` | Now playing panel |

## Components

### Album Card
- Square album art (varies by grid), title + artist below
- Hover reveals green play button overlay
- Rounded 8px corners on artwork

### Now Playing Bar
- Fixed bottom bar, 90px height
- Track info left, controls center, volume right
- Progress bar: green on dark gray track

### Playlist Header
- Gradient background sampled from cover art
- Large cover, title, creator, duration stats
- Play and shuffle buttons

## Do's and Don'ts

### Do
- Let album art drive the visual palette per screen
- Use green only for primary interactive elements
- Use Circular at Black (900) weight for hero moments

### Don't
- Don't use green for backgrounds or large surfaces
- Don't crop album art into non-square shapes
- Don't use system fonts — Circular is core to the brand
