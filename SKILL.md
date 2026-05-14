---
name: codex-light-ui-style
description: Use when a user wants a UI, dashboard, admin panel, tool page, or component restyled toward a light Codex-like aesthetic with cool white-blue tones, restrained borders, subtle shadows, and low-noise visual polish. Use for color direction, card/button/sidebar styling, icon tone, and avoiding dark, neon, glassy, or overly decorative results.
---

# Codex Light UI Style

## Overview

Apply a cool white-blue visual system inspired by Codex app aesthetics without copying Codex layouts or features. Keep the result bright, low-saturation, calm, and tool-like rather than flashy, neon, glassy, or marketing-heavy.

`DESIGN.md` is the normative source of truth for tokens and high-level style rules. Use the reference files only when you need more detail.

## When to Use

- Use when the user asks for a Codex-like visual tone
- Use when a dashboard, admin panel, tool page, or settings surface feels too dark, too blue, too loud, or too decorative
- Use when colors, borders, shadows, cards, buttons, navigation, or iconography need a cleaner visual system
- Use when the goal is a professional desktop-tool feeling rather than a landing-page feeling

Do not use this skill when the user explicitly wants:

- dark mode
- brutalist or high-contrast styling
- strong gradients as the primary motif
- glassmorphism or heavy translucency
- a brand palette that conflicts with cool white-blue tones

## Workflow

1. Read `DESIGN.md` first.
2. If the task changes buttons, navigation, cards, tables, drawers, forms, or other UI parts, read `references/component-families.md`.
3. If the task is about overview pages, list-detail workbenches, settings, history, or operations surfaces, read `references/app-surface-patterns.md`.
4. If the task includes visible copy, labels, badges, counters, headings, or empty states, read `references/writing-tone.md`.
5. If the task touches hover, active, focus, disabled, contrast, or state visibility, read `references/accessibility-rules.md`.
6. If the output starts drifting toward glow, noise, over-styling, or generic AI dashboard aesthetics, read `references/do-dont.md`.
7. Before finishing, run through `references/quality-gates.md` and `references/review-rubric.md`.

## Implementation Priorities

When applying this style to an existing interface, prefer this order:

1. Normalize color variables and surfaces
2. Normalize panel, card, and border treatment
3. Normalize button hierarchy and navigation states
4. Normalize icon tone and interactive states
5. Remove loud gradients, heavy shadows, glass, and visual noise

## Reusable Prompt Template

```text
Restyle this UI toward a light Codex-like visual system. Use bright, low-saturation, cool white-blue tones with restrained borders, subtle shadows, and low-noise surfaces. Keep the background in cold white or very pale blue-white, keep cards mostly pure white with thin borders, and use accent blue only for active states and primary actions. Favor linear icons, pale blue active navigation, white default buttons with pale blue borders, and solid blue primary buttons with white text. Avoid dark heavy blue panels, neon gradients, glow effects, and glassmorphism.
```

## Deliverables

Prefer outputs that include one or more of:

- normalized color tokens
- semantic state tokens
- updated card / panel / button / navigation rules
- app-surface pattern alignment
- concise rationale for visual changes
- a short review pass against `references/quality-gates.md`

## Common Mistakes

- Treating accent blue as a page background instead of an emphasis color
- Solving hierarchy with shadow instead of borders and tonal contrast
- Putting gradients inside normal cards
- Making everything rounded, glowy, or soft without enough structure
- Producing a marketing hero look instead of a professional workbench feel

When unsure, bias toward:

- lighter
- simpler
- flatter
- calmer
- whiter
- more bordered
- less decorative
