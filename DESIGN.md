---
version: alpha
name: Codex Light UI Style
description: Light cool white-blue design system for professional tool UIs inspired by Codex app aesthetics.
colors:
  primary: "#339CFF"
  primary-strong: "#2F91FF"
  primary-soft: "#EAF4FF"
  neutral-0: "#FFFFFF"
  neutral-25: "#F8FBFF"
  neutral-50: "#F7FAFD"
  neutral-75: "#F5F8FC"
  neutral-300: "#DCE7F3"
  neutral-700: "#687386"
  neutral-950: "#171A1F"
  bg: "#F7FAFD"
  bg-alt: "#F5F8FC"
  panel: "#FFFFFF"
  panel-soft: "#F8FBFF"
  border: "#DCE7F3"
  text-primary: "#171A1F"
  text-secondary: "#687386"
  accent: "#339CFF"
  accent-strong: "#2F91FF"
  accent-soft: "#EAF4FF"
  active-bg: "#DDEEFF"
  gradient-start: "#F8FBFF"
  gradient-end: "#EEF5FC"
states:
  hover-surface: "#EAF4FF"
  active-surface: "#DDEEFF"
  focus-ring: "#B7D9FF"
  disabled-opacity: "0.52"
  transition-fast: "140ms"
  transition-normal: "180ms"
elevation:
  flat: "none"
  soft: "0 8px 24px rgba(120, 160, 210, 0.08)"
  overlay: "0 16px 40px rgba(116, 150, 194, 0.14)"
typography:
  headline-lg:
    fontFamily: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
    fontSize: 24px
    fontWeight: 650
    lineHeight: 1.2
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: -0.01em
  body-sm:
    fontFamily: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0
  label-md:
    fontFamily: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: -0.01em
rounded:
  sm: 12px
  md: 14px
  lg: 18px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  2xl: 32px
components:
  button-default:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text-primary}"
    borderColor: "{colors.border}"
    rounded: "{rounded.full}"
    typography: "{typography.label-md}"
    padding: 14px
    transitionDuration: "{states.transition-normal}"
  button-default-hover:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.accent-strong}"
    borderColor: "{colors.border}"
    rounded: "{rounded.full}"
    typography: "{typography.label-md}"
    padding: 14px
    transitionDuration: "{states.transition-normal}"
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    typography: "{typography.label-md}"
    padding: 14px
    transitionDuration: "{states.transition-normal}"
  button-primary-hover:
    backgroundColor: "{colors.accent-strong}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    typography: "{typography.label-md}"
    padding: 14px
    transitionDuration: "{states.transition-normal}"
  card-default:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text-primary}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: 24px
    shadow: "{elevation.soft}"
  input-default:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text-primary}"
    borderColor: "{colors.border}"
    rounded: "{rounded.md}"
    typography: "{typography.body-md}"
    padding: 14px
  input-focus:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text-primary}"
    borderColor: "{states.focus-ring}"
    rounded: "{rounded.md}"
    typography: "{typography.body-md}"
    padding: 14px
  nav-item:
    backgroundColor: "transparent"
    textColor: "{colors.text-secondary}"
    rounded: "{rounded.md}"
    padding: 12px
  nav-item-active:
    backgroundColor: "{colors.active-bg}"
    textColor: "{colors.accent-strong}"
    rounded: "{rounded.md}"
    padding: 12px
  icon-default:
    textColor: "{colors.text-secondary}"
  icon-active:
    textColor: "{colors.accent}"
  badge-neutral:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.text-secondary}"
    borderColor: "{colors.border}"
    rounded: "{rounded.full}"
    typography: "{typography.body-sm}"
    padding: 8px
  badge-active:
    backgroundColor: "{colors.active-bg}"
    textColor: "{colors.accent-strong}"
    borderColor: "{colors.accent-soft}"
    rounded: "{rounded.full}"
    typography: "{typography.body-sm}"
    padding: 8px
---

# Codex Light UI Style

## Overview

Codex Light UI Style is a restrained desktop-tool visual system built around cool whites, pale blue neutrals, and precise blue emphasis. The interface should feel professional, dependable, and easy to scan, more like a focused workbench than a marketing surface.

Use these five high-level principles as the fallback rule set whenever a more specific token or component rule is not enough:

1. 冷白为底，蓝色只是强调，不是背景主角。
2. 组件更像专业工作台，不像营销展示卡。
3. 边框比阴影更重要。
4. 渐变只属于大背景，不属于普通卡片。
5. 激活态强调清晰，但不过度发光。

The desired emotional output is calm clarity: bright, low-saturation, lightly structured, and operationally confident. The UI should avoid looking playful, glossy, over-decorated, or “AI-generated by default.”

## Colors

The palette is led by cold white surfaces and one clear blue emphasis range.

- **Background (`#F7FAFD` / `#F5F8FC`)** forms the workspace field and should stay bright.
- **Panel (`#FFFFFF`)** is the default surface for cards, drawers, and major containers.
- **Panel Soft (`#F8FBFF`)** is for secondary surfaces, grouped sections, and subtle contrast.
- **Border (`#DCE7F3`)** is a structural color and should often carry hierarchy more than shadow.
- **Text Primary (`#171A1F`)** is reserved for high-legibility headings and core copy.
- **Text Secondary (`#687386`)** is used for metadata, helper text, and inactive interface chrome.
- **Accent (`#339CFF`, `#2F91FF`)** should be used sparingly for primary actions, active states, and status emphasis.
- **Accent Soft (`#EAF4FF`)** and **Active Background (`#DDEEFF`)** should create soft interaction surfaces without visual noise.

