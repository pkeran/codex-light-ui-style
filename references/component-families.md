# Component Families

Use this file when the task changes concrete UI components rather than only broad color direction.

## Buttons

- Default: white fill, thin border, dark text
- Primary: solid accent blue, white text
- Secondary emphasis: pale-blue fill, accent text
- Avoid oversized shadows and glossy highlights
- Keep button groups visually aligned and similarly sized within one cluster

## Navigation

- Sidebars, tabs, pills, segmented controls, and menu rows should share the same active-state logic
- Active item: pale-blue surface + accent text/icon
- Inactive item: transparent or white surface + muted gray-blue text/icon
- Do not use a heavy dark block for active state unless the user explicitly asks for it

## Cards and Panels

- Standard cards: pure white background, thin border, `14px` to `18px` radius
- Use soft contrast between page background and panel background
- Only overlays and modal-like surfaces may justify slightly stronger depth
- Do not decorate utility cards like marketing feature blocks

## Forms and Inputs

- Inputs, selects, and textareas should align with the same panel language as cards
- Use bright surfaces, clear borders, and precise focus styling
- Error states should remain calm and legible, not aggressive or glowing
- Placeholder text must remain visibly secondary, not low-contrast to the point of disappearing

## Tables, Lists, and Rows

- Favor clean row rhythm and minimal separators
- Use subtle background changes for hover rather than saturated fills
- Badges and counters should act as metadata accents, not dominate the row
- Keep dense surfaces readable by relying on text hierarchy first

## Drawers, Dialogs, and Popovers

- Use white or near-white surfaces with clean borders
- Prefer stronger separation through backdrop contrast and controlled shadow rather than blur-heavy glass treatment
- Maintain the same radius family as cards

## Badges, Chips, and Status Tokens

- Default badge/chip: white or pale-blue fill with thin border
- Status badges may use soft semantic tints, but they should still belong to the same low-noise system
- Avoid over-saturated fills and overly thick outlines

## Empty States and Summary Blocks

- Keep empty states concise and operational
- Use icon + short label + next action pattern
- Do not turn empty states into marketing sections

## Toolbars and Control Bars

- Keep toolbars quiet and structured
- Group related actions with spacing and alignment, not loud background treatment
- Primary action may use accent blue, but surrounding controls should stay calm
