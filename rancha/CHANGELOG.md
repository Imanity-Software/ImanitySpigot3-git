# Changelog

### Contributors:
- [LeeGod](https://github.com/LeeGodSRC)
- [Whizyyy](https://github.com/Whizyyy)

All notable changes to this project will be documented in this file.

## [2023.2.1 BUILD 4] - 2023-March-30
-  Bumped FastUtil to 8.5.11 - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 BUILD 3] - 2023-February-23
- Added download properties system. - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 BUILD 2] - 2023-February-18
- Fixed Incompatible error with modern JRE/JDK. - [LeeGod](https://github.com/LeeGodSRC)

## [2023.2.1 BUILD 1] - 2023-February-17
**``(New Release)``**

Added:
- Added enterprise plan support
- Added startup flag `-Dimanity.version=(LATEST/LTS/*spigot version*)`
  - *Resolved [#124](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/124)*

## [2022.7.1 BUILD 1] - 2022-July-1
- Upgraded JavaAssist to 3.29.0-GA - [LeeGod](https://github.com/LeeGodSRC)
- Upgraded JNA to 5.11.0 - [LeeGod](https://github.com/LeeGodSRC)
- Upgraded OSHI to 6.1.6 - [LeeGod](https://github.com/LeeGodSRC)
- Upgraded Log4J2 to 2.18.0 - [LeeGod](https://github.com/LeeGodSRC)

## [2022.5.1 BUILD 2] - 2022-May-22
- Downgraded netty versions to 4.1.60.Final - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixed [#117](https://github.com/Imanity-Software/ImanitySpigot3-git/issues/117)* 

## [2022.5.1 BUILD 1] - 2022-May-18
- Added license key startup flag support `-Dimanity.license={license}` - [LeeGod](https://github.com/LeeGodSRC)
- Bumped fastutil versions to 8.5.6 - [LeeGod](https://github.com/LeeGodSRC)
- Bumped netty versions to 4.1.73.Final - [LeeGod](https://github.com/LeeGodSRC)
- Updated 2k22 copyright in config files - [Whizyyy](https://github.com/Whizyyy)

## [2021.11.1 LTS BUILD 4] - 2021-December-16
- Made Jna runtime library download - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 3] - 2021-December-10
- Bumped Log4j versions to 2.15.0 - [LeeGod](https://github.com/LeeGodSRC)
  - *Major exploit fix: https://www.lunasec.io/docs/blog/log4j-zero-day/*

## [2021.11.1 LTS BUILD 2] - 2021-November-14

### Changes
- Added Support for legacy netty - [LeeGod](https://github.com/LeeGodSRC)
  - *Requires ImanitySpigot3 2021.11.1 LTS BUILD 1*
- Added Hash check when launching spigot failed or updating spigot - [LeeGod](https://github.com/LeeGodSRC)
  - *Fixes server downtime when update failed*
- Generates netty version properties file to ensure plugin compatibilitv - [LeeGod](https://github.com/LeeGodSRC)

## [2021.11.1 LTS BUILD 1] - 2021-November-07
- Automatically updating rancha depend on the spigot you are updating to - [LeeGod](https://github.com/LeeGodSRC)
- Fixed Java 17 compatibility - [LeeGod](https://github.com/LeeGodSRC)
- Fixed compatibility issue to some jvm forks - [LeeGod](https://github.com/LeeGodSRC)
- Use maven api to download maven libraries - [LeeGod](https://github.com/LeeGodSRC)
- Added support for Source plan - [LeeGod](https://github.com/LeeGodSRC)
- Fixed MalformedException when yaml are different encoding - [LeeGod](https://github.com/LeeGodSRC)

## [2021.09.1 BUILD 2] - 2021-October-07
- compatible to ``2021.10.1 BUILD 1`` ImanitySpigot3 - [Whizyyy](https://github.com/Whizyyy)
- Made default message display Imanity - Software instead of [Imanity] for ``/imanity`` - [Whizyyy](https://github.com/Whizyyy)
- Improved configuration section for Premium - [Whizyyy](https://github.com/Whizyyy)

## [2021.09.1 BUILD 1] - 2021-September-24
- Added mockito library - [LeeGod](https://github.com/LeeGodSRC)
- Added ability to write paste with specific content type - [LeeGod](https://github.com/LeeGodSRC)
- Removed thread displaying in log4j format - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 5] - 2021-Augest-22
- Warning when netty patch failed because of Java 12+ - [LeeGod](https://github.com/LeeGodSRC)
  - *This error is not able to patch, Servers need ``--illegal-access=permit`` in their startup flag inorder to fix it*
- If launching Spigot JAR failed, Rancha will suggest to update and give 30 seconds of wait time - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 4] - 2021-Augest-22
- Fixed an error on startup - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 3] - 2021-Augest-22
- Improved Security - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 2] - 2021-Augest-16
- Added option forceNettyUseUnpoolBuffer - [LeeGod](https://github.com/LeeGodSRC)

## [2021.08.1 BUILD 1] - 2021-Augest-3
- Initial Support for Raisensu Version Check - [LeeGod](https://github.com/LeeGodSRC)
- Added Displaying current version in ``!update`` - [LeeGod](https://github.com/LeeGodSRC)
- Added mentioning to License FAQ - [LeeGod](https://github.com/LeeGodSRC)
