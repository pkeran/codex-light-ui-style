# List + Detail Example

Use this file when the user wants a repository page, inventory workbench, file list, queue inspector, or any list-plus-detail operational surface.

## Intent

This page type should feel data-first and task-oriented:

- a neutral list region
- a focused detail surface
- quiet but usable toolbars

## Recommended structure

1. command bar
2. list or table region
3. detail drawer / inspector / side panel
4. local row or bulk actions

## Surface behavior

- list rows should stay visually quiet
- hover changes should be subtle
- selected row can use pale-blue surface or structured highlight
- detail panel may use slightly stronger elevation than the list, but should remain within the same material family

## Suggested content blocks

- account list
- export file list
- failed import list
- history row detail
- selected record inspector

## Prompt-ready implementation note

If implementing this page, preserve:

- borders over shadows
- blue as selection and action emphasis only
- low-noise rows
- a bright inspector rather than a dark console panel

## Smell tests

The page is drifting if:

- rows use too many colored badges
- the toolbar looks louder than the data
- the detail pane becomes a separate aesthetic system
- selection state turns into a saturated full-row banner
