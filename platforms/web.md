# Platform: web

> Last reviewed: 2026-11 · Status: 🚧 Draft (add stack-specific rules once the default stack is chosen)

## TL;DR (the rules)

- Pick a default stack via an ADR, then document it here so every web project starts the same way.
- TypeScript over JavaScript for anything beyond a one-off page.
- Server-render or statically generate public pages for SEO and speed.
- Meet the web [performance budget](../engineering/performance-budgets.md).
- Use semantic HTML first ([accessibility](../design/accessibility.md)).
- Images: modern formats, explicit width and height, lazy-load below the fold.
- Forms: server-side validation, clear errors, no lost input on failure.
- Configure security headers (CSP, HSTS) at the hosting level.

## AI stack profile

See [stack-profiles](../ai/setup/stack-profiles.md#web).

## Default stack

_To decide (ADR)._ Record framework, styling approach, database/auth, hosting, and testing tools here.
