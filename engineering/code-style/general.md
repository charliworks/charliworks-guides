# Code style: general

> Last reviewed: 2026-11 · Applies to: all languages

Language-specific guides go next to this file (`typescript.md`, `dart.md`, …) and only list what differs from here.

## TL;DR (the rules)

- **Formatters and linters decide style.** Don't argue about it, configure it. Every repo has a formatter and linter that run in CI.
- Use `.editorconfig` everywhere ([template](../../templates/editorconfig)): UTF-8, LF line endings, final newline, 2-space indent unless the language convention differs.
- **Name for meaning**: `daysUntilService`, not `d` or `temp2`. Booleans read as questions: `isOverdue`, `hasVehicle`.
- **Small functions** that do one thing. If a function needs a comment explaining *what* it does, split it or rename it.
- **Comments explain *why***, not what.
- **No magic numbers.** Use named constants.
- **Handle errors explicitly.** No empty `catch` blocks. Log with context.
- Prefer **early returns** over deep nesting.
- **Don't leave dead code** behind. Git remembers it.
- `TODO` comments must reference an issue: `// TODO(#42): handle offline mode`

## Language guides

| Language | Guide | Status |
|---|---|---|
| TypeScript / JavaScript | `typescript.md` | 🚧 To write |
| CSS | see [design/styling](../../design/styling.md) | ✅ |
| *add as needed* | | |

## Related

- [naming](../naming.md)
- [project-structure](../project-structure.md)
