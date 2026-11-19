# AI usage rules

> Last reviewed: 2026-11 · Applies to: all AI tools, all repos

## TL;DR (the rules)

- **You own what ships.** AI output gets the same review as human code, and every line is read before merging ([Definition of Done](../00-start-here/definition-of-done.md)).
- **Never share** secrets, `.env` contents, production data, client confidential material, or users' personal data in prompts.
- **Every repo has an `AGENTS.md`** pointing to these guides ([template](../templates/AGENTS.template.md)), so the AI starts with our rules.
- **Plan before generating.** For anything bigger than a small fix, have the AI write a plan first, review it, then let it build.
- **Ask before risky actions.** AI tools must not push to `main`, run destructive commands, change database schemas, or add dependencies without your approval. Configure the tool's permission settings to enforce this.
- **Verify facts.** AI can invent APIs, flags, and package names. Check against the docs (Context7 helps) and run the code.
- **Watch for slopsquatting.** Confirm a suggested package actually exists and is the real one before installing it.
- **Keep the context lean.** Install only the tools your [stack profile](setup/stack-profiles.md) lists, because every plugin uses context.
- **Attribution**: optional `Co-Authored-By` trailer on commits ([commit-messages](../workflow/commit-messages.md#ai-assisted-commits)).
- **Generated assets** (images, audio): record the tool and check its commercial-use terms ([licensing](../engineering/licensing.md)).

## Good uses

Boilerplate, tests, refactors with a clear target, explaining unfamiliar code, first drafts of docs, design critique, reproducing bugs.

## Needs extra care

Auth, payments, cryptography, data migrations, privacy-related code, and anything you couldn't explain yourself.
