# Context7

> Type: MCP server / plugin · Source: [upstash/context7](https://github.com/upstash/context7) · Version: _record on install_
> Last reviewed: 2026-11 · Use on: all · Status: Adopted

## What it's for

It fetches current, version-specific library documentation and code examples into the AI's context, so the AI stops using outdated or invented APIs.

## When to use / when not to

- ✅ Any work with a framework or library, especially ones that change fast
- ❌ Don't use it for private or internal code. It covers public libraries.

## Install

```bash
# Claude Code: official marketplace
/plugin install context7@claude-plugins-official
```

## Our workflow

When asking for code that uses a library, say "use Context7 for <library> <version>". Pin the version that matches the project's lockfile.

## Vetting notes

The MCP server code is open source, but documentation queries go to a hosted backend, so **don't put secrets or private code in queries**. Vetted: 2026-11.
