# GitHub (plugin / MCP)

> Type: plugin / MCP server · Source: GitHub official MCP server · Version: _record on install_
> Last reviewed: 2026-11 · Use on: all · Status: Adopted

## What it's for

It lets the AI read and work with issues, PRs, and repo context.

## When to use / when not to

- ✅ Drafting issues from a spec, summarizing PR feedback, linking work to issues
- ❌ Don't let it merge PRs or push to `main` without your approval ([usage-rules](../usage-rules.md))

## Install

```bash
# Claude Code: official marketplace
/plugin install github@claude-plugins-official
```

Use a fine-grained token scoped to the charliworks org's repos, with the minimum permissions needed.

## Our workflow

- Issues follow [issue-tracking](../../workflow/issue-tracking.md) labels and templates.
- PRs follow [pull-requests](../../workflow/pull-requests.md) and the PR template.

## Vetting notes

Official GitHub source. The token's scope is the main risk, so keep it narrow. Vetted: 2026-11.
