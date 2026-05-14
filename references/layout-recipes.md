# Layout Recipes

Use this file when a task needs not just styling but repeatable app-page composition patterns.

## General Layout Rule

Compose pages like workbenches, not landing pages.

- One clear primary workspace
- Quiet supporting surfaces
- Strong alignment
- Controlled density
- Minimal decorative emptiness

## Recipe 1: Overview Dashboard

### Structure

1. top summary surface
2. secondary status or KPI surfaces
3. recent activity / next actions / exports / alerts

### Styling guidance

- Use one strong overview panel, not a giant gradient hero
- KPI cards stay white and structural
- Let key numbers speak through typography and spacing before color
- Use blue only for one main action or selected state

### Good use cases

- repository overview
- export center
- operations dashboard
- inventory summary

## Recipe 2: List + Detail Workbench

### Structure

1. command bar
2. list/table region
3. detail drawer or side panel

### Styling guidance

- List region should feel neutral and data-first
- Detail pane may use slightly stronger elevation than the list
- Actions belong in toolbar, row actions, or detail pane, not scattered visually
- State cues should be local and restrained

### Good use cases

- account repository
- import queue
- export file list
- failure inspection

## Recipe 3: Settings / Configuration Surface

### Structure

1. small page summary
2. grouped settings cards
3. actions anchored near relevant settings block

### Styling guidance

- Keep settings cards bright and simple
- Use helper text sparingly and functionally
- Avoid making settings pages feel more decorated than operational pages
- Save/submit actions should be obvious but not loud

### Good use cases

- token refresh settings
- export options
- scan and import behavior
- automation policy

## Recipe 4: History / Logs / Activity Feed

### Structure

1. filters or tabs
2. dense event list
3. optional detail expansion or side inspector

### Styling guidance

- Prioritize scan speed
- Use subtle dividers and row rhythm
- Reserve stronger emphasis for failures, warnings, or active filters
- Keep metadata quiet but legible

### Good use cases

- operation history
- refresh logs
- failure reasons
- import/export activity

## Recipe 5: Form / Wizard / Import Flow

### Structure

1. intro or context card
2. primary input block
3. validation / preview / confirmation block
4. final action row

### Styling guidance

- Keep the main form surface bright and stable
- Use blue for one primary progression action
- Validation should feel informative, not punitive
- Avoid marketing-style steps or oversized illustrations

### Good use cases

- import JSON/ZIP
- export configuration
- batch repair or refresh flow

## Recipe 6: Drawer / Inspector / Side Utility

### Structure

1. header
2. summary block
3. grouped detail sections
4. local actions

### Styling guidance

- Preserve same border and radius language as main app
- Use slightly stronger shadow only if needed for separation
- Keep sections modular and vertically readable
- Avoid turning inspectors into dark floating consoles

### Good use cases

- account detail
- failure detail
- JSON preview
- metadata inspector

## Density Rules

- Overview surfaces: medium density
- Workbench/list surfaces: medium-high density
- Settings: medium density
- History/logs: high density but high clarity
- Drawers: medium density with strong grouping

## Anti-Patterns

- Empty hero banners on operational pages
- Equal visual emphasis on every card
- Toolbars that look louder than the content
- Lists with too much color and too many badge styles
- Settings pages that feel like promotional landing sections
