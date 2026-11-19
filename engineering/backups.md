# Backups and recovery

> Last reviewed: 2026-11 · Applies to: anything with real data

## TL;DR (the rules)

- **3-2-1 rule**: 3 copies, on 2 types of storage, with 1 off-site.
- Production databases: automatic daily backups, kept for at least 7 days.
- Back up signing keys (Android upload key, iOS certificates) in two separate secure places. If you lose them, you can lose the ability to update the app.
- Back up source assets (design files, game art, audio) that aren't in git.
- **Test a restore** at least once a quarter. A backup you've never restored is only a hope.
- Write down the recovery steps in each project's README or `docs/`.
