# Localization and local payments (Philippines)

> Last reviewed: 2026-11 · Status: 🚧 Draft

## Formatting

| Thing | Rule | Example |
|---|---|---|
| Currency | `₱` symbol, two decimals, comma thousands | `₱1,250.00` |
| Currency code (APIs and data) | `PHP` | `amount: 125000, currency: "PHP"` (store money as integer centavos) |
| Dates (display) | Month-day-year, written-out month to avoid ambiguity | `Nov 19, 2026` |
| Dates (storage) | ISO 8601, UTC | `2026-11-19T02:00:00Z` |
| Time zone | Display in `Asia/Manila` unless the user sets another | |
| Phone numbers | Store in E.164 format, display local format | `+639171234567` → `0917 123 4567` |
| Locale tag | `en-PH`, `fil-PH` | |

## Language

- Default to English UI copy.
- If supporting Filipino, translate it properly (natural phrasing, not word-for-word) and keep strings in i18n files from day one.
- Taglish can work in marketing and casual copy, but keep it consistent and decide per product in the README.

## Payments

- Common local methods include e-wallets (e.g. GCash, Maya), cards, and bank transfers. Choose based on your actual users.
- Use a payment gateway that supports local methods rather than integrating each one yourself. Compare fees, settlement time, and docs, and record the choice in an ADR.
- Never store card details yourself. Let the gateway handle them.
- Handle webhooks idempotently (the same event may arrive twice).
- Payment providers receive personal data, so list them in the privacy notice ([data-privacy](data-privacy.md)).
