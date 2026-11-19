# Naming

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

| Thing | Convention | Example |
|---|---|---|
| Repos | `kebab-case`, product name first | `odomo-app`, `bloomie-game`, `charliworks-guides` |
| Branches | `type/kebab-description` | `feat/42-google-signin` |
| Folders and files (general) | `kebab-case` | `vehicle-card.tsx`, `service-history/` |
| Files (framework convention wins) | follow the framework | `VehicleCard.tsx` if the project uses PascalCase components |
| Variables and functions | `camelCase` (or the language's convention) | `nextServiceDate` |
| Classes, types, components | `PascalCase` | `VehicleCard`, `ServiceRecord` |
| Constants | `SCREAMING_SNAKE_CASE` | `MAX_VEHICLES` |
| Env vars | `SCREAMING_SNAKE_CASE`, prefixed by service | `SUPABASE_URL`, `PAYMONGO_SECRET_KEY` |
| Database tables and columns | `snake_case`, plural tables | `service_records.next_due_at` |
| API routes | `kebab-case`, plural nouns | `/api/service-records` |
| CSS classes / tokens | `kebab-case` | `--color-surface-raised` |
| Assets | `kebab-case` with a type prefix | `icon-wrench.svg`, `spr-tulip-bloom.png` |
| Git tags | `vMAJOR.MINOR.PATCH` | `v1.2.0` |

## Product names

- Check for domain, app store, and trademark conflicts before committing to a name.
- The codename may differ from the public name. Record both in the project README.

## Related

- [commit-messages](../workflow/commit-messages.md)
- [games](../platforms/games.md) for asset naming
