# Prompting

> Last reviewed: 2026-11

## TL;DR (the rules)

- **Give context**: what the project is, which files matter, and which guide applies. "Follow `workflow/commit-messages.md`" beats restating the rules.
- **State the goal and the constraints**: what done looks like, and what *not* to touch.
- **Ask for a plan first** on anything multi-step, then approve it.
- **Show examples** of the output you want (a component, a test style).
- **One task per prompt** when possible. Chain them rather than writing one giant request.
- **Ask it to say what it's unsure of** or didn't test.
- **Save good prompts.** If you use a prompt twice, turn it into a skill in [skills/](skills/).

## Template

```text
Context: <project, relevant files, guide links>
Goal: <what done looks like>
Constraints: <don't touch X, use Y, follow Z guide>
Output: <plan first | code | review comments>
```
