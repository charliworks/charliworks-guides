# Vetting AI plugins, skills, and MCP servers

> Last reviewed: 2026-11 · Applies to: anything installed into an AI tool

Thousands of plugins exist, and only a fraction are worth installing. Each one also uses context and may run code on your machine. **Install less, and install deliberately.**

## Checklist (all must pass)

- [ ] **Solves a real gap** you've hit at least twice, which no installed tool covers
- [ ] **No overlap** with an installed tool (e.g. two design skills in one project)
- [ ] **Source read**: you've skimmed the `SKILL.md`, commands, and especially any **hooks** or scripts, since hooks run commands automatically
- [ ] **Trustworthy**: known author or org, active maintenance (recent commits), real usage, issues get answered
- [ ] **License** allows our use ([licensing](../engineering/licensing.md))
- [ ] **Data**: you know what it sends where. MCP servers that call external APIs see your code and prompts.
- [ ] **Permissions**: it doesn't need more access than the job requires
- [ ] **Version pinned**, or the installed version recorded on its page

## After adopting

1. Write its page in [plugins/](plugins/) from the [template](plugins/_template.md).
2. Add it to [stack-profiles](setup/stack-profiles.md).
3. Review at the quarterly review: still used? Still maintained? If not, uninstall it and mark the page retired.
