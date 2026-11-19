# Platform: games

> Last reviewed: 2026-11 · Status: 🚧 Draft (add engine-specific rules once chosen)

## TL;DR (the rules)

- **Asset naming**: `kebab-case` with a type prefix ([naming](../engineering/naming.md)):
  - `spr-` sprites, `bg-` backgrounds, `ui-` UI art, `sfx-` sound effects, `mus-` music, `fx-` particles, `font-` fonts
  - Animation frames: `spr-tulip-bloom-01.png`, `spr-tulip-bloom-02.png`, …
- **Sprite atlases**: group by scene or feature, not one giant atlas. Use power-of-two sizes where the engine benefits.
- **Source files** (`.psd`, `.aseprite`, `.kra`) live in `art-src/`. Large binaries use Git LFS or an external backup ([backups](../engineering/backups.md)).
- **Save data**:
  - Always has a `version` field
  - Write migration code for every format change, and test that old saves load ([release-checklists](../workflow/release-checklists.md#games-in-addition-to-mobileweb))
  - Write atomically (temp file, then rename) so a crash can't corrupt the save
- **Game constants** (growth times, prices, drop rates) live in data files, not hard-coded, so you can tune them without code changes.
- **Playtesting**: log each session in `docs/playtests/YYYY-MM-DD.md`: who played, what confused them, what they enjoyed, and what to change.
- **Credits and licenses** for all art, audio, and fonts ([licensing](../engineering/licensing.md)).
- Meet the game [performance budget](../engineering/performance-budgets.md).

## Default engine

_To decide (ADR)._ Record the engine, version, target platforms, and export settings here.
