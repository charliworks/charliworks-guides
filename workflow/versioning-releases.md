# Versioning and releases

> Last reviewed: 2026-11 · Applies to: anything that ships

## TL;DR (the rules)

- Use [Semantic Versioning](https://semver.org/): `MAJOR.MINOR.PATCH`
  - `feat` → MINOR, `fix`/`perf` → PATCH, `!` / `BREAKING CHANGE` → MAJOR
  - Stay at `0.x` until the first public release
- Tag releases on `main`: `v1.4.0`
- Each repo keeps a `CHANGELOG.md` in [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format. Write the entries for users, not developers.
- Create a GitHub Release from the tag, with the changelog section as its notes.
- Mobile apps: the store version name matches the semver, and the build number only goes up.

## Release flow

1. Make sure `main` is green and the [release checklist](release-checklists.md) for the platform is done.
2. Bump the version and move `Unreleased` changelog entries under the new version.
3. Commit `chore(release): v1.4.0`, then tag `v1.4.0` and push the tag.
4. Publish the GitHub Release, then deploy or submit.

## Automation (optional)

Tools like release-please or semantic-release can bump versions and write changelogs from Conventional Commits. Adopting one means writing an ADR first.

## Related

- [commit-messages](commit-messages.md)
- [release-checklists](release-checklists.md)
