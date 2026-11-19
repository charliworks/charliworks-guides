# Release checklists

> Last reviewed: 2026-11 · Applies to: web, mobile, games

Copy the relevant list into the release issue. Always do the general list first.

## General (every release)

- [ ] `main` is green; [Definition of Done](../00-start-here/definition-of-done.md) met for every included PR
- [ ] Version bumped and changelog written ([versioning-releases](versioning-releases.md))
- [ ] Database migrations tested on a copy of production data
- [ ] Production environment variables and secrets checked ([environments-secrets](../engineering/environments-secrets.md))
- [ ] A fresh backup exists ([backups](../engineering/backups.md))
- [ ] Rollback plan written down

## Web

- [ ] Production build runs locally with no console errors
- [ ] [Performance budget](../engineering/performance-budgets.md) met (Lighthouse or similar)
- [ ] Meta tags, Open Graph image, favicon, and `robots.txt` in place
- [ ] Error tracking and analytics verified
- [ ] Privacy notice up to date ([data-privacy](../market-ph/data-privacy.md))
- [ ] Smoke test on production after deploy

## Mobile: Google Play

- [ ] `versionCode` incremented and `versionName` matches semver
- [ ] Release build signed with the upload key; key backed up **outside** the repo
- [ ] Target API level meets current Play requirements
- [ ] Data safety form matches what the app actually collects
- [ ] Store listing: screenshots, short and full descriptions, privacy policy URL
- [ ] Rolled out to internal or closed testing first, then a staged rollout

## Mobile: App Store

- [ ] Build number incremented
- [ ] Privacy nutrition labels match actual data collection
- [ ] Screenshots for the required device sizes
- [ ] TestFlight build tested on a real device
- [ ] Review notes and demo account provided if login is required

## Games (in addition to mobile/web)

- [ ] Save data from the previous version loads correctly ([games](../platforms/games.md))
- [ ] Tested on a low-end target device
- [ ] Audio and asset licenses checked ([licensing](../engineering/licensing.md))

Store rules change often. Check the official Play Console and App Store Connect requirements every release, and update this list when they change.
