# AGENTS.md: charliworks rules for AI assistants

This file is for AI coding tools (Claude Code, Cursor, Codex, Gemini CLI, and others). Project repos should point here from their own `AGENTS.md` / `CLAUDE.md`. Use [`templates/AGENTS.template.md`](templates/AGENTS.template.md) to set that up.

## Rules that always apply

1. **Commits** follow [Conventional Commits](workflow/commit-messages.md): `type(scope): summary`, imperative, ≤ 72 chars.
2. **Branches** follow [git-branching](workflow/git-branching.md): `feat/…`, `fix/…`, `chore/…`, `docs/…`. Never commit directly to `main`.
3. **PRs** stay small and use the [PR template](templates/github/pull_request_template.md). Every PR must meet the [Definition of Done](00-start-here/definition-of-done.md).
4. **Secrets**: never write real secrets into code, commits, logs, or prompts. Use `.env` files that are gitignored, and commit only `.env.example`. See [environments-secrets](engineering/environments-secrets.md).
5. **Naming** follows [naming.md](engineering/naming.md).
6. **Ask before** adding a dependency, changing a public API or database schema, or deleting files you didn't create.
7. **Decisions**: if you make an architectural choice, propose an ADR using [the ADR template](project-management/templates/adr.md).
8. **UI work**: follow [design/styling.md](design/styling.md) and [accessibility.md](design/accessibility.md). If Impeccable is installed, run its audit before calling UI work finished. See [ai/plugins/impeccable.md](ai/plugins/impeccable.md).
9. **Personal data**: anything that stores user data must follow [market-ph/data-privacy.md](market-ph/data-privacy.md).
10. **Be honest about uncertainty**: say what you didn't test or verify.

## Where to look

| Task | Read |
|---|---|
| Starting a new project | [project-kickoff](00-start-here/project-kickoff.md) |
| Writing code | [code-style](engineering/code-style/general.md), [project-structure](engineering/project-structure.md), [testing](engineering/testing.md) |
| Shipping | [versioning-releases](workflow/versioning-releases.md), [release-checklists](workflow/release-checklists.md) |
| UI/design | [design/](design/) and [platforms/](platforms/) |
| Which AI tools to use | [ai/README.md](ai/README.md) |
