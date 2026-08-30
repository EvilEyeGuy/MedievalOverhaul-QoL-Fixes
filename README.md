# Medieval Overhaul: QoL & Fixes

A collection of small fixes and quality of life additions for
[Medieval Overhaul](https://steamcommunity.com/sharedfiles/filedetails/?id=3219596926).

Every patch checks first whether the problem is actually there. On an
installation that is already fixed, nothing happens. Changes no balance.

## Fixes

- **Great trees draw correctly.** The four great trees sat on inconsistent draw
  layers, so they clipped through each other and through pawns. They now share
  one layer and sort by row. A mod setting picks whether the canopy is drawn
  behind pawns and items, over them, or over everything.
- **Plant graphics stay in place.** A tree's draw offset was only applied to its
  main graphic. Its leafless, immature, polluted and snow variants ignored it and
  jumped out of position when the season changed.
- **Noble houses trade again.** Their faction defs pointed at trader kinds that
  do not exist, which produced errors on startup and silent caravans. Dead
  entries are removed, empty lists get a working default.
- **Cellar and ice cellar are findable.** Both labels contained a stray Cyrillic
  character, so typing `cellar` in the architect search found nothing.
- **Beds and comfort furniture recognise each other.** Vanilla beds only accepted
  vanilla end tables and dressers, MO beds only MO furniture, so the wrong
  combination gave no comfort bonus at all. Both sides now accept both. The tall
  end table, which was in no bed's list and could never do anything, is included.

## Quality of life

- **Copy and paste building settings.** The way RimWorld already does it for
  storage, now on processors and fuelled buildings: processes, allowed fuels and
  the fuel level carry over instead of being set again on every new building.
  Paste onto any number of selected buildings at once.
- **The water barrel puts out fires.** A colonist can tip it over. Flames in the
  surrounding tiles go out, anyone caught in it is soaked and will not burn until
  they dry, and the barrel is used up.

## Requirements

Harmony, [SYR] Processor Framework, Medieval Overhaul. Load after Medieval
Overhaul.

## Installing from here

Download the repository and drop the folder into `RimWorld/Mods`. The built
assembly is included, so nothing needs to be compiled.