Allow only one broad, very soft background gradient:

`linear-gradient(180deg, #F8FBFF 0%, #EEF5FC 100%)`

Do not turn normal cards, panels, or common components into gradient objects.

## Surfaces & Hierarchy

Surface hierarchy should be semantic, not theatrical.

- **Workspace background** stays cold white or pale blue-white.
- **Primary panels** are white and carry most functional content.
- **Secondary surfaces** may step slightly cooler or softer to group controls.
- **Overlay surfaces** may use slightly stronger elevation, but they still belong to the same color family.

The preferred stack is:

1. tonal separation
2. thin borders
3. spacing
4. typography
5. shadow only where still needed

## Typography

Typography should feel crisp, modern, and operational. Prefer a strong system-sans stack over expressive or novelty typography.

- Headlines are slightly condensed through negative tracking and heavier weights.
- Body text stays compact, readable, and neutral.
- Labels and controls should feel precise, not shouty.
- Prefer two to three visible size tiers per screen rather than large type-scale jumps.

The system should read like a professional tool, not an editorial spread or a startup landing page.

## Layout & Density

Layout should prioritize scan speed and containment.

- Use a consistent 4px / 8px-derived spacing rhythm.
- Group related content into bright surfaces with generous but not wasteful padding.
- Keep horizontal alignment disciplined.
- Prefer structured sections, toolbars, cards, and rails over floating ornamental clusters.
- Leave enough whitespace to reduce noise, but do not create empty “hero” zones that weaken operational density.

Different app surfaces may use different density, but the same structural language must persist across overview dashboards, workbenches, settings, logs, and forms.

## Elevation & Depth

Depth is secondary. Structure should come from tonal separation and borders first.

- Use `1px` borders widely and consistently.
- Shadows should remain light and soft:
  - `0 8px 24px rgba(120, 160, 210, 0.08)` or lighter
- Use stronger shadows only for overlays that truly need separation.
- Avoid bloom, glow, neon rims, and floating “glass card” stacks.

If a UI feels under-structured, add border clarity and tonal contrast before increasing shadow.

## Shapes

The shape language should feel contemporary and controlled.

- Standard controls: `12px` to `14px` radius
- Primary cards and panels: `18px` radius
- Pills and CTA buttons: fully rounded when they read as controls rather than containers

Do not mix many unrelated radius styles on one screen. The system should feel coherent and engineered.

## Interaction States

Interactive states should feel precise and visible.

- Hover should lightly acknowledge intent, usually through pale-blue or tonal change.
- Active should read clearly through pale-blue surfaces and blue text/icon emphasis.
- Focus should rely on crisp outline or border reinforcement, not glowing halos.
- Disabled should remain legible and understandable without collapsing into invisibility.

State transitions should be short and quiet. Prefer roughly `140ms` to `180ms` timing.

## Motion

Motion should be almost invisible.

- Prefer soft fades, slight translate, or small tonal shifts.
- Avoid springy, bouncy, or playful motion language.
- Avoid large cinematic entrance animations.
- If motion attracts more attention than the content, it is too strong.

## Components

Component styling should reinforce the five high-level principles.

- **Buttons:** Default buttons are white with pale blue borders. Primary buttons are solid blue with white text. Hover states should brighten or deepen slightly, not glow.
- **Navigation:** Active items use a pale blue background and accent text. Inactive items remain calm and gray-blue. Avoid heavy dark active slabs.
- **Cards:** Cards are mostly pure white with thin borders, a large but disciplined radius, and very light shadow or none.
- **Icons:** Prefer linear icons. Default icon tone is gray-blue; active states use accent blue.
- **Forms:** Inputs should preserve the same bright-white, thin-border treatment as cards. Focus is communicated with border clarity, not giant outer glows.
- **Lists / tables / toolbars:** Keep them clean, lightly separated, and operational. Avoid decorative backgrounds that compete with the data.

For extended component rules, read `references/component-families.md`.

## App Surface Patterns

This design language should scale across multiple app scenarios:

- overview dashboard
- list/detail workbench
- settings/configuration
- history/log activity surfaces
- forms and data entry
- drawers and inspectors

For those patterns, read `references/app-surface-patterns.md`.

## Do's and Don'ts

### Do

- Do keep cold white backgrounds as the dominant field.
- Do use blue as emphasis, not as the main page fill.
- Do prefer borders and soft tonal separation over heavy shadow stacks.
- Do reserve gradients for broad, quiet background treatment only.
- Do make active states obvious through pale-blue surfaces and clean blue accents.
- Do keep components feeling like professional workbench elements.

### Don't

- Don’t turn the app into a deep-blue dashboard.
- Don’t make ordinary cards gradient objects.
- Don’t solve hierarchy by making every block glow.
- Don’t use heavy glassmorphism or translucent blur as a default material.
- Don’t make components feel like hero banners, promo modules, or ad tiles.
- Don’t let active states become neon or over-lit.
