# Accessibility Rules

Use this file when a UI change involves visible state, contrast, focus, readability, or interactive controls.

## Contrast

- Maintain at least WCAG AA contrast for body text and interactive labels
- Do not rely on pale blue text over pale blue surfaces for primary content
- Secondary text may be softer, but must remain comfortably readable

## State Visibility

- Hover, active, focus, selected, disabled, and error states must be visually distinct
- Blue alone should not be the only differentiator if structure can be improved with border, fill, or icon change
- Active states should be obvious without turning neon

## Focus Treatment

- Focus should read as precise and deliberate
- Prefer a clear border, ring, or outline that fits the accent system
- Avoid giant fuzzy outer glows

## Typography Readability

- Keep text hierarchy simple and consistent
- Do not compress dense admin interfaces by shrinking everything at once
- Small labels and metadata need enough contrast and spacing to remain scannable

## Surface Separation

- White cards on a pale background need enough border distinction to remain visually discrete
- If two surfaces visually merge, strengthen border clarity before increasing shadow

## Icon and Color Meaning

- Icons should not be the only signal for state
- Status color should be paired with text, shape, or placement cues
- Muted iconography must still remain visible at practical screen brightness
