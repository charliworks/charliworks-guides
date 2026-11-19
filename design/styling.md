# Styling

> Last reviewed: 2026-11 · Applies to: web, mobile UI

## TL;DR (the rules)

- **Design tokens first.** Colors, spacing, radii, shadows, and type sizes live as tokens (CSS custom properties or a theme file). Don't hard-code values in components.
- **Spacing scale**: multiples of 4 (`4, 8, 12, 16, 24, 32, 48, 64`).
- **Type scale**: a small set of sizes (about 6) with consistent line heights. Body text is at least 16px on the web.
- **Color**: semantic token names (`--color-surface`, `--color-text-muted`, `--color-danger`), not raw names (`--blue-500`) in components. Contrast must meet [accessibility](accessibility.md).
- **Dark mode**: plan for it in the tokens from day one, even if it ships later.
- **Layout**: mobile-first, using flex and grid. Avoid fixed pixel heights for text containers.
- **States**: every interactive element has hover, focus-visible, active, and disabled styles.
- **Motion**: subtle and fast (150–300 ms), and respect `prefers-reduced-motion`.
- **Avoid the generic "AI look"**: default gradients, purple-on-white, cards inside cards, every heading centered. Run a design pass ([Impeccable](../ai/plugins/impeccable.md) or [frontend-design](../ai/plugins/frontend-design.md)) before a UI is called done.

## Token naming

`--{category}-{role}-{variant}` → `--color-text-muted`, `--space-4`, `--radius-lg`.

## Related

- [brand](brand.md)
- [ui-ux-principles](ui-ux-principles.md)
