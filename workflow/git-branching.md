# Git branching

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- **`main` is always deployable.** It's protected: no direct pushes, changes only arrive through PRs.
- Use short-lived branches off `main`, merged back within days, not weeks.
- Branch name format: `type/short-kebab-description`, optionally with the issue number: `feat/42-google-signin`
- **Squash merge** by default. The PR title becomes the commit message, so it must follow [commit-messages](commit-messages.md).
- Delete branches after merging.
- Rebase on `main` before merging if the branch has fallen behind.

## Branch types

Use the same types as commits: `feat/`, `fix/`, `docs/`, `refactor/`, `chore/`, `test/`, `ci/`, `perf/`.

Two extras:

- `hotfix/` for urgent production fixes. Merge as soon as possible and tag a patch release.
- `release/x.y.z` only if a project ever needs a stabilization period. Most won't.

## Examples

✅ `feat/odometer-reminders` · `fix/31-login-crash` · `docs/env-setup`

❌ `charli-branch` · `new` · `test2` · `feature/Add_Login_Page`

## Why

Trunk-based flow fits a small studio: less merge pain and fewer forgotten branches, and `main` always reflects reality.

## Related

- [pull-requests](pull-requests.md)
- [versioning-releases](versioning-releases.md)
