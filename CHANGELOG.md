# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

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
