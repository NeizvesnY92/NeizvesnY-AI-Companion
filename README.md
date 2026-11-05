# NeizvesnY AI Companion

Offline Mindustry iOS companion experiment (HJSON + built-in logic; no Java or server).

## Mk.I experimental custom combat drone

- Unit definition: `content/units/neizvesny-companion.hjson`
- Logic: `logic/companion-custom-unit.mlog`
- Fast flying unit with a basic weapon, intended for follow/escort behavior.
- **Not yet verified in-game.** The custom sprite is not yet included, so the unit may appear with a missing-texture placeholder. Content loading and processor binding need testing.

## Testing on iPhone

1. In Mindustry, remove and re-import this GitHub mod (or update it), then restart the game.
2. Open a sandbox map. Check whether the unit `neizvesny-companion` appears in the unit list and can be spawned.
3. Place a micro processor and paste the code from `logic/companion-custom-unit.mlog`.
4. Check whether the drone moves and follows. If the unit or script does not load, report the exact error.

The `.mlog` files are references: importing the mod does **not** automatically install the script in processors.

## Known limits

Mindustry Logic's `uradar` has a limited search radius; a faster custom unit may reduce lag but does not provide unlimited player tracking. This is a logic-controlled allied unit, not a second multiplayer player or conversational AI.

Older Flare prototype: `logic/companion-follow.mlog`.

## Experimental Companion Factory

The block definition `content/blocks/companion-factory.hjson` adds a 3x3 UnitFactory named **Companion Factory** under the Units category. It is intended to cost no resources and produce `neizvesny-companion` in 60 ticks (about one second at 60 TPS). This configuration has not yet been verified in-game. Re-import/update the mod and restart Mindustry before testing. The factory and unit currently have no custom PNG sprites, so missing-texture placeholders may appear.
