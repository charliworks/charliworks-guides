# Environments and secrets

> Last reviewed: 2026-11 · Applies to: all repos

## Environments

| Name | Purpose | Data |
|---|---|---|
| `local` | Your machine | Seed or fake data |
| `preview` / `staging` | PR previews, pre-release testing | Fake or anonymized data |
| `production` | Real users | Real data, so access is restricted |

## TL;DR (the rules)

- `.env` is **always** gitignored. Commit `.env.example` with every key and a placeholder or description:

  ```dotenv
  # Supabase project URL (Settings → API)
  SUPABASE_URL=
  # Server-only. Never expose to the client.
  SUPABASE_SERVICE_ROLE_KEY=
  ```

- Names follow [naming](naming.md): `SCREAMING_SNAKE_CASE`, prefixed by service.
- **Client-exposed variables** must use the framework's public prefix (e.g. `NEXT_PUBLIC_`, `VITE_`) and must never hold secrets.
- Production secrets live in the hosting platform's secret store or a password manager, never in chat, notes, or repos.
- Each environment has **its own keys**. Never reuse production keys locally.
- Rotate keys when someone loses access, and at least once a year.
- Record every key's location and owner in the [infrastructure inventory](infrastructure-inventory.md).
- Docker: pass secrets via `env_file` or secrets, never baked into images ([docker](docker.md)).
