# Setup: Claude Code

> Last reviewed: 2026-11 · Status: 🚧 Draft

## Per project

1. Copy [AGENTS.template.md](../../templates/AGENTS.template.md) to the repo root as `AGENTS.md`, and add a `CLAUDE.md` that says "Follow AGENTS.md".
2. Copy the charliworks skills you need from [ai/skills/](../skills/) into `.claude/skills/`.
3. Install the plugins from the project's [stack profile](stack-profiles.md). Most are added with `/plugin` (browse or install from a marketplace).
4. Set permissions so the tool must ask before `git push`, destructive shell commands, and installing dependencies ([usage-rules](../usage-rules.md)).
5. Commit `.claude/skills/` and any project settings meant to be shared. Keep personal or local settings gitignored.

## Tips

- Use `/plugin` to see what's installed, and uninstall what you don't use.
- Keep `AGENTS.md` short and link to these guides rather than copying them.
