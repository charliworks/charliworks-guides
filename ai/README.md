# AI at charliworks

> Last reviewed: 2026-11

## Read first

1. [usage-rules](usage-rules.md): what AI may and may not do
2. [vetting](vetting.md): checklist before installing any plugin, skill, or MCP server
3. [setup/stack-profiles](setup/stack-profiles.md): which tools to install for each project type

## Which tool for which job

| Job | Tool | Page |
|---|---|---|
| Design quality, UI audit, polish | Impeccable *or* frontend-design (pick one per project) | [impeccable](plugins/impeccable.md), [frontend-design](plugins/frontend-design.md) |
| Structured plan → spec → test workflow | Superpowers | [superpowers](plugins/superpowers.md) |
| Up-to-date library docs | Context7 | [context7](plugins/context7.md) |
| Browser testing and bug reproduction | Playwright MCP | [playwright](plugins/playwright.md) |
| Issues, PRs, repo context | GitHub | [github](plugins/github.md) |
| Commit messages per our rules | charliworks `commit-writer` skill | [SKILL.md](skills/commit-writer/SKILL.md) |
| PR self-review against our DoD | charliworks `code-reviewer` skill | [SKILL.md](skills/code-reviewer/SKILL.md) |
| Starting a new project | charliworks `project-kickoff` skill | [SKILL.md](skills/project-kickoff/SKILL.md) |

## Folders

- `setup/`: per-tool setup (Claude Code, and others as they're adopted)
- `plugins/`: one page per **third-party** tool, using [_template.md](plugins/_template.md)
- `skills/`: **our own** skills. Each is a folder with a `SKILL.md`, ready to copy into a project's `.claude/skills/` (or the equivalent folder for other tools).

## Adding a tool

1. Pass the [vetting](vetting.md) checklist.
2. Write a page from [plugins/_template.md](plugins/_template.md).
3. Add it to the table above and to [stack-profiles](setup/stack-profiles.md).
4. Log it in [CHANGELOG](../CHANGELOG.md).
