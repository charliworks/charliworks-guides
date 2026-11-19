# Infrastructure inventory

> Last reviewed: 2026-11 · Applies to: the whole studio

One table for every account, domain, service, and key, so nothing expires or bills you by surprise.

**Never put secret values here.** Only record where they're stored. Because this repo is public, keep the real inventory in a **private** place (a private repo or a password manager) and use this table as the template.

| Item | Type | Project | Provider | Owner / login | Where the secret lives | Renews / expires | Cost | Notes |
|---|---|---|---|---|---|---|---|---|
| example.com | Domain | studio | registrar | charliworks | password manager | 2027-01 | | auto-renew on |
| | Database | | | | | | | |
| | API key | | | | | | | |
| | App store account | | | | | | | |

## Review

At each quarterly review, check renewal dates and remove anything unused.
