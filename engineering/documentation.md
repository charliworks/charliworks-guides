# Documentation

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- Every repo has a README from [the template](../templates/README.template.md). Someone new should be able to run the project in 10 minutes or less.
- Keep `.env.example` complete ([environments-secrets](environments-secrets.md)).
- Record decisions as ADRs in `docs/adr/` ([template](../project-management/templates/adr.md)).
- Comment public functions and APIs with the language's doc format (JSDoc, dartdoc, …).
- Update docs **in the same PR** as the code change. That's part of the [Definition of Done](../00-start-here/definition-of-done.md).
- Write for users in the changelog and release notes, using the [brand voice](../design/brand-voice.md).
