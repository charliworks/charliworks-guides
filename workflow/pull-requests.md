# Pull requests

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- **Small PRs**: aim for under ~400 changed lines. Split bigger work into slices.
- The title follows [commit-messages](commit-messages.md), because it becomes the squash commit.
- Use the [PR template](../templates/github/pull_request_template.md): what, why, how to test, screenshots for UI.
- Link the issue: `Closes #N`.
- CI must be green before merging.
- Meet the [Definition of Done](../00-start-here/definition-of-done.md).
- Open a draft PR early if you want feedback on direction.

## Reviewing

- Review for correctness first, then clarity, then style. Linters handle most of the style.
- Prefix comments: `blocker:`, `suggestion:`, `nit:`, `question:`.
- **Solo self-review**: take a break, then read the full diff on GitHub as if someone else wrote it. Optionally run the [code-reviewer skill](../ai/skills/code-reviewer/SKILL.md), but its findings are input, not approval.

## Why

Small, well-described PRs are easier to review, easier to revert, and leave a history you can understand later.

## Related

- [git-branching](git-branching.md)
- [ai/plugins/github](../ai/plugins/github.md)
