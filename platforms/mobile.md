# Platform: mobile

> Last reviewed: 2026-11 · Status: 🚧 Draft (add framework-specific rules once chosen)

## TL;DR (the rules)

- **Android first** for the Philippine market, but test on iOS before any cross-platform release.
- Test on a real **mid-range Android device**, not just emulators.
- Design for spotty connections: offline-first data, sync with conflict handling, and clear offline states.
- Request permissions only when they're needed, with an explanation screen first.
- Push notifications: opt-in, useful, never spammy. Give users controls.
- Keep signing keys out of the repo and back them up ([backups](../engineering/backups.md)).
- Follow the [release checklists](../workflow/release-checklists.md) for Play and the App Store.
- Meet the mobile [performance budget](../engineering/performance-budgets.md).

## Default stack

_To decide (ADR)._ Record the framework, state management, local storage, backend, and push service here.
