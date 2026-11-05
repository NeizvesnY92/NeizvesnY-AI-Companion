# NeizvesnY AI Companion

Standalone offline companion prototype for Mindustry on iPhone.

## Current status
Experimental v0.1, **not yet tested in game**. Mindustry iOS does not support ordinary Java mods. This project uses built-in Mindustry Logic to command an allied unit; it is not a second multiplayer player or a conversational AI.

## Try the prototype
1. Import this repository as a mod if your Mindustry iOS version permits HJSON mod imports.
2. In a sandbox world, place a **micro processor** and create an allied **flare** unit.
3. Open `logic/companion-follow.mlog` in this repository and enter its instructions into the processor's logic editor. The .mlog file is reference logic, **not automatically installed into a processor** by the mod.
4. Stay near the flare and observe its behavior. The experimental script tries to approach the allied player and fire at enemies.

## Next steps
- Verify syntax and behavior against the installed Mindustry version.
- Add a convenient in-game processor schematic with embedded code.
- Add selectable modes (follow, defend, repair).
- Explore mining and building constraints of logic-controlled units.

No cloud server or internet is required during gameplay.
