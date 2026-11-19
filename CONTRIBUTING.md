# Contributing to the guides

> Last reviewed: 2026-11

## Proposing a change

1. Branch: `docs/<short-topic>`.
2. Edit or add the guide. New guides start from [`guide-template.md`](00-start-here/guide-template.md).
3. Update the guide's `Last reviewed` line.
4. Add a line to [CHANGELOG.md](CHANGELOG.md) under `Unreleased`.
5. Open a PR that explains **why** the rule should change, not just what changed.

## Retiring a rule

Don't silently delete it. Move it to a `## Retired` section at the bottom of the guide with the date and reason, and log it in the changelog.

## Quarterly review

Every quarter (Jan / Apr / Jul / Oct), go through any guide whose `Last reviewed` date is more than 6 months old. Either confirm it (just bump the date) or update it.

## Writing style

- Put the rules first. Explanations go below them.
- Prefer short bullets and ✅/❌ examples over long paragraphs.
- One topic per file.
- Mark incomplete guides with `🚧 Draft` in the header.
