# Accessibility

> Last reviewed: 2026-11 · Applies to: all products with a UI

Target: **WCAG 2.2 AA**.

## TL;DR (the checklist)

- [ ] Text contrast ≥ 4.5:1 (≥ 3:1 for large text and UI elements)
- [ ] Everything works with the keyboard alone, with a visible focus ring
- [ ] Semantic HTML: real `<button>`, `<a>`, `<label>`, headings in order
- [ ] Every image has meaningful `alt` text (or `alt=""` if decorative)
- [ ] Form fields have labels, and errors are announced, not shown only in red
- [ ] Color is never the only way information is conveyed
- [ ] Touch targets ≥ 44×44 px
- [ ] Respects `prefers-reduced-motion`, and text scales to 200% without breaking
- [ ] Mobile: screen reader labels set (TalkBack / VoiceOver tested on the main flow)

## Tools

Use browser devtools' accessibility panel, axe DevTools, and Lighthouse. An Impeccable audit also flags many issues ([impeccable](../ai/plugins/impeccable.md)), but automated tools catch only part of the problems. Do a keyboard-only pass by hand.
