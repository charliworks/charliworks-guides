# Playwright MCP

> Type: MCP server · Source: [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) · Version: _record on install_
> Last reviewed: 2026-11 · Use on: web · Status: Adopted

## What it's for

It gives the AI a real browser so it can navigate, click, fill forms, and check app behavior.

## When to use / when not to

- ✅ Reproducing bugs, smoke-testing a flow, checking UI after changes
- ✅ Drafting Playwright test files that run in CI
- ❌ Don't point it at production with real accounts or real payments
- ❌ It doesn't replace committed tests. Save what it finds as test files ([testing](../../engineering/testing.md)).

## Install

```bash
# As an MCP server (runs locally)
npx @playwright/mcp@latest
```

Or install the Playwright plugin from the Claude Code `/plugin` marketplace. Record the method used.

## Our workflow

1. Run the app locally or on a preview deploy.
2. Ask the AI to walk the flow and report problems.
3. Turn the confirmed checks into `*.spec.ts` tests in the repo.

## Vetting notes

Official Microsoft project. Runs a browser locally, and any page it opens can try to influence the AI, so only point it at your own apps. Vetted: 2026-11.
