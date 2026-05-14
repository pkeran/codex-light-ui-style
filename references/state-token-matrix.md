# State Token Matrix

Use this file when a task needs consistent component states across buttons, navigation, inputs, badges, rows, tabs, and other interactive elements.

## Core Principle

State changes should feel precise, obvious, and calm. They should not depend on glow, dramatic saturation jumps, or oversized motion.

## Global State Tokens

| State | Surface | Text/Icon | Border | Shadow | Notes |
|---|---|---|---|---|---|
| default | `panel` / transparent | `text-primary` or `text-secondary` | `border` | none or soft | Base operational state |
| hover | `accent-soft` or slight tonal shift | `accent-strong` or `text-primary` | `border` | none | Acknowledge intent lightly |
| active / selected | `active-bg` | `accent-strong` | `accent-soft` or `border` | none | Clear but not glowing |
| focus | `panel` | inherit | `focus-ring` | none | Use crisp border/ring |
| disabled | inherit | reduced emphasis | inherit | none | Lower contrast carefully, do not hide |
| error | pale semantic tint | readable semantic text | semantic border | none | Stay calm and local |

## Button Matrix

| Variant | Default | Hover | Active | Focus | Disabled |
|---|---|---|---|---|---|
| quiet/default | white surface, border, dark text | pale-blue surface, blue or dark text | pale-blue surface, stronger blue text | crisp ring/border | reduce opacity, keep readable |
| primary | solid blue, white text | stronger blue, white text | slightly deeper blue | crisp ring around primary shape | mute but keep button visible |
| destructive | use only when needed, keep restrained | slightly stronger semantic tone | slightly deeper tone | crisp semantic ring | same disabled discipline |

## Navigation Matrix

| State | Surface | Text/Icon |
|---|---|---|
| inactive | transparent | muted gray-blue |
| hover | pale-blue or soft tonal shift | stronger text/icon |
| active | pale-blue | accent blue |
| focus | may match active or use ring | clearly visible |

Do not use a heavy dark-blue slab as the default active behavior.

## Input Matrix

| State | Surface | Border | Text |
|---|---|---|---|
| default | white | neutral border | primary text |
| hover | white | slightly stronger border | primary text |
| focus | white | focus-ring | primary text |
| disabled | slightly muted surface | neutral border | muted text |
| error | white or very pale semantic tint | semantic border | primary text |

## Row / Table / List Item Matrix

| State | Surface | Notes |
|---|---|---|
| default | transparent or white | quiet baseline |
| hover | very subtle tonal shift | never overpower data |
| selected | pale-blue surface or structured border cue | should read as controlled selection |
| active/actionable | localized blue emphasis only | do not colorize entire data region unless necessary |

## Badge / Chip Matrix

| State | Surface | Text | Border |
|---|---|---|---|
| neutral | white or panel-soft | muted | border |
| active | active-bg | accent-strong | accent-soft |
| status | soft semantic tint | readable semantic text | soft semantic border |

## Motion Guidance by State

- Hover: `140ms` to `180ms`, small tonal shift only
- Active: no bounce, no glow burst
- Focus: immediate clarity over animation
- Disabled: no animated fade-out theatrics

## Anti-Patterns

- Hover only changes shadow while text and fill stay identical
- Focus is shown only through a large diffuse glow
- Active state relies on very saturated blue fills everywhere
- Disabled state becomes unreadable
- Error state turns the component into a loud red block
