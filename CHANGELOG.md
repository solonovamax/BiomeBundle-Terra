# Biome Bundle Changelog

## Repository + Scope changes via Hard Fork (2021-04-11)

This project was forked on 2021-04-11 with the intent of porting it over to the
Terra terrain generation engine. Because of this, a few things have changed in
the repository structure:

- Changing versioning to comply with SemVer (The previous version was 6.0, so
  future versions will start from 6.0.0)
- Added CHANGELOG.md containing all the changes.
- Renamed license file from "LICENCE" to "LICENSE"
- Forked base repo to move from the OTG engine to the Terra engine. As of this
  message, nothing has been ported over yet, but the process will begin shortly.
- Modified some of the git commit history to clean it up. This means the git
  history is different from the original repo.
- Added .gitignore

## v6.0

Note: This version is not compatible with worlds made with previous versions of
Biome Bundle. Biomes have been added/removed and so seeds no longer generate the
same layout. Starting a brand new world is recommended.

### Fixed

* Raised sea level to Y63 to improve mod compatibility and create more space
  underground (integrated all of SamGungraven's changes)
* Ore generation is now vanilla
* Fix volatility values between biomes to improve terrain smoothing
* Fix generation of huge oceans
* Re-enabled vanilla ocean monuments
* [#77](https://github.com/BiomeBundle/BiomeBundle/issues/77): Fix cut-off
  structures
* [#84](https://github.com/BiomeBundle/BiomeBundle/issues/83): Fix double
  entries
* [#84](https://github.com/BiomeBundle/BiomeBundle/issues/84): Re-enabled biomes
* Rebalanced rarity of all structures to increase variation and increase
  spawning chances for rarer structures lik the custom mansions.
* Fixed books not correctly enchanted in loot chests
* Fixed file name issues on linux
* Fixed incorrect data in flower pots generated in structures
* Reviewed mob spawners, some structures had them too closely together making it
  to easy to create mob farms

### Added

* Emeralds now have a small chance to appear in any biome
* Changed global 'fracture' settings to prevent overhanging terrain and create
  more realistic landscapes
* Added a few new biomes using new trees, rocks, etc.
* Added a few new flatter variants of existing biomes to create easier to
  traverse variations.
* Add a couple more structure variants existing structures
* Lots of small enhancements to existing biomes

### Removed

* Overhauled ice biome group

## v5.1

### Fixed

* Ravines and caves now properly remove all surface/ground blocks
* Added missing biome dictionary tags for SpookySwampland & Savanna Edge (Forge
  only)
* Fixed custom ocean temple rarity & improved temple placement
* Lots of other fixes and improvements for existing objects and structures

### Added

* Added default portal frame material: Dirt Block for returning from other OTG
  dimensions if they are installed (Forge only)
* Biome Bundle now initialises other OTG dimensions (Skylands, Flatlands, Void)
  automatically so they can be travelled to via their respective portals if also
  installed (Forge only)
* Added a new near bedrock custom cave layer across all biomes to make
  underground caving/mining more interesting and rewarding
* Entirely reworked Desert Cliffs biome
* Version 2.0 of the witches mansion structures
* Added 3 new mini ocean temples
* Added a new castle structure variant
* Added a new custom underground stronghold variant (sandstone)
* Added a few small structures for red sand/mesa areas
* Added iron golems to custom structures containing villagers
* Enabled mesa style mineshafts in more biomes
* Reworked grass cover and water/lava availability in many biomes
* Lots of other tweaks and polish to existing biomes

### Removed

* Stopped villages spawning in all 'floating' biomes

## v5.0

Biome Bundle changelog:

* BBundle is now a .jar file - just drop it in your mods folder!
* Added Biome Dictionary settings for all biomes, improving compatibility with
  biome specific resources from other mods
* Added mob inheritance settings for all biomes (modded mobs now inherit the
  spawn rules of vanilla biomes where appropriate to improve compatibility)
* There is a new 'clone' GUI button in the single player world creation menu
  that allows multiple worlds with BBundle.
* Added 'prismarine coral' to ocean/deep ocean biomes
* Added rare giant versions of existing structures: giant jungle dungeons, giant
  desert pyriamid dungeons and giant witches mansions
* Enhancements to almost every existing biome and added several new biomes
* Mineshafts re-enabled, 'single stronghold' bug fixed
* Enabled vanilla loot list compatibility for almost all loot containers
* Added entities to over 100 structures and reduced the number of spawners (no
  more witch spawners sorry for those who enjoyed that!)
* Fixed pig spawners and placeholder blocks in one of the 'CastleBranch'
  structures
* Reworked most of the structure generation and added many more structures
* Enabled all different kinds of vanilla villages (Taiga, Savanna, etc), and
  added a custom desert villages
* Guardians now spawn in deep ocean and prismarine coral biomes
* Added new ocean temple variants and fixed odd ocean temple placements
* All known crashes and mod incompatibilities fixed by switching to OTG

## v4.1

* Disabled Mineshafts :( as a temporary way to prevent the crash on returning
  from the Nether
* Tripled Coal and Iron Generation below sea level (previously mountainous areas
  generated ample iron and coal but biomes that mostly stayed around sea level
  were not generating enough)
* Fixed bug causing only one type of beach to appear
* Added edge biomes to another dozen or so biomes for smoother biome transitions
* Enabled strongholds in more biomes
* Reduced frequency of volcano objects
* Tweaked custom stronghold rarity and fixed a few small branch placement issues
* Fixed obsidian geodes placing oddly and being cut in half sometimes
* Fixed red sand small lakes placing oddly
* Fixed some incorrect river types
* Added another semi-random castle generator to the 'CastleBranch' structure
  group
* Added existing structures to more biomes
* More tweaks to structure placement
* Added more grass to a few biomes

## v4.0 (probably)

* Forge version now working (with much much improved mod compatibility than the
  1.7.10 version)
* Stair block rotation fixed across all structures
* Added 23 new edge/isle biomes to provide smoother biome transitions and more
  varied terrain
* Added more clay under larger lakes
* Added more Melons in jungles
* Added more coal to ore generation, a tiny bit more iron, fewer diamonds and
  emeralds
* Fixes for some biome colours not displaying properly when using forge client
* Added stricter checks to make some odd structure placement less likely
* Further rebalanced structure rarities
* Added more custom small lake and volcano variety
* Fixed surface 'gravel ores' always generating gold incorrectly
* Fixed wrong beach type for some biomes
* Added more diorite to some biomes
* Reduced number of jukeboxes in generated structures
* Reworked Ocean island biomes a little in preparation for a future overhaul
* Improvements to Mesa Verde, Swampland, Taiga, Archipelago, various Ocean
  Islands, TropicalRainforest, Desert Hills, Rocky Mountains, Snowy Mesa, Frozen
  Forest, Snowy Mountains, Ice Plains, Rainforest, Tropical Rainforest,
  ForestCliffs, Ocean Rocks, Taiga Highlands, a few of the Cliffs variants,
  Small Deserts and some others
* Almost all biomes have a Replacetobiomename set and identify as vanilla biome
  IDs, which should make a lot of things work more smoothly with other mods and
  means temperatures should display more accurately when running server side
  only
* New biome: Diorite Cliffs

## v3.0 (probably)

* Basic generation of 1.8+ new blocks and mobs
* Many changes to virtually every biome
* Added first custom 'stronghold style' dungeon generator (only one theme so
  far)
* 5 or so completely new biomes and a ton of new edge and 'variation' biomes
* Overhaul of 'snow' biome group
* Significant tweaks to ore generation
* 300+ things ticked off a 'fix' list
* 75-100 new structures and caves
* Rebalance of loot and spawners in all structures
* Fundamental change to how trees generate (no longer can they collide with each
  other / most structures)
* Temporary fix for ocean monuments
* Implemented workaround for spigot/TC structure rotation issues (not sure if
  this is 100% working)

## Beta v2.1

* Fixed 'Savanna hard clay
  issue': https://www.reddit.com/r/biomebundle/comments/4isj9d/new_savanna_is_bugged/
* Made witch villages not spawn in water
* Fixed missing NBT data on some spawners/dispensers/chests
* Reduced chance of 'watchtower' structures to prevent 'clustering'
* Reduced chance of structures in large biomes
* Increased chance of generating large biomes
* Added two brand new structures missing from initial release
* Added variants to witch village
* Fixed a couple of small issues with vanilla desert temple variants

## Beta v2.0

* Almost all biomes have undergone changes, ranging from just a few tweaks to
  complete overhauls
* Over 100 structures added. More biome decoration (trees, rocks, etc), variants
  of the vanilla temples, as well as a number of new biome specific dungeons and
  ruins http://imgur.com/a/bkWrb
* Many biomes have been reduced in size and rarities have been adjusted,
  ocean/land rarities have been tweaked. Some new biomes added
  e.g. http://imgur.com/a/qqx62
* 'Frozen' biome group made more common http://i.imgur.com/sBiyAQ0.png
* Caves biomes: There are a few underground biomes to seek
  out http://imgur.com/a/RHYK0 (Not fully implemented yet, more coming in an
  update soon)
* A new GUI for enabling Biome Bundle & Terrain Control in the new world screen
  in single player forge (bye bye to manually naming your world 'bbundle')
* Ravines are re-enabled and are more epic than vanilla, watch your step :)
* Custom mob spawn rules now work in single player forge
* World generation for the forge version is now 5x faster



