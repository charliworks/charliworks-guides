# Planning

> Last reviewed: 2026-11 · Applies to: all projects

## TL;DR (the flow)

Idea → Spec → ADRs → Milestones → Issues → Slices:

1. **Idea**: lives in the [parking lot](idea-parking-lot.md) until picked.
2. **Spec**: written with [templates/spec.md](templates/spec.md). Keep it to 1–2 pages: the problem, users, scope in/out, and success metric.
3. **ADRs**: one per significant decision, using [templates/adr.md](templates/adr.md).
4. **Milestones**: 1–3 week chunks, each ending in something demo-able.
5. **Issues**: each one fits in a PR of a day or two ([issue-tracking](../workflow/issue-tracking.md)).
6. **Slices**: build end to end (UI → API → DB) thinly, then widen.

## Rules

- Nothing gets built without at least a short spec.
- Write the "out of scope" list. It protects the MVP.
- Re-plan at the end of each milestone with a quick [retro](templates/retro.md).
- When something goes wrong in production, write a [postmortem](templates/postmortem.md).

## AI-assisted planning

A planning workflow such as [Superpowers](../ai/plugins/superpowers.md) can turn a spec into an implementation plan. Save the plan in the repo (`docs/plans/`) and review it before any code is written.

## Related

- [estimation](estimation.md)
- [project-kickoff](../00-start-here/project-kickoff.md)
