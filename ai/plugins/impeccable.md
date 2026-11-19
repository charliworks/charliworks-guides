# Impeccable

> Type: skill + plugin + CLI · Source: [pbakaus/impeccable](https://github.com/pbakaus/impeccable) · Docs: [impeccable.style](https://impeccable.style) · Version: _record on install_
> Last reviewed: 2026-11 · Use on: web (primary), mobile UI (advisory) · Status: Adopted

## What it's for

Design guidance for AI coding agents. It gives the AI real design vocabulary, a set of slash commands to steer UI work (for example `/audit`, `/polish`, `/typeset`), and anti-pattern detection, so AI-generated UI doesn't look generic. It works across Claude Code, Cursor, Codex CLI, Gemini CLI, and other tools. Apache-2.0.

## When to use / when not to

- ✅ Any web UI work: new screens, redesigns, and the design pass before a UI is called done
- ✅ Design critique when you can no longer judge your own screens
- ❌ Don't install it alongside [frontend-design](frontend-design.md) in the same project, because they overlap
- ❌ Not a replacement for testing with real users

## Install

Pick **one** method:

```bash
# Option A: from the project root (works across supported AI tools)
npx impeccable install

# Option B: Claude Code plugin
/plugin marketplace add pbakaus/impeccable
# then open /plugin and install Impeccable
```

Afterward, run the project design-context setup once inside your AI tool. Current docs use `/impeccable init`; older versions used `/impeccable teach`. Check `/help` or the docs for your installed version.

## Our workflow

1. **Kickoff**: run the design-context setup once and describe the product, its users, and the brand ([brand](../../design/brand.md)). Commit the context file it creates.
2. **Building**: build the UI using our [styling](../../design/styling.md) tokens.
3. **Before the PR**: run an audit on the changed screens, fix the findings or knowingly accept them, then use polish for refinements.
4. **CI (optional)**: the CLI detector (`npx impeccable detect <path-or-url>`) can scan files or URLs for anti-patterns. Try it before wiring it into CI.
5. Turn the fixes into **design tokens**, not one-off overrides, so they stay fixed.

## Project config

- The design-context file (e.g. `.impeccable.md`): **commit it**. Updates don't overwrite it.
- Installed skill files: commit them if the whole project should share the same setup.

## Vetting notes

- Open source (Apache-2.0), actively maintained, widely used.
- Some install paths add a **hook**. Read what it runs before trusting it ([vetting](../vetting.md)).
- Vetted: 2026-11.

## Gotchas

- The command list grows between versions. Trust `/help` over this page, and update this page when they differ.
- Browser-based features target web pages. For native mobile, use it for critique and vocabulary only.
