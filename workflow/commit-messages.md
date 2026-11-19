# Commit messages

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/): `type(scope): summary`
- Summary: imperative mood ("add", not "added"), lowercase, no period, **≤ 72 characters**
- One logical change per commit
- Body (optional): explain **why**, wrapped at 72 characters
- Breaking change: add `!` after the type/scope **and** a `BREAKING CHANGE:` footer
- Reference issues in the footer: `Closes #12`

## Types

| Type | Use for |
|---|---|
| `feat` | A new user-facing feature |
| `fix` | A bug fix |
| `docs` | Documentation only |
| `style` | Formatting only, no logic change |
| `refactor` | Code change that neither fixes a bug nor adds a feature |
| `perf` | Performance improvement |
| `test` | Adding or fixing tests |
| `build` | Build system, dependencies |
| `ci` | CI configuration |
| `chore` | Maintenance that doesn't fit elsewhere |
| `revert` | Reverting an earlier commit |

**Scope** is optional and names the area: `auth`, `ui`, `api`, `db`, `deps`, or a feature name.

## Examples

✅ Good:

```text
feat(auth): add Google sign-in
fix(reminders): stop duplicate notifications on resume
docs: explain .env setup in README
refactor(api)!: rename /vehicles to /garage

BREAKING CHANGE: clients must call /garage instead of /vehicles.
Closes #42
```

❌ Bad:

```text
fixed stuff
WIP
Update index.tsx
feat: Added new login page and also fixed the navbar and updated deps.
```

## AI-assisted commits

Either add a trailer such as `Co-Authored-By: <tool> <email>` or leave it off. Just be consistent within a repo. The human author is still responsible for the change ([ai/usage-rules](../ai/usage-rules.md)).

## Enforcement

Use [commitlint](https://commitlint.js.org/) with `@commitlint/config-conventional` in JavaScript/TypeScript projects. The [commit-writer skill](../ai/skills/commit-writer/SKILL.md) drafts messages that follow this guide.

## Why

Readable history, automatic changelogs, and semver bumps that follow from commit types ([versioning-releases](versioning-releases.md)).

## Related

- [git-branching](git-branching.md)
- [pull-requests](pull-requests.md)
