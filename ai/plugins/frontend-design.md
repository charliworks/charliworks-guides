# frontend-design (Anthropic)

> Type: skill · Source: [anthropics/skills, frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) · Version: _record on install_
> Last reviewed: 2026-11 · Use on: web · Status: Alternative to Impeccable

## What it's for

Anthropic's official skill that pushes Claude toward distinctive, intentional UI instead of templated defaults. Impeccable was originally built on top of it.

## When to use / when not to

- ✅ Lightweight projects where you want better design defaults without the extra commands
- ✅ When Impeccable's extra tooling (CLI, hooks) isn't wanted
- ❌ Not together with [Impeccable](impeccable.md) in the same project

## Install

In Claude Code, open `/plugin` and install it from the official marketplace, or copy the skill folder from the repo into `.claude/skills/`. Record the exact method you used here.

## Our workflow

Same as Impeccable: build with our [styling](../../design/styling.md) tokens, then do a manual design pass against the styling and [accessibility](../../design/accessibility.md) checklists before the PR.

## Vetting notes

Official Anthropic source. Instructions only, no hooks. Vetted: 2026-11.
