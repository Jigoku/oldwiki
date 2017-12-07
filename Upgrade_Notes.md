This page contains instructions you should take into account when migrating to Red Eclipse's development version.

## Codename L

Version 2.0 (Codename L) is Red Eclipse ported to use the Tesseract rendering engine, and is the latest and greatest state of Red Eclipse.

### Incompatible user settings

-   Mouse sensitivity scale has changed. Use this formula to calculate the new value: \`new = old \* 100 / 3\`

### Porting maps

-   Sunlights are imported from an entity to a set of variables, the importer takes all the entities and averages out their value to pick a new singular sunlight. You may need to adjust \`sunlightyaw\` and \`sunlightpitch\` to re-align the sunlight properly. For a visual indicator try: \`/atmo 1; atmoblend 0.5\` (remember to turn this off again if you don't want atmosphere effects).
-   More to come...

