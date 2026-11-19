# Project kickoff checklist

> Last reviewed: 2026-11 · Applies to: every new project

Work through this before writing any code. Copy it into the project's first issue and tick items off.

## 1. Define it

- [ ] One-sentence pitch: *"X helps Y do Z."*
- [ ] Target users and the main problem, written down
- [ ] Short spec using [templates/spec.md](../project-management/templates/spec.md)
- [ ] MVP scope: what's **in** and explicitly **out**
- [ ] Success metric: how you'll know it works
- [ ] Checked the [idea parking lot](../project-management/idea-parking-lot.md) for related notes

## 2. Name it

- [ ] Product name and repo name follow [naming.md](../engineering/naming.md)
- [ ] Domain and handle availability checked, if public-facing

## 3. Decide the stack

- [ ] Platform guide read: [web](../platforms/web.md), [mobile](../platforms/mobile.md), or [games](../platforms/games.md)
- [ ] Stack chosen; first ADR written: `0001-stack-choice.md`
- [ ] AI stack profile picked from [stack-profiles](../ai/setup/stack-profiles.md)

## 4. Set up the repo

- [ ] Created from the starter template (see [templates/](../templates/))
- [ ] `README.md` from [README.template.md](../templates/README.template.md)
- [ ] `AGENTS.md` from [AGENTS.template.md](../templates/AGENTS.template.md)
- [ ] `.editorconfig`, `.gitignore`, `.env.example` added
- [ ] Branch protection on `main` (PRs required)
- [ ] Linter, formatter, and commitlint wired up
- [ ] CI runs lint and tests on every PR

## 5. Data and compliance

- [ ] Personal data inventory: what you collect and why ([data-privacy](../market-ph/data-privacy.md))
- [ ] Secrets stored per [environments-secrets](../engineering/environments-secrets.md)
- [ ] New accounts, domains, and keys added to the [infrastructure inventory](../engineering/infrastructure-inventory.md)
- [ ] License chosen ([licensing](../engineering/licensing.md))

## 6. Design context

- [ ] Brand applied or a project palette defined ([brand](../design/brand.md))
- [ ] If using Impeccable: run its project-context setup once and commit the context file ([impeccable](../ai/plugins/impeccable.md))
- [ ] [Performance budget](../engineering/performance-budgets.md) set

## 7. Plan

- [ ] Milestones and the first issues created ([planning](../project-management/planning.md))
- [ ] GitHub Project board set up ([issue-tracking](../workflow/issue-tracking.md))
