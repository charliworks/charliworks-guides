# Superpowers

> Type: plugin (skills) · Source: [obra/superpowers](https://github.com/obra/superpowers) · Version: _record on install_
> Last reviewed: 2026-11 · Use on: all · Status: Trial

## What it's for

A set of skills that makes the AI follow a disciplined engineering process (brainstorm → plan → execute with tests → review) instead of improvising.

## When to use / when not to

- ✅ Large features or new projects where planning pays off
- ✅ When you want test-driven discipline from the AI
- ❌ Small fixes or one-line changes, where the extra process slows you down

## Install

```bash
# Claude Code: official marketplace
/plugin install superpowers@claude-plugins-official
```

Check the repo README for the current install method if this one fails.

## Our workflow

Use it to turn a [spec](../../project-management/templates/spec.md) into an implementation plan. Save the plan to `docs/plans/` and review it before execution, as described in [planning](../../project-management/planning.md). The plan still has to follow our branching, commit, and DoD rules.

## Vetting notes

Open source (MIT), widely used. Skim the skills before trusting it. Vetted: 2026-11.

## Gotchas

Its process can conflict with ours on details (branch names, commit style). Ours wins. Tell it to follow `AGENTS.md`.
