# Changelog

### Contributors:
- [LeeGod](https://github.com/LeeGodSRC)
- [Whizyyy](https://github.com/Whizyyy)

All notable changes to this project will be documented in this file.

## [2024.1.1 BUILD 1] - 2024-Januray-1
**``(New Release)``**

### Added:
- Added `disableFallingBlocksPhysics` world option. - [LeeGod](https://github.com/LeeGodSRC)
  - Thanks to @Xefreh for the patch.
 
### Fixed:
- Fixed NullPointerException from shutting down ghost patcher. - [LeeGod](https://github.com/LeeGodSRC)

### Changed
- Updated outdated links and time. - [LeeGod](https://github.com/LeeGodSRC)

## [2023.10.1 LTS BUILD 2] - 2023-October-28

### Fixed
- Fixed NPE in lighting - [LeeGod](https://github.com/LeeGodSRC)

## [2023.10.1 LTS BUILD 1] - 2023-October-26

### Added
- Added TNTPrimeEvent - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#210](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/210)*
- Addd non-mutative getCrossProduct method to bukkit Vector - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#227](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/227)*

### Changed
- Reload world configurations when `/imanity reload` - [LeeGod](https://github.com/LeeGodSRC)
- Make sure lighting update not sharing the same cache - [LeeGod](https://github.com/LeeGodSRC)
- Use weak reference for light cache - [LeeGod](https://github.com/LeeGodSRC)
- Improved ignore damage ticks functionality - [LeeGod](https://github.com/LeeGodSRC)

## [2023.7.1 BUILD 1] - 2023-July-27

### Added
- Added `arrowIgnoreDamageTicks` option - [LeeGod](https://github.com/LeeGodSRC)

### Changed
- Added fillWorld description (inform /imanity fillWorld radius is in blocks) - [LeeGod](https://github.com/LeeGodSRC)

### Fixed
- Only apply yaw and pitch since only rotation can desync for `ghostBucketFix` option - [LeeGod](https://github.com/LeeGodSRC)
- Fixed toggleantixray command on console - [LeeGod](https://github.com/LeeGodSRC)

## [2023.5.1 LTS BUILD 3] - 2023-June-22

### Changed
- Don't update blocks that's too faraway for antixray (reduce loads) - [LeeGod](https://github.com/LeeGodSRC)
- Stricter solid block checks for antixray - [LeeGod](https://github.com/LeeGodSRC)

## [2023.5.1 LTS BUILD 2] - 2023-May-31

### Changed
- Improved network manager initialization and packet sending - [LeeGod](https://github.com/LeeGodSRC)
  - *Removed network manager packet queue synchronization*
  - *Ensure queued packet only being sent once*
  - *Add network manager to pending list and add them all at once on main thread tick*
  - *Don't try to flush packet out of main thread unless it's in pending state*
  - *Solved [#198](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/198)*
  - *Solved [#204](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/204)*
  - *Solved [#207](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/207)*

## [2023.5.1 LTS BUILD 1] - 2023-May-24
![20230501](https://github.com/Imanity-Software/ImanitySpigot3-git/assets/36093806/498f2a96-36ca-4666-b693-fdfb4c45c673)

### Added
- Added Raytrace AntiXray Addition - [LeeGod](https://github.com/LeeGodSRC)
  - *An advanced anti xray system that only display ores to people who can see it from raytracing.*
  - *Built on top of Async AntiXray*
  - *Exclusive to ImanitySpigot3 Enterprise.*
  - Sub feature: Fake Ores
    - *Generating random ores surrounding the world.*
    - *To mislead xrayers from mining the real ores.*
- Added Async AntiXray - [LeeGod](https://github.com/LeeGodSRC)
  - *Alternative to current spigot anti xray, obfuscation is running completely in different thread pool.*
  - *Also fixed the issue where ores are tend to not be obfuscated.*
- Added `/imanity disableAntiXray` - [LeeGod](https://github.com/LeeGodSRC)
  - *Only works when Async AntiXray was enabled*
- Added `/imanity bypassAntiXray` - [LeeGod](https://github.com/LeeGodSRC)
  - *Only works when Async AntiXray was enabled*
- Added `improvedHitDetection` option - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#199](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/199)*
- Added `ghostBucketFix` option - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed ghost water/lava bucket placement by improving right click detection.*
- Added `bucketUpdateRange` option - [LeeGod](https://github.com/LeeGodSRC)

### Fixed
- Fixed memory leak for AsyncFastLight - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#140](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/140)*

## [2023.4.1 BUILD 2] - 2023-April-25
- Fixed lighting issue with loading chunks - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#133](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/133)*

## [2023.4.1 BUILD 1] - 2023-April-23
- Added throughCobweb option to every egg, snowball, and pearl - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#193](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/193)*
- Added velocity exploit patch - [LeeGod](https://github.com/LeeGodSRC)

## [2023.3.1 BUILD 3] - 2023-April-12
- Disallow natural creature spawning system from loading chunks - [LeeGod](https://github.com/LeeGodSRC)
- Fixed incorrect casting in part of chunk generation - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#195](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/195)*

## [2023.3.1 BUILD 2] - 2023-March-29
- Added `compatibilityMode` option - [LeeGod](https://github.com/LeeGodSRC)
  - *It's an option that attempts to fix edge cases for different scenarios or plugins. More changes will be added to this option, currently focsuing on chunk related stuff.*
- Added TileEntityChest thread safe fallback - [LeeGod](https://github.com/LeeGodSRC)
  - *An attempt of fixing [#137](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/137)*

## [2023.3.1 BUILD 1] - 2023-March-17
- Added **Redstone Limiter** addition - [LeeGod](https://github.com/LeeGodSRC)
  - *An addition that allows you to control the maximum amount of redstone, hopper, dispenser, dropper, piston push per tick by configuration. currently available for Enterprise only.*
- Added [mob stacker related APIs](https://docs.imanity.dev/imanityspigot/api/extended-api-methods#entity) to Entity class - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#186](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/186)*

## [2023.2.1 LTS BUILD 6] - 2023-March-6
- Added world region modification `sealevel` - [LeeGod](https://github.com/LeeGodSRC)
  - *This option allows you to modify the sea/water level of a special region*
  - *Argument: `sealevel: <number>`*

## [2023.2.1 LTS BUILD 5] - 2023-March-2
- Fixed restart script not working - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 LTS BUILD 4] - 2023-February-28
- Fixed remove lakes region using wrong condition checking - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 LTS BUILD 3] - 2023-February-28
- `removeLakes` world region option will now remove lakes generated by heightmap (lower than sea level) - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#180](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/180)*
- usercache.json now won't crash the server for failed loading - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 LTS BUILD 2] - 2023-February-18
- Fixed small error on explosion calculation - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 LTS BUILD 1] - 2023-February-17
**``(New Release)``**

## Added
- Added **Enterprise Plan** - [LeeGod](https://github.com/LeeGodSRC)
  - *Checkout Enterprise now on [HERE](https://go.imanity.dev/enterprise)*
- Added **AsyncExplosion** addition - [LeeGod](https://github.com/LeeGodSRC) & [Whizyyy](https://github.com/Whizyyy)
  - *A mutli-threaded explosion system with enhanced algorithm to optimize Explosion by 3-8x.*
- Added **GhostPatcher** addition - [LeeGod](https://github.com/LeeGodSRC)
  - *A patcher system that will remove ghost blocks when fast instant mining.*
- Added option `explosion.shouldCheckBlockDensity` into imanity world config - [LeeGod](https://github.com/LeeGodSRC)
- Added option `explosion.constantExplosionRange` into imanity world config - [LeeGod](https://github.com/LeeGodSRC)

## Chores
- Improved explosion algorithm - [Whizyyy](https://github.com/Whizyyy)
- Improved comments in confiugrations - [Whizyyy](https://github.com/Whizyyy)

## [2023.1.1 BUILD 2] - 2023-February-6
- Emerald ore generation will now be overriden by Custom block rule set if enabled - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#176](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/176)*
- Attempting to fix BKCommonLib reflection compatibility on nms World class - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#174](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/174)*
- Ignore Citizens patching if the Citizens is on new versions - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#172](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/172)*

## [2023.1.1 BUILD 1] - 2023-Januray-1

### Chores
- Improved block position memory allocation - [Whizyyy](https://github.com/Whizyyy)
- Improved player chunk map memory allocation - [Whizyyy](https://github.com/Whizyyy)

### Fixes
- Fixed EquipmentSetEvent not called when item is the same - [LeeGod](https://github.com/LeeGodSRC)
  - *Special Thanks to [Xefreh](https://github.com/Xefreh) for helping on the issue!*

## [2022.11.1 LTS BUILD 3] - 2022-December-8
- Should not reset damage ticks on entity death with mob stacker stacked - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#164](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/164)*
- Fixed not checking for overriden ChunkRegionLoader - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#160](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/160)*

## [2022.11.1 LTS BUILD 2] - 2022-November-7
- Fixed MobStacker ignoring entity equipments - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#161](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/161)*

## [2022.11.1 LTS BUILD 1] - 2022-November-3
**``(New Release)``**

### Added
- Implemented MobStacker - [Whizyyy](https://github.com/Whizyyy)

```yaml
# This section allow you to configure the MobStacker settings
# MobStacker is a feature that allow you to stack mobs together
# So that you can have less entities in the world and then better performance
# This is very useful for servers such as SkyBlock or Faction that run huge mob farms
mobStacker:
  enabled: true
  onlyStackFromSpawner: false
  stackRadius: 5.0
  maxStackAmount: 50
  ticksToStack: 100
  ignoreEntityType:
  - HORSE
  - VILLAGER
  - WOLF
```
![image](https://user-images.githubusercontent.com/36093806/199691142-35591000-3a54-4838-b950-8c844e64ec68.png)


### Bug Fixes
- Fixed setFlying() wrong variable used - [LeeGod](https://github.com/LeeGodSRC)

## [2022.8.1 BUILD 2] - 2022-August-30
- Added world option `enderPearlTrajectoryRandomness` - [LeeGod](https://github.com/LeeGodSRC)
- Added world option `potionTrajectoryRandomness` - [LeeGod](https://github.com/LeeGodSRC)
- Added world option `snowBallTrajectoryRandomness` - [LeeGod](https://github.com/LeeGodSRC)
- Added world option `eggTrajectoryRandomness` - [LeeGod](https://github.com/LeeGodSRC)
- Prevent server crashing from invalid movement packet - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#153](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/153)*
- Fixed instant respawn not working properly with setHealth(0) - [Whizyyy](https://github.com/Whizyyy)
  - *Solved [#144](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/144)*
- Fixed some errors on parallel entity tracking - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#148](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/148)*

## [2022.8.1 BUILD 1] - 2022-August-24
**``(New Release)``**

### Added
- Added option `fishingHookTrajectoryRandomness` - [LeeGod](https://github.com/LeeGodSRC)
- Added isEssentialRedstoneWaterProof option - [Whizyyy](https://github.com/Whizyyy)

### Changed
- Updated ImanityKnockback - [LeeGod](https://github.com/LeeGodSRC)
- Allow scanPlayers(list) to be used when parallel - [LeeGod](https://github.com/LeeGodSRC)
  - *Solved [#149](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/149)*

### Fixed
- Fixed PandaWire's redstone logic, some advanced tnt cannons are now working - [Whizyyy](https://github.com/Whizyyy)
- Fixed merge cannon optimization + improved explosions - [Whizyyy](https://github.com/Whizyyy)

## [2022.5.3 BUILD 4] - 2022-July-21
- Added LagSpikeTriggerEvent - [Whizyyy](https://github.com/Whizyyy)
  - *Solved [#122](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/122)*
- Added auto download spark profiler - [LeeGod](https://github.com/LeeGodSRC)
- Improved chunk cache and ensure main in getOrCreateChunk - [LeeGod](https://github.com/LeeGodSRC)
  - *Maybe fixes [#121](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/121)*
- Allow NibbleArray to be 0 length on load - [LeeGod](https://github.com/LeeGodSRC)
- Fixed timing export error in broken host - [LeeGod](https://github.com/LeeGodSRC)
- Fixed chunk scheduler NPE - [LeeGod](https://github.com/LeeGodSRC)
- Fixed issue when Citizens NPC were throwing potion with vanishPatch option enabled - [Whizyyy](https://github.com/Whizyyy)

## [2022.5.3 BUILD 3] - 2022-June-3
- Fixed PacketPlayInBlockPlace decode error - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [#126](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/126)*
  - *Fixed [#125](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/125)*

## [2022.5.3 BUILD 2] - 2022-June-2
- Fixed AsyncFastLight ArrayIndexOutOfBoundsException - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [#113](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/113)*
- Fixed Knockback Enchantment level get shifted by 1 - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [#120](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/120)*
  - *Fixed [#110](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/110)*
- Fixed TNT Merging - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [#109](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/109)*
- Fixed /ping permission command - [Whizyyy](https://github.com/Whizyyy)
- Added dontReadItemNBTDataFromPackets option - [LeeGod](https://github.com/LeeGodSRC)

## [2022.5.3 BUILD 1] - 2022-May-21
**``(New Release)``**

**⚠️ Potential API & Config Changes, Please be aware before updating. ⚠️**

**⚠️ This is an extremely experimental version, Please use it on your own risk. ⚠️**

### Added
- **Migrated ImanitySpigot3's knockback system into ImanityKnockback** - [LeeGod](https://github.com/LeeGodSRC)
- Added V2 editor and file format support - [LeeGod](https://github.com/LeeGodSRC)
  - *This is very meanful for those server who still rely on v2 knockback*
  - *It now supports you directly dragging your knockback profile into imanity/knockback folder and reload*
  - *And edit it the same way as the old one!*
- Use pastebin for get knockback config button - [LeeGod](https://github.com/LeeGodSRC)

https://user-images.githubusercontent.com/36093806/169641719-2062ada0-65c2-49e0-aa5e-0a72895a2e1e.mp4

### Changes
- **Knockback related api has been moved to package** ``dev.imanity.knockback.api`` - [LeeGod](https://github.com/LeeGodSRC)
  - *Check Imanity docs for more detailed changes on API.*
  - *This change is due to our future plan for knockback system.*
- Renamed Velocities behaviour to HitBase - [LeeGod](https://github.com/LeeGodSRC)
- Shift all knockback related config option into `imanity/knockback.yml` - [LeeGod](https://github.com/LeeGodSRC)
  - *No auto config migration, please be aware.*

### Fixed
- Fixed wrong knockback calculation on all behaviour - [LeeGod](https://github.com/LeeGodSRC)
- Fixed V3 editor glitches when multiple people have it opening - [LeeGod](https://github.com/LeeGodSRC)

### Removed
- Removed Classic Knockback Importer - [LeeGod](https://github.com/LeeGodSRC)
  - *Replaced by direct file format support*
- Removed Multiple global knockback support - [LeeGod](https://github.com/LeeGodSRC)
  - *Replaced by single global profile.*
  - *Pretty much no server uses more than one profile by default and applies randomly.*
  - *Have it support multiple random knockback is basically useless.*
- Removed Per world knockback support - [LeeGod](https://github.com/LeeGodSRC)
  - *Will be replaced by plugin soon.*

## [2022.5.1 LTS BUILD 4] - 2022-June-1
- Fixed AsyncFastLight ArrayIndexOutOfBoundsException - [LeeGod](https://github.com/LeeGodSRC)

## [2022.5.1 LTS BUILD 3] - 2022-May-18
- Fixed IncompatibleClassChangeError on modern java versions (java 12+) - [LeeGod](https://github.com/LeeGodSRC)

## [2022.5.1 LTS BUILD 2] - 2022-May-4
- Fixed java 11+ compatibility - [LeeGod](https://github.com/LeeGodSRC)
- Fixed plugin compatibility for SWM and lazarus when AsyncFastLight enabled - [LeeGod](https://github.com/LeeGodSRC)

## [2022.5.1 LTS BUILD 1] - 2022-May-3
**``(New Release)``**

### Fixed
- Fixed some issues for AsyncFastLight addition - [LeeGod](https://github.com/LeeGodSRC)
  - *If you purchased AsyncFastLight addition, please update to this version or above for the best experience.*

## [2022.3.1 BUILD 2] - 2022-April-19
- Added option `zeroHeightCarpets` to imanity config
- Added option `arrowTrajectoryRandomness` to imanity world config
- Do not allow logins while the server is shutting down
- Ensure chunks are always loaded on hard position sets
- Dont broadcast head rotation packet
- Fixed block break desync
- Fixed invisibility for non-parallel tracker
- Reverted useless explode optimization
  - *Fixed [`#100`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/100)*

## [2022.3.1 BUILD 1] - 2022-March-22
**``(New Release)``**

### Added
- Modern Tick Loop - [LeeGod](https://github.com/LeeGodSRC)

### Fixed
- Fixed instant respawn dont clear fire tick in lava - [LeeGod](https://github.com/LeeGodSRC)
- Fixed durability update when other container open - [LeeGod](https://github.com/LeeGodSRC)

## [2022.1.1 BUILD 3] - 2022-February-24
- Added 2022 copyright in config files - [Whizyyy](https://github.com/Whizyyy)
- Fixed durability changer option - [Whizyyy](https://github.com/Whizyyy)
  - *Fixed [`#93`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/93)*
- Don't let packet processing error crash the server - [LeeGod](https://github.com/LeeGodSRC)

## [2022.1.1 BUILD 2] - 2022-February-11
- Added option `forceDurabilityUpdating`
- Improved how durabilityMultiplier works 
  - *Made durability item update only did on specific slot rather than entire inventory for specific situation like armor damage and such to prevent updating inventory when player eating food or drinking potion.*
  - *Fixed [`#86`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/86)*

## [2022.1.1 BUILD 1] - 2022-Januray-15
**``(New Release)``**

### Added
- Added Packet processing while sleeping - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [`#76`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/76)*.
- Added detailed watchdog report information - [LeeGod](https://github.com/LeeGodSRC)
- Added limit login processing per tick - [LeeGod](https://github.com/LeeGodSRC)

### Changes
- Attempt to shutdown scheduler on unload world - [LeeGod](https://github.com/LeeGodSRC)
- Let timings data use Int2ObjectOpenHashMap - [LeeGod](https://github.com/LeeGodSRC)
- Bring old tile entity ticking system back - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [`#81`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/81)*.

### Removed
- Removed `Free from using item while sprint start` patch - [LeeGod](https://github.com/LeeGodSRC)

### Fixed
- Fixed portal not working when cancelling the PlayerPortalEvent - [Whizyyy](https://github.com/Whizyyy)
  - *Fixed [`#83`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/83)*.
- Fixed player disconnect not able to log on back in certain situation - [Whizyyy](https://github.com/Whizyyy)
  - *Fixed [`#75`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/75)*.

## [2021.12.1 BUILD 2] - 2021-December-24
- Added upTo256CharsInChat option - [Whizyyy](https://github.com/Whizyyy)
  - Fixes [`#74`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/74)
- Added options to configure Cannon Optimizations - [Whizyyy](https://github.com/Whizyyy)
  - Fixes [`#73`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/73)
- Added Projectile Custom Through Options - [Whizyyy](https://github.com/Whizyyy)
  - Fixes [`#66`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/66)
- Added eatAndDropFix Option - [Whizyyy](https://github.com/Whizyyy)
  - Fixes [`#67`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/67)
- unloadQueue iterator safe - [LeeGod](https://github.com/LeeGodSRC)
  - Fixes [`#70`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/70)
- Changed tab completion for PLManager on load arg - [Whizyyy](https://github.com/Whizyyy)
- Fixed comments mistake in EnderPearl configuration section - [Whizyyy](https://github.com/Whizyyy)

## [2021.12.1 BUILD 1] - 2021-December-13
**``(New Release)``**

### Added
- FastAsyncLight addition - [LeeGod](https://github.com/LeeGodSRC)
- Added isIntelligence & setIntelligence method in Mob interface - [Whizyyy](https://github.com/Whizyyy)

### Changes
- Optimize VarInts - [LeeGod](https://github.com/LeeGodSRC)
- ASM generated packet constructors - [LeeGod](https://github.com/LeeGodSRC)
- Made entityList iterator safe while accepting add or removal - [LeeGod](https://github.com/LeeGodSRC)
- Player and ItemFrame always run in main-thread for Parallel Entity Tracking - [LeeGod](https://github.com/LeeGodSRC)
- Non-blocking in-progress chunk saving - [LeeGod](https://github.com/LeeGodSRC)

### Code Quality
- Caching relative chunks - [LeeGod](https://github.com/LeeGodSRC)
- Force async catching for unloadQueue anywhere - [LeeGod](https://github.com/LeeGodSRC)
- Added different variants for chunk getter - [LeeGod](https://github.com/LeeGodSRC)

### Bug Fixes
- Free from using item while sprint starts (fixes double eat) - [LeeGod](https://github.com/LeeGodSRC)
- Fixed PlayerChunkMap reflection error for BKCommonLib - [LeeGod](https://github.com/LeeGodSRC)
- Fixed NPE for arrow knockback - [LeeGod](https://github.com/LeeGodSRC)
- Fixed [`#72`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/72) - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 6] - 2021-December-10

### Urgent FIX
- Disable the possibility to send RCE message including inbounds and outbounds - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 5] - 2021-November-28

### Added
- ``HumanEntity#setBlocking(boolean bloocking)`` method in API, allow to force a HumanEntity to block the sword or not - [Whizyyy](https://github.com/Whizyyy)
- TabCompletion for FakeEnvironment command - [Whizyyy](https://github.com/Whizyyy)
- Chunk list & tile entity list caching to improve memory allocation - [LeeGod](https://github.com/LeeGodSRC)

### Changes
- Improved TabCompletion for PluginManager command - [Whizyyy](https://github.com/Whizyyy)

### Bug Fixes
- Chunks inaccessible/broken during their unloading and needed to be used at the same time - [LeeGod](https://github.com/LeeGodSRC)
  - This fix also corrected a bug with the FakeEnvironment command

## [2021.11.1 LTS BUILD 4] - 2021-November-26

### Added
- Added AsyncHeartbeat addition support (new addition coming soon) - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 3] - 2021-November-24

### Added
- Added PlayerOnGroundEvent - [Whizyyy](https://github.com/Whizyyy)

### Changes
- Changed header comments of config files - [Whizyyy](https://github.com/Whizyyy)
- Improved prioritized task queue for chunk loaders - [LeeGod](https://github.com/LeeGodSRC)
- Always update lighting on first tick ignoring randomTickUpdate options from spigot - [LeeGod](https://github.com/LeeGodSRC)

### Bug Fixes
- Don't lock for blocking thread in async chunk whenever unnecessary - [LeeGod](https://github.com/LeeGodSRC)
  - *a bug fix attempt target towards [`#60`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/60)*

## [2021.11.1 LTS BUILD 2] - 2021-November-18

### Bug Fixes
- Fixed incorrect percentage calculation for cave generate rate - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 1] - 2021-November-14

### Added
- Added more precise error display when creating knockack behaviour/modifier - [LeeGod](https://github.com/LeeGodSRC)
- Supported legacy netty (4.0.23.Final) - [LeeGod](https://github.com/LeeGodSRC)
  - *Requires Rancha 2021.11.1 LTS BUILD 2*
  - *Fixed [`#51`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/51)*

### Changes
- Blocking main for block flowing and applyPhysics - [LeeGod](https://github.com/LeeGodSRC)
  - *possibly fixes some weird behaviour in terms of chunk or physics*
- AsyncTabCompleteEvent will now be called from player's tab complete action - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [`#55`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/55)*

### Bug Fixes
- Fixed Knockback editor layout for default minecraft font - [LeeGod](https://github.com/LeeGodSRC)
![old_new](https://user-images.githubusercontent.com/36093806/141652678-bdc7a6a2-590e-4aec-83bf-b280743fe001.png)
- Fixed protocollib patch - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Generate ASM Code for EventExecutor patch - [Whizyyy](https://github.com/Whizyyy)
- Fixed /imanity fillWorld command - [LeeGod](https://github.com/LeeGodSRC)
- Fixed ChunkAnalyzer start / end event calling - [LeeGod](https://github.com/LeeGodSRC)

# **[Pre Release]**

## [2021.10.1 BUILD 14] - 2021-November-11
- Fixed knockback error on java 9+ - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes fishing hook or arrow not working properly and the IncompatibleClassChangeError*

## [2021.10.1 BUILD 13] - 2021-November-10
*Stable release are coming very soon! Get ready for it ;)*

- Added Projectile behaviour support for arrow & fishing hook - [LeeGod](https://github.com/LeeGodSRC)
- Added support for KQueue transport (netty's native transport for mac os) - [LeeGod](https://github.com/LeeGodSRC)
- Knockback Editor interface will now automatically closed when you try to execute other command - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Vanilla behaviour incorrect extra knockback calculation - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 12] - 2021-November-7
- Added more information in /imanitySpigot help command - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 11] - 2021-November-5
- Improved knockback control centre, player section - [LeeGod](https://github.com/LeeGodSRC)
- Improve Metrics - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 10] - 2021-November-1
- Fixed Metrics data sending - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 9] - 2021-October-31
- Added Fake Environment feature and command - [Whizyyy](https://github.com/Whizyyy)
  - *Ability to fake nether / the end environment into overworld, made some special visual for your server!*
- Added option to limit nbt packet decode - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 8] - 2021-October-28
- Changed ``Chunk packet anti xray obfuscate done directly in netty encode`` patch - [LeeGod](https://github.com/LeeGodSRC)
  - *Possibly fixes [`#49`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/49)*
- Improved World Biome Option - [Whizyyy](https://github.com/Whizyyy)

## [2021.10.1 BUILD 7] - 2021-October-26
- Fixed and improved ``/pluginmanager`` command - [Whizyyy](https://github.com/Whizyyy)
- If plugin attempts to async accessing getChunkAt() search from cache first - [LeeGod](https://github.com/LeeGodSRC)
- Chunk packet anti xray obfuscate done directly in netty encode - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes FastAsyncWorldEdit error*
- sendPacketNearby() lookup from world player list - [LeeGod](https://github.com/LeeGodSRC)
- Fixed asyncChunkGeneration error - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes [`#46`](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/46)*

## [2021.10.1 BUILD 6] - 2021-October-24
- Added ``/pluginmanager`` command - [Whizyyy](https://github.com/Whizyyy)
  - *The powerful tool to manage plugins in the server*
  - *Replaces [Plugman](https://dev.bukkit.org/projects/plugman) or any similar plugin management plugins*
- getChunkAt() is now MT-safe if chunk is loaded - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes multiple plugin incompatible issues*

## [2021.10.1 BUILD 5] - 2021-October-21
- Fixed a compatbility issue with some tablist apis - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes [``#40``](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/40)*
- Removed unused patches - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 4] - 2021-October-20
- Show 'Imanity' and some useful infomation when server stop responding - [LeeGod](https://github.com/LeeGodSRC)
- Added book exploit patch - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 3] - 2021-October-19
- Properly handling InterruptedException on server shutdown - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes [``#38``](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/38)*

## [2021.10.1 BUILD 2] - 2021-October-16
- **EXPERIMENTAL** Added server side hit detection - [LeeGod](https://github.com/LeeGodSRC)
- Added option "asyncChunkLoads.chunkGenerateThreads" - [LeeGod](https://github.com/LeeGodSRC)
- Added command "/imanitySpigot fillWorld" - [LeeGod](https://github.com/LeeGodSRC)
- Added debug for entity slice - [LeeGod](https://github.com/LeeGodSRC)
- Chunk Generation is now capable for multi-threads - [LeeGod](https://github.com/LeeGodSRC)
- Use shared random for entities - [LeeGod](https://github.com/LeeGodSRC)
- Dont teleport dead entities - [LeeGod](https://github.com/LeeGodSRC)
- Cache creature type in entity list - [LeeGod](https://github.com/LeeGodSRC)
- Fixed some bugs - [LeeGod](https://github.com/LeeGodSRC)

## [2021.10.1 BUILD 1] - 2021-October-07
**``(New Release)``**

**⚠️ Update required for [``Rancha 2021.09.1 BUILD 2``](https://github.com/Imanity-Software/ImanitySpigot3-git/blob/master/rancha/CHANGELOG.md#2021091-build-1---2021-september-24)**

### Functional
- Added chunkTickRate option - [LeeGod](https://github.com/LeeGodSRC)
- Added ability to change plugin enable / plugin disable color for premium - [Whizyyy](https://github.com/Whizyyy)
- Made <processCpuLoad> display as percentage - [LeeGod](https://github.com/LeeGodSRC)

### Bug Fixes
- Fixed chunk tick algorithm - [LeeGod](https://github.com/LeeGodSRC)
- - Fixed Cactus growing without a limit - [LeeGod](https://github.com/LeeGodSRC)

### Code Quality
- Improved block position allocation - [LeeGod](https://github.com/LeeGodSRC)
- Reduce the amount of chunk lookup in setTypeAndData() - [LeeGod](https://github.com/LeeGodSRC)
- Changed C/I to Github Action - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.3 BUILD 5] - 2021-October-02
- Added classic knockback profile importer - [LeeGod](https://github.com/LeeGodSRC)
  - *The ability to import knockback profiles from ImanitySpigot2*
  - *This only works on knockbacks that was advanced module.*
- Added classic knockback behaviour - [LeeGod](https://github.com/LeeGodSRC)
  - *Repersent advanced module from ImanitySpigot2*
- Added option "asyncChunkLoads.waitForChunks" - [LeeGod](https://github.com/LeeGodSRC)
- Improve algorithm for chunk tick list - [LeeGod](https://github.com/LeeGodSRC)
- Fixed broken plugin nms compatibility in Server Connection - [LeeGod](https://github.com/LeeGodSRC)

https://user-images.githubusercontent.com/36093806/135712330-e1c1d3dd-1716-4458-9596-78c358a97b83.mp4

## [2021.09.3 BUILD 4] - 2021-September-28
- Fixed an NPE error - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.3 BUILD 3] - 2021-September-28
- Fixed some memory leak issues - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.3 BUILD 2] - 2021-September-25
- Added documentation page [``Knockback - Getting Started``](https://docs.imanity.dev/books/imanityspigot-3/page/getting-started) - [LeeGod](https://github.com/LeeGodSRC)
- Added Getting Started page into Control Centre page - [LeeGod](https://github.com/LeeGodSRC)
- Fixed some issue in Control Centre - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.3 BUILD 1] - 2021-September-24
**``(New Release)``**

**⚠️ Update required for [``Rancha 2021.09.1 BUILD 1``](https://github.com/Imanity-Software/ImanitySpigot3-git/blob/master/rancha/CHANGELOG.md#2021091-build-1---2021-september-24)**

### Functional
- Added Metrics [``HERE``](https://bstats.org/plugin/bukkit/ImanitySpigot3/12858) - [LeeGod](https://github.com/LeeGodSRC)
- Improved lag spike logger - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed a problem where old entries were still counted in new lag spike log*
  - *Added tick count display for each entries*

### API Changes
- Added API annotation to every imanitySpigot package API classes - [LeeGod](https://github.com/LeeGodSRC)
- Added Chunk Analyse API - [LeeGod](https://github.com/LeeGodSRC)
  - *Documentation will be added soon*

### Code Quality
- Don't compile mockito-core directly into jar - [LeeGod](https://github.com/LeeGodSRC)

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
