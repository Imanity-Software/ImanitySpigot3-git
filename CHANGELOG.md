# Changelog

### Contributors:
- [LeeGod](https://github.com/LeeGodSRC)
- [Whizyyy](https://github.com/Whizyyy)

All notable changes to this project will be documented in this file.

## [Unreleased]

## [2021.07.3 BUILD 2] - 2021-July-30
- Fixed Versioning
  - *Plugins will now receive 1.8.8-R0.1-SNAPSHOT instead of custom versioning format*

## [2021.07.3 BUILD 1] - 2021-July-29
### Documentation
- Added Documentation Page https://docs.imanity.dev/books/imanityspigot-3/page/commands - [LeeGod](https://github.com/LeeGodSRC)
- Added Documentation Page https://docs.imanity.dev/books/imanityspigot-3/page/optimization-tips - [LeeGod](https://github.com/LeeGodSRC)

### Functional
- Supported Oversized Chunk read & write - [LeeGod](https://github.com/LeeGodSRC)
- Added Old Enchanting option - [LeeGod](https://github.com/LeeGodSRC)
- Added /imanitySpigot docs - [LeeGod](https://github.com/LeeGodSRC)

### Performance
- Reduce Chunk Lookup in Entity Ticking - [LeeGod](https://github.com/LeeGodSRC)

### Bug Fixes
- Fixed FastAsyncWorldEdit support - [LeeGod](https://github.com/LeeGodSRC)
- Fixed View Distance player disappear issue - [LeeGod](https://github.com/LeeGodSRC)
- Fixed /curkb Error - [LeeGod](https://github.com/LeeGodSRC)

### API
- Added PlayerPickupArrowEvent - [LeeGod](https://github.com/LeeGodSRC)
- Added EntityPickupItemEvent - [LeeGod](https://github.com/LeeGodSRC)
- Added Player.imanity().setKnockback() - [LeeGod](https://github.com/LeeGodSRC)
- Added Player.imanity().isCanPickupExperience() - [LeeGod](https://github.com/LeeGodSRC)
- Added Player.imanity().setCanPickupExperience() - [LeeGod](https://github.com/LeeGodSRC)
- Added Chunk.getBlock(Location) - [LeeGod](https://github.com/LeeGodSRC)

### Code Quality
- Improved Physics error silence - [LeeGod](https://github.com/LeeGodSRC)
- Use Cache instead of MapMaker in Offline Players Cache - [LeeGod](https://github.com/LeeGodSRC)
- Remove extra useless postToMainThread call - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.2 BUILD 3] - 2021-July-20
- Added World.setSpawnLocation(Location) - [LeeGod](https://github.com/LeeGodSRC)
- Added ability to upload information data on [`code.imanity.dev`](https://code.imanity.dev) with flag - [LeeGod](https://github.com/LeeGodSRC)
  * `/imanitySpigot chunkAnalyzer export -u` is the command, `-u` flag stands for upload - [LeeGod](https://github.com/LeeGodSRC)
- Added ability to reload premium.yml while `/imanitySpigot reload` - [LeeGod](https://github.com/LeeGodSRC)
- Starting Code base for Plugin Manager - [Whizyyy](https://github.com/Whizyyy)
- Fixed Knockback Reload - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.2 BUILD 2] - 2021-July-20
- Added `!stacktrace` Command in Rancha (This command will print out all thread's stacktrace, useful when having server timed out issues.)
- Added Command Documentation for Knockback [`Docs`](https://docs.imanity.dev/books/imanityspigot-3/page/knockback) - [LeeGod](https://github.com/LeeGodSRC)
- **Premium Feature** Added Lag Spike Alert Message for customization while lag spike alert - [LeeGod](https://github.com/LeeGodSRC)
- **Premium Feature** Added Ping Self Message for customization when pinging ourself - [LeeGod](https://github.com/LeeGodSRC)
- Reload Knockback Profiles while `/imanitySpigot reload` - [LeeGod](https://github.com/LeeGodSRC)
- Fixed ChunkAnalyzer Description in /imanitySpigot - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Plugin Command again - [Whizyyy](https://github.com/Whizyyy)

## [2021.07.2 BUILD 1] - 2021-July-16
- Auto Saving and Chunk Unloading Optimziation - [LeeGod](https://github.com/LeeGodSRC)
  - *Re-added Auto Save cap (configurable in world config "maxAutoSaveChunksPerTick")*
  - *Build level NBT Data in IO Thread if chunk has been unloaded*
  - *Dont queue jobs if queue is over an amount (configurable in world config "maxQueuedSizeAutoSave")*
  - *Reattempt chunk save if failure (prevent unnecessary bugged chunk load)*
- Added Command to Toggle Lag Spike Detector - [LeeGod](https://github.com/LeeGodSRC)
- Let /tp execute player teleport after chunk loaded - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.1 BUILD 4] - 2021-July-16
- Fixed Plugin Command Patch - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.1 BUILD 3] - 2021-July-14
- Disallow Negative value in Hit Delay, Horizontal Friction and Vertical Friction - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Speed Value Modifier ClassCastException - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.1 BUILD 2] - 2021-July-13
- Added "switchToSimple" tab completion to Advanced Command Editor - [LeeGod](https://github.com/LeeGodSRC)
- Allow deletion for Advanced Format Profile in Simple Command Editor - [LeeGod](https://github.com/LeeGodSRC)
- Storing World directly in the Knockback Profile instead of in world config - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Command Type Choice being useless - [LeeGod](https://github.com/LeeGodSRC)
- Fixed /plugins color code - [Whizyyy](https://github.com/Whizyyy)

## [2021.07.1 BUILD 1] - 2021-July-12
- Added documentation page for Knockback System https://docs.imanity.dev/books/imanityspigot-3/page/knockback
- Added Command "/curkb <player>" to view player's current knockback
- Added Command "/kb togglePerWorld" to enable Knockback Per World in game
- Added Command "/kb <profile> addWorld <world name>" to set available profile in worlds for Knockback Per World Feature
- Added Command "/kb <profile> removeWorld <world name>" to remove available profile in worlds for Knockback Per World Feature
- Added Ability to modify knockback per world options in Command Editor
- Added Command and editor button to enable and disable hit delay in Simple Command Editor
- Added limitation of knockback profile names (attempts to create knockback with name "vanilla", "reload", "listprofiles", "listdefaults", "listbehaviours", "listmodifiers", "toggleperworld", "switchtoadvanced", and "switchtosimple" is not allowed)
- Mentioning documentation page in Knockback Command Editor (modifierPath explaination, Help Page etc)
- Changed Command to switch command mode from "/kb simple" and "/kb advanced" to "/kb switchToSimple" and "/kb switchToAdvanced"

## [2021.06.2 BUILD 3] - 2021-July-2
- Improved lag spike detection message
- Fixed Chunk status not being recognized correctly
- Fixed build configuration
- Fixed plugin command
- Fixed UnsupportedOperationException on set default knockback profiles

## [2021.06.2 BUILD 2] - 2021-June-27
- Fixed Compile Error

## [2021.06.2 BUILD 1] - 2021-June-26

### API Changes
- Added getKnockback method to KnockbackService.
- Added PlayerSelectKnockbackEvent.
- Renamed getDefaultKnockback() to getRandomKnockback(World).

### Docs Changes
- Javadocs for Knockback class
- Javadocs for KnockbackBehaviour class.
- Javadocs for KnockbackService class.

### Knockback System
- Added knockbackPerWorld option in config.yml and knockback option in world configuration.
- Added hit delay to Simple command editor.
- Knockback Behaviours can now be enabled or disabled.
- Hit delay is now overwriting based, Now if a hit delay behaviour is enabled, bukkit hit delay will be overrided.
- Renamed simple behaviour to velocities behaviour.
- Renamed default knockback to vanilla knockback.
- Improved Description for Knockback Modifier.
- Profile registered with name "vanilla" or "reload" will not be allowed.
- If a knockback profile were unregistered, Player's using the porilfe will automatically pick a knockback from default lists.
- Displaying Behaviour Identity in knockback profile editor.
- Removed velocityPacket behaviour (We believe there is no reason for this to be customizable, so we decide to made it enabled by default without customization ability.)
- Removed no valid knockback warning (Planning to make a command for checking player's current knockback.)

### Code Quality
- knockback instance for players are now not allowed to be null

## [2021.06.1 BUILD 6] - 2021-June-24
- Added notes for instantRespawn option (for Via-Version compatibility) - closed #3
- Improved BlokState Array map, fixed
- Fixed FAWE compatibility on PlayerChunkMap NMS issue
- Fixed getChunk callback not being called correctly when chunk is already loaded & Async Chunk is disabled - closed #4

## [2021.06.1 BUILD 5] - 2021-June-23
- Added Instant Respawn Option
- Fixed ProtocolLib Patching
- Fixed FastAsyncWorldEdit Compatibility
- Fixed ImanityCommand weird behaviour when entering unknown sub command
- Don't patch ProtocolLib if it's ProtocolLib 4.6.1-SNAPSHOT or above
- Updated JavaAssist to 3.28.0-GA
