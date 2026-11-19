# Security

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- **Secrets**: follow [environments-secrets](environments-secrets.md). Never commit them.
- **Validate on the server.** Client-side validation is for UX only.
- **Auth**: use a proven provider or library. Don't write your own password hashing or session handling.
- **Least privilege** for database roles, API keys, and cloud IAM. If you use row-level security (e.g. Supabase RLS), it must be **on** for every table that holds user data.
- **Dependencies**: enable Dependabot (or Renovate) and secret scanning on every repo. Review dependency-update PRs weekly.
- **Dependencies are a decision**: check maintenance, downloads, and license before adding one ([licensing](licensing.md)).
- **HTTPS only.** Set secure cookie flags.
- **Don't log** personal data, tokens, or passwords.
- **AI tools**: vet plugins before installing them ([ai/vetting](../ai/vetting.md)), and never paste secrets or client data into prompts.

## If a secret leaks

1. **Rotate it immediately.** Deleting the commit isn't enough, because the secret stays in git history and forks.
2. Check access logs for misuse.
3. Purge it from history if the repo is public.
4. Write a [postmortem](../project-management/templates/postmortem.md).
5. If personal data was exposed, follow the breach steps in [data-privacy](../market-ph/data-privacy.md).
