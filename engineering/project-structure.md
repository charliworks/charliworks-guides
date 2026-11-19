# Project structure

> Last reviewed: 2026-11 · Applies to: all repos

## Every repo has

```text
.
├── README.md            # from templates/README.template.md
├── AGENTS.md            # from templates/AGENTS.template.md
├── CHANGELOG.md
├── LICENSE
├── .editorconfig
├── .gitignore
├── .env.example         # every variable, no real values
├── .github/
│   ├── workflows/       # CI
│   ├── ISSUE_TEMPLATE/
│   └── pull_request_template.md
├── docs/
│   ├── adr/             # 0001-stack-choice.md, …
│   └── plans/           # AI or human implementation plans
└── src/ (or framework default)
```

## Rules

- **Organize by feature**, not by file type, once the app grows past a few screens: `src/features/reminders/{components,api,hooks}`.
- Shared code goes in `src/shared/` (or `lib/`). Only move code there after a *second* use.
- Tests live next to the code they test (`thing.test.ts`), or in `tests/` if the framework expects it.
- Use framework conventions when they exist. Don't fight the framework.

## Platform layouts

See [web](../platforms/web.md), [mobile](../platforms/mobile.md), [games](../platforms/games.md).
