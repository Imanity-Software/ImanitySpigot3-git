# Changelog

### Contributors:
- [LeeGod](https://github.com/LeeGodSRC)
- [Whizyyy](https://github.com/Whizyyy)

All notable changes 

to this project will be documented in this file.

# **[Pre Release]**

## [2021.09.3 BUILD 1] - 2021-September-24
**``(New Release)``**

**⚠️ Update required for [``Rancha 2021.09.1 BUILD 1``](https://github.com/Imanity-Software/ImanitySpigot3-git/blob/master/rancha/CHANGELOG.md#2021091-build-1---2021-september-24)**

### Functional
- Added Metrics [``HERE``](https://bstats.org/plugin/bukkit/ImanitySpigot3/12858)
- Improved lag spike logger
  - *Fixed a problem where old entries were still counted in new lag spike log*
  - *Added tick count display for each entries*

### API Changes
- Added API annotation to every imanitySpigot package API classes
- Added Chunk Analyse API
  - *Documentation will be added soon*

### Code Quality
- Don't compile mockito-core directly into jar

# **[Experimental]**

## [2021.09.2 BUILD 2] - 2021-September-20
- Changed max text length in profile name, behaviour name and modifier name to 16 characters - [LeeGod](https://github.com/LeeGodSRC)
- Fixed [``#31``](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/31) - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.2 BUILD 1] - 2021-September-18
**``(New Release)``**

### Knockback Changes
- Added Knockback Control Centre - [LeeGod](https://github.com/LeeGodSRC)
  - *This is a completely redesigned knockback editor system*
  - *This is the very first update with Knockback Control Centre implementation*
  - *Some feature is lacking:*
    - *Simple editor*
    - *Knockback per world options*
- Added damager specify for velocities behaviour - [LeeGod](https://github.com/LeeGodSRC)
- Removed priority for behaviour - [LeeGod](https://github.com/LeeGodSRC)
  - *Replaced by list order swapping*

https://user-images.githubusercontent.com/36093806/133881160-de77bbb1-2853-4d4d-818e-2fc2d5bab606.mp4

### Bug Fixes
- Fixed region modification location incorrect issue - [LeeGod](https://github.com/LeeGodSRC)

### Code Quality
- Added brand new source generator for Source code buyers - [LeeGod](https://github.com/LeeGodSRC)
- Removed WorldData debug code - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.1 BUILD 1] - 2021-September-2
**``(New Release)``**

### API Changes
- Added ``org.bukkit.entity.Mob`` interface. Refer to entities that has AI - [LeeGod](https://github.com/LeeGodSRC)
  - *This is the same interface that >=1.12 bukkit API has, You can use it safety on both ImanitySpigot and modern APIs.*
- Added ``com.destroystokyo.paper.entity.RangedEntity`` interface. Refer to entities that has Ranged attack ability (ex: Skeletion) - [LeeGod](https://github.com/LeeGodSRC)
  - *a replica of modern Paper's interface. some method aren't possible to be ported*
- Added ``com.destroystokyo.paper.entity.Pathfinder`` interface. Open the possibility to control Pathfinding without NMS - [LeeGod](https://github.com/LeeGodSRC)
  - *This is the same interface that >=1.13 Paper API has, You can use it safety on both ImanitySpigot and modern APIs.*
- Added ``org.imanity.imanityspigot.ai`` package of interfaces. Open the possibility to control Mob AI / Goals without NMS - [LeeGod](https://github.com/LeeGodSRC)
  - *a replica of modern Paper's interface (>=1.15). Due to Mojang changes a lot in terms of Goal types, some aren't possible to port*
  - ***Documentation available [HERE](https://docs.imanity.dev/books/imanityspigot-3/page/mob-ai)***
- MobAIHandler is now desperated. - [Whizyyy](https://github.com/Whizyyy)
- Bumped Maven dependency version to ``2021.09.1b1`` - [LeeGod](https://github.com/LeeGodSRC)

### Bug Fixes
- Fixed an error on startup - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Compatibility patch for Citizens - [LeeGod](https://github.com/LeeGodSRC)

### Docs Changes
- Added Documentation Page for Mob AI **[``HERE``](https://docs.imanity.dev/books/imanityspigot-3/page/mob-ai)** - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 8] - 2021-Augest-31
- Prevent Fire Spread load chunks - [LeeGod](https://github.com/LeeGodSRC)
- Force getChunkAt() main thread - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed in some cases plugins broke when getChunkAt and get error with async catcher*
- Only process BlockPhysicsEvent if a plugin has a listener - [LeeGod](https://github.com/LeeGodSRC)
- Fixed hard coded async catcher unloadQueue - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [`#26`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/26)*
- Fixed wrong index field were being used in PlayerInventory clear - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [`#25`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/25)*
- Fixed Tile Entity Unload Lag Spike - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Cancelling BlockPlaceEvent triggering physics - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 7] - 2021-Augest-27
- Fixed an critical error - [LeeGod](https://github.com/LeeGodSRC)
- Fixed an issue with loadChunk() and regenerateChunk() while async chunk is enabled - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 6] - 2021-Augest-27
- Added Hard coded Async Catcher to unloadQueue - [LeeGod](https://github.com/LeeGodSRC)
- Improved option **``durabilityMultiplier``** - [LeeGod](https://github.com/LeeGodSRC)
  - *round durabilityMultiplier multiplied result*
  - *update inventory if durabilityMultiplier has a different result, so it synced with clients*

## [2021.08.1 BUILD 5] - 2021-Augest-26
- Added world config option **``blockOperation``** - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 4] - 2021-Augest-25
- Fixed an issue while Old Enchanting is disabled - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes [#16](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/16)*
- Flooring BlockPosition in Explosion - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes [#17](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/17)*
- Changed option higherDurabilityMultiplier to durabilityMultiplier - [LeeGod](https://github.com/LeeGodSRC)
- Improved option durabilityMultiplier - [LeeGod](https://github.com/LeeGodSRC) [Whizyyy](https://github.com/Whizyyy)
  - *durabilityMultiplier instead of diving use multiply is more intuitive*
  - *Fixed comment*
- Added Notes for knockback related stuff - [LeeGod](https://github.com/LeeGodSRC)
  - *extraHorizontal*
  - *extraVertical*
  - *default profile system*

## [2021.08.1 BUILD 3] - 2021-Augest-23
- Fixed an issue cause EntityTracker broken - [LeeGod](https://github.com/LeeGodSRC)
  - *This issue may result in you can't see other players, which is fixed now*

## [2021.08.1 BUILD 2] - 2021-Augest-23
- Added check for ChunkRegionLoader, if it's not ChunkRegionLoader don't activate Async Chunk
- Added reference Taliban Pearl showcase video
- Fixed [`#12`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/12)
- Fixed [`#13`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/13)
- Fixed [`#14`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/14)

## [2021.08.1 BUILD 1] - 2021-Augest-22
**``(New Release)``**

- Fixed Citizens Compatibility - [LeeGod](https://github.com/LeeGodSRC)
- Improved Configuration Descriptions - [Whizyyy](https://github.com/Whizyyy)
- Improved Security - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.3 BUILD 7] - 2021-Augest-16
- Fixed Compile Error - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.3 BUILD 6] - 2021-Augest-16
- Added Configurable Merge Range based on Item Type - [LeeGod](https://github.com/LeeGodSRC)
- Optimized Network connection - [LeeGod](https://github.com/LeeGodSRC)
  - *Consolidate flush calls for entity tracker packets*
  - *Only Flush packets once in flushPacketQueue*
- Implemented Entity Lookup Improvement - [LeeGod](https://github.com/LeeGodSRC)
- Remove Netty Unpooled buffer option - [LeeGod](https://github.com/LeeGodSRC)
  - *Moved to patch internally in rancha*

## [2021.07.3 BUILD 5] - 2021-Augest-1
- Removed option ``nettyNotPreferDirectBuffer`` - [LeeGod](https://github.com/LeeGodSRC)
- added option ``nettyUseUnpoolBuffer`` - [LeeGod](https://github.com/LeeGodSRC)
  - *This is an option that patches netty to use unpooled heap buffer so it fixes some compatibility issue*

## [2021.07.3 BUILD 4] - 2021-July-30
- Fixed captureDrops order - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.3 BUILD 3] - 2021-July-30
- Added ability to disable drops in BlockBreakEvent - [LeeGod](https://github.com/LeeGodSRC)

## [2021.07.3 BUILD 2] - 2021-July-30
- Fixed Versioning - [LeeGod](https://github.com/LeeGodSRC)
  - *Plugins will now receive 1.8.8-R0.1-SNAPSHOT instead of custom versioning format*

## [2021.07.3 BUILD 1] - 2021-July-29
**``(New Release)``**

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
**``(New Release)``**

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
**``(New Release)``**

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
**``(New Release)``**

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
