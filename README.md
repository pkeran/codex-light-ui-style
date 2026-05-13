# Codex Light UI Style

Reusable light blue-white UI styling assets for Codex-compatible agents and prompt-driven front-end work.

## What this project contains

- `SKILL.md` — the agent-facing entrypoint
- `DESIGN.md` — the design-system source of truth
- `agents/openai.yaml` — UI metadata for skill discovery
- `references/` — component families, accessibility rules, do/don't rules, quality gates, writing tone
- `prompts/codex-light-ui-style.md` — copy-paste short and long prompts plus CSS token starter

## Visual intent

This project captures a restrained Codex-like desktop-tool aesthetic:

- cold white backgrounds
- blue as emphasis, not as the main page fill
- white cards with thin borders
- subtle shadows
- pale-blue active states
- low-noise, professional workbench feel

## Core principles

1. 冷白为底，蓝色只是强调，不是背景主角  
2. 组件更像专业工作台，不像营销展示卡  
3. 边框比阴影更重要  
4. 渐变只属于大背景，不属于普通卡片  
5. 激活态强调清晰，但不过度发光  

## Install as a local Codex skill

Copy this folder into your local Codex skills directory:

- Windows: `C:\Users\<you>\.codex\skills\codex-light-ui-style`
- Typical Unix-like path: `~/.codex/skills/codex-light-ui-style`

## Use it as a skill

Invoke it in a request like:

```text
Use $codex-light-ui-style to restyle this interface.
```

## Use it as a prompt

If you only need prompt-based reuse, open:

- `prompts/codex-light-ui-style.md`

and copy either the short or long prompt block.

## Repository layout

```text
.
├── SKILL.md
├── DESIGN.md
├── README.md
├── agents/
│   └── openai.yaml
├── prompts/
│   └── codex-light-ui-style.md
└── references/
    ├── accessibility-rules.md
    ├── component-families.md
    ├── do-dont.md
    ├── quality-gates.md
    └── writing-tone.md
```
