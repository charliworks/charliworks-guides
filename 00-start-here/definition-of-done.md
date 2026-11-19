# Definition of Done

> Last reviewed: 2026-11 · Applies to: every PR

A change is **done** only when every applicable box is ticked. The [PR template](../templates/github/pull_request_template.md) links here.

## Always

- [ ] It does what the issue or spec asked, and you've checked it yourself
- [ ] Code follows [code style](../engineering/code-style/general.md) and lint passes
- [ ] Tests added or updated, and CI is green ([testing](../engineering/testing.md))
- [ ] No secrets, debug logs, or commented-out code left behind
- [ ] Commits follow [commit-messages](../workflow/commit-messages.md)
- [ ] Docs updated: README, `.env.example`, ADR if a decision was made
- [ ] Reviewed (self-review when solo: re-read the full diff the next day or after a break)
- [ ] AI-generated parts reviewed line by line ([ai usage rules](../ai/usage-rules.md))

## If it touches UI

- [ ] Works on mobile and desktop widths
- [ ] Keyboard and screen-reader basics pass ([accessibility](../design/accessibility.md))
- [ ] Empty, loading, and error states handled
- [ ] Design pass done (Impeccable audit or manual check against [styling](../design/styling.md))

## If it touches data

- [ ] Migrations are reversible or have a rollback plan
- [ ] Personal data handling still matches the privacy notice ([data-privacy](../market-ph/data-privacy.md))

## If it ships

- [ ] Version bumped and changelog updated ([versioning](../workflow/versioning-releases.md))
- [ ] Platform release checklist completed ([release-checklists](../workflow/release-checklists.md))
- [ ] Performance budget still met ([performance-budgets](../engineering/performance-budgets.md))
