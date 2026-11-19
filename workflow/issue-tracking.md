# Issue tracking

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- All work starts as a GitHub issue, even small things.
- Use the issue templates: [bug](../templates/github/ISSUE_TEMPLATE/bug_report.md), [feature](../templates/github/ISSUE_TEMPLATE/feature_request.md).
- Each issue has one type label and one priority label.
- Track work on a GitHub Projects board with the columns: **Backlog → Ready → In progress → In review → Done**.
- Group issues into milestones that match the [plan](../project-management/planning.md).

## Labels

| Group | Labels |
|---|---|
| Type | `type: bug`, `type: feature`, `type: chore`, `type: docs`, `type: design` |
| Priority | `P0` (broken now), `P1` (this milestone), `P2` (soon), `P3` (someday) |
| Status helpers | `blocked`, `needs-spec`, `good-first-issue` |
| Area (optional) | `area: ui`, `area: api`, `area: db`, … |

## Writing a good issue

- The title says what's wrong or what's wanted: "Reminder fires twice after app resume", not "bug".
- Include acceptance criteria as a checklist.
- Bugs need steps to reproduce, the expected result, the actual result, and environment details.

## Related

- [planning](../project-management/planning.md)
- [estimation](../project-management/estimation.md)
