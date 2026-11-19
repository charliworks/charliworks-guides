# Testing

> Last reviewed: 2026-11 · Applies to: all repos

## TL;DR (the rules)

- **Test behavior, not implementation details.**
- Every bug fix comes with a test that would have caught the bug.
- Write unit tests for business logic: calculations, date math, validation. Example: the logic for when a service is due.
- Write integration tests for API routes and database queries.
- Write a few end-to-end tests for the critical flows only (sign up, the core action, payment).
- CI runs all tests on every PR. Red means no merge.
- Never use real production data or real secrets in tests.

## End-to-end and UI testing with AI

[Playwright](../ai/plugins/playwright.md) lets an AI assistant click through the app in a real browser. Use it to reproduce bugs and run smoke tests, then save what you learn as real Playwright test files so they run in CI.

## Coverage

There's no fixed coverage target. Aim for high coverage on core logic and don't chase 100% on UI glue code.
