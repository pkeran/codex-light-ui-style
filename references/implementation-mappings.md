# Implementation Mappings

Use this file when the user wants the design language translated into real implementation decisions for CSS, Tailwind, shadcn/ui, or common app component stacks.

## Mapping Priority

Apply the system in this order:

1. semantic tokens
2. surface tokens
3. state tokens
4. component recipes
5. app-surface layout patterns

Do not jump straight to per-component styling without first defining tokens.

## CSS Variables Mapping

Start with global variables. Keep variable names semantic rather than page-specific.

```css
:root {
  --ui-bg: #F7FAFD;
  --ui-bg-alt: #F5F8FC;
  --ui-panel: #FFFFFF;
  --ui-panel-soft: #F8FBFF;
  --ui-border: #DCE7F3;
  --ui-text: #171A1F;
  --ui-text-muted: #687386;
  --ui-accent: #339CFF;
  --ui-accent-strong: #2F91FF;
  --ui-accent-soft: #EAF4FF;
  --ui-active-bg: #DDEEFF;
  --ui-focus-ring: #B7D9FF;
  --ui-shadow-soft: 0 8px 24px rgba(120, 160, 210, 0.08);
  --ui-shadow-overlay: 0 16px 40px rgba(116, 150, 194, 0.14);
  --ui-radius-sm: 12px;
  --ui-radius-md: 14px;
  --ui-radius-lg: 18px;
  --ui-duration-fast: 140ms;
  --ui-duration-normal: 180ms;
}
```

## Tailwind Mapping

Translate the design system into `theme.extend` entries rather than ad-hoc utility strings everywhere.

```ts
export default {
  theme: {
    extend: {
      colors: {
        ui: {
          bg: "#F7FAFD",
          "bg-alt": "#F5F8FC",
          panel: "#FFFFFF",
          "panel-soft": "#F8FBFF",
          border: "#DCE7F3",
          text: "#171A1F",
          muted: "#687386",
          accent: "#339CFF",
          "accent-strong": "#2F91FF",
          "accent-soft": "#EAF4FF",
          active: "#DDEEFF",
          focus: "#B7D9FF",
        },
      },
      borderRadius: {
        uiSm: "12px",
        uiMd: "14px",
        uiLg: "18px",
      },
      boxShadow: {
        uiSoft: "0 8px 24px rgba(120, 160, 210, 0.08)",
        uiOverlay: "0 16px 40px rgba(116, 150, 194, 0.14)",
      },
      transitionDuration: {
        uiFast: "140ms",
        uiNormal: "180ms",
      },
    },
  },
};
```

### Tailwind Usage Guidance

- Prefer `bg-ui-panel`, `border-ui-border`, `text-ui-text`, `text-ui-muted`
- Use `shadow-uiSoft` sparingly
- Avoid long one-off utility chains that bypass the token system

## shadcn/ui Mapping

If using shadcn/ui, map this style at the token/theme layer rather than rewriting every component from scratch.

### Recommended mapping

- `background` -> `ui-bg`
- `card` / `popover` -> `ui-panel`
- `muted` -> `ui-panel-soft`
- `border` -> `ui-border`
- `foreground` -> `ui-text`
- `muted-foreground` -> `ui-text-muted`
- `primary` -> `ui-accent`
- `primary-foreground` -> white
- `accent` -> `ui-accent-soft`
- `accent-foreground` -> `ui-accent-strong`

### shadcn/ui behavior guidance

- Default buttons should often use `outline` or quiet `secondary` treatment
- Primary buttons should be reserved for one main action per cluster
- Cards should stay plain and bright, not gradient-filled
- Dialogs and sheets may use slightly stronger shadow than cards, but still remain within the same material family

## Plain HTML / CSS Component Recipes

### Default button

```css
.btn {
  min-height: 40px;
  padding: 0 15px;
  border: 1px solid var(--ui-border);
  border-radius: 9999px;
  background: var(--ui-panel);
  color: var(--ui-text);
  transition:
    background var(--ui-duration-normal) ease,
    color var(--ui-duration-normal) ease,
    border-color var(--ui-duration-normal) ease,
    box-shadow var(--ui-duration-normal) ease;
}

.btn:hover {
  background: var(--ui-accent-soft);
  color: var(--ui-accent-strong);
}
```

### Primary button

```css
.btn-primary {
  background: var(--ui-accent);
  color: #fff;
  border-color: transparent;
}

.btn-primary:hover {
  background: var(--ui-accent-strong);
  color: #fff;
}
```

### Card

```css
.card {
  background: var(--ui-panel);
  border: 1px solid var(--ui-border);
  border-radius: var(--ui-radius-lg);
  box-shadow: var(--ui-shadow-soft);
}
```

### Navigation item

```css
.nav-item {
  color: var(--ui-text-muted);
  border-radius: var(--ui-radius-md);
}

.nav-item.is-active {
  background: var(--ui-active-bg);
  color: var(--ui-accent-strong);
}
```

## Stack-Specific Rules

### React component systems

- Keep tokens in one exported theme file
- Keep state variants predictable
- Avoid local hard-coded blues that bypass the system

### Vue / Svelte / template-first stacks

- Push tokens to root variables first
- Bind variant classes through semantic names such as `is-active`, `is-muted`, `is-primary`
- Avoid scattered inline style values

### Electron / desktop-style apps

- Favor denser but calmer layouts
- Use border clarity for pane separation
- Let sidebars and inspectors stay light rather than dark and immersive

## Anti-Patterns

- Hard-coding page-specific colors in components
- Solving every component with a custom gradient
- Mixing tokenized components with one-off visual experiments
- Treating primary blue as a brand wallpaper instead of a controlled accent
