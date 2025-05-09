<img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/main/images/waters%20of%20life%20wj%20image.webp" target="_blank"></a>

---

<p align="center">
  <a href="https://www.nexusmods.com/fallout3/mods/26081">Nexus Page</a> ·
  <a href="README.md">Installation</a> ·
  <a href="changelog.md">Changelog</a> ·

---

# Changelog

## 1.2.4
> [!tip]
> **Safe Midgame**

List:
- Cleared my Wabbajack patch cache. Why? To see if it changes anything with the issues that Steam users are having.

## 1.2.3
> [!caution]
> **I haven't mentioned this in previous releases but this is probably not safe to update midgame due to the addition of Intro Street Bus and Trailer Ruins.**

List:
- Added Geck Patcher - optional patcher for if you want to use the GECK Extender that was added to the list in 1.2.2
- Reset `falloutprefs.ini` because it was broken and caused crashes for some users
- Renamed Post Installation separator to Patches and Optionals
- Renamed Optionals separator to Other Profiles

Bugfixes:
- Added FO3 Decal Flickering Fix
- ~~Added Mostly Fixed FaceGen Tints~~ Edit: I forgot to add these.
- Added Damage To Armor Fix

User Interface:
- Added Clean Vanilla HUD
- Hid repair_meter_pips.dds because it's not part of the FO3 UI
- Added Clean Vanilla HUD FO3 Aesthetics Patch
- Removed CNDArrows code from hud_main_menu.xml to fix visual bug
- Downgraded Vault Boy Paper Doll 5.0 to Clean Vault Boy Paper Doll 1.2 because I don't like the v5 style

Gameplay:
- Added Statics to Vanilla Items
- Removed Statics to Vanilla Items - a careful inspection revealed that Goodies covers everything this mod does except for `000918E5`, `0400DF04`, `0401206D`
- Added BD-SM
- Moved Fallout 3 Quick Start to Gameplay from Overhauls
- Moved Zeta Enable Somah Paulson to Gameplay from Overhauls

Content:
- Added Laurens Bathroom Poetry
- Added Intro Street Bus and Trailer Ruins Unofficial Fixed
- Added Prototype Medic Power Armor Dialogue Expansion
- Moved Auto Gates to Content from Overhauls
- Moved Fallout 3 Ending Restored to Content from Overhauls
- Moved the Nicer Goodbye mods to Content from Overhauls
- Moved The Megaton Walkway to Content from Overhauls

Audio:
- Added Subtle Rifle Equip Sound
- Added PhySFX
- Added A.W.S.O.M.E - Fallout 3 Edition

Visuals:
- Added Anniversary Anim Pack
- Added FNV Clean Anims - Anniversary Edition
Hid the following files/folders because they're not needed or bugged in some way:
- `Config` folder - from Anniversary Anims, B42 Optics configs
- `Meshes\AnimGroupOverride` folder - from FNV Clean Anims, kNVSE animations
- `rockbiter_AnimationSounds.esp` - FNV Clean Anims
- `1hpAttack3IS.kf` - Anniversary Anims, bugged recoil for alien/laser pistols
- `1hpJamA.kf` - Anniversary Anims
- `1hpJamF.kf`
- `1hpJamH.kf`
- `1hpJamK.kf` - FNV Clean Animations
- `1hpReloadB.kf` - Anniversary Anims
- `1hpReloadC.kf` - Anniversary Anims
- `1hpReloadD.kf`
- `1hpReloadE.kf`
- `1hpReloadF.kf`
- `1hpReloadG.kf` - Anniversary Anims
- `1hpReloadH.kf`
- `1hpReloadI.kf` - Anniversary Anims
- `1hpReloadJ.kf` - Anniversary Anims
- `1hpReloadK.kf`
- `2haJamC.kf`
- `2haJamH.kf` - Anniversary Anims
- `2haReloadB.kf`
- `2haReloadC.kf`
- `2haReloadD.kf`
- `2haReloadH.kf`
- `2hhReloadC.kf`
- `2hhReloadD.kf` - Anniversary Anims
- `2hhReloadE.kf`
- `2hhReloadF.kf` - Anniversary Anims
- `2hlReloadA.kf` - Anniversary Anims
- `2hlReloadE.kf`
- All variants of `2hrAttack3.kf` - Anniversary Anims
- `2hrJamB.kf` - FNV Clean Anims
- `2hrJamD.kf`
- `2hrReloadA.kf` - Anniversary Anims
- `2hrReloadB.kf`
- `2hrReloadC.kf` - Anniversary Anims
- `2hrReloadD.kf`
- `2hrReloadE.kf` - Anniversary Anims
- `2hrReloadF.kf` - Anniversary Anims
- `2hrReloadG.kf`
- `2hrReloadH.kf` - Anniversary Anims

LOD:
- Added Fallout 3 LOD
- Added plugin that adds the Use LOD Data flag to MegatonWorld and ParadiseFalls worldspaces, basically a port of Wasted Return of LOD by GoatOfArmor
- Removed Arefu LOD (included in Fallout 3 LOD)
- Regenerated LOD with Keep Specular enabled for Object LOD and Terrain LOD meshes

Patches and Optionals:
- Removed Character Overhaul UUF3P Patch because Ruy updated the mod
- Moved Fallout 3 Quick Start to here from Gameplay
- Moved Fugacity - Fallout 3 Quick Start to here from Gameplay
- Flagged FO3_Optimization - UUF3P Patch as an ESM
- Flagged FO3_Optimization - Goodies Patch as an ESM
- Flagged Megaton Walkway - UUF3P Patch as an ESM

## 1.2.2

List:
- Added new splash screen

User Interface:
- Added Clean Visual Objectives
- Added Companion Wheel (FOSE)

Gameplay:
- Added Essential Hired Companions by me

Audio:
- Added Ambient Wasteland 2
- Removed Ambient Wasteland 2
- Added CONELRAD 640-1240 - Civil Defense Radio and decompressed its plugin
- Removed CONELRAD 640-1240 - Civil Defense Radio

Visuals:
- Updated Megaton Illuminated to version 13
- Removed Fallout Street Lights and Street Lights Script Fix - Don't really want to include a mod that predates 3/5 of the game's DLCs, plus Clarity and True Weathers don't get dark enough to warrant street lights
- Added Cataract Eyes
- Removed Cataract Eyes
- Added Windows To The Soul - Full Vanilla Eye Retexture
- Removed Lost in Light - An Eye Improvement Mod (replaced)
- Added Vanilla Hair - No Shine

LOD:
- Removed terrain LOD - not needed with vanilla textures
- Added Contrasted LOD Noise Texture - Improved LOD Noise Texture stays for the ModdingLinked profiles for parity with the FO3 guide

## 1.2.1

LOD:
- Updated Much Needed LOD FO3 to version 2
- Regenerated LODGen output with xLODGen beta 130

Visuals:
- Disabled Atmospheric Sun Glare in main profile to use the one included in True Weathers instead
- Updated Megaton Illuminated to version 11

Post Installation:
- Updated DXVK and DXVK - HDR to 2.5.3
- Fixed missing DXVK

Optionals:
- Updated Megaton Illuminated UUF3P Patch

## 1.2.0
List:
- Added new ModdingLinked Extended profile

Custom INI:
- Removed TerrainManager ini tweaks (not needed and caused certain LOD objects to not load)

Utilities:
- Added No Exit to Main Menu
- Updated ButcherPete FOSE to 2.5

Bugfixes:
- Updated Stewie Tweaks Essentials INI to 1.04

Gameplay:
- Replaced Marathoner with Simple Sprint Fallout 3
- Removed Can Has Recoil because I can't really notice the recoil (at least on a couple semiautos I tried)

Visuals:
- Replaced Alternative Megaton Lighting with Megaton Illuminated
- Added New Vegas version of Accurate NASA Stars which has the star texture correctly saved with DXT1 compression and includes gamesetting tweaks to make it so the north star points north

Optionals:
- Updated ATMOS and Fugacity UUF3P patches
- Added Megaton Illuminated UUF3P patch
- Added Megaton Illuminated Goodies patch
- Added FOMOD so it's easier for me to setup the patch selection for each profile

## 1.2.0rc2
LOD:
- Packed LOD output into a BSA and merged LOD resource plugins

List:
- Decompressed plugins for Fugacity and its UUF3P patch

## 1.2.0rc1

List Updates

Profiles:
- Added a new Classic profile that uses Clarity and the older Enhanced Night Sky and krzymar HI-RES Moon retextures
- Added a new ModdingLinked Basics profile that has only the utilities and bug fixes from the ModdingLinked FO3 mod guide

MO2:
- Updated and switched MO 2.5.1rc2 to MO 2.5.2-ML1.5

Utilities:
- Updated patched vanilla ESMs to 1.6
- Removed Fallout 3 Heap Replacer because of its experimental nature and its questionable reliabilty judging by the bug reports
- Updated Command Extender to 23.0

Bugfixes:

- Updated UUF3P to 3.4.9
- Updated UUF3P patches to account for any new changes
- Updated Stewies Tweaks Essentials INI to 1.02
- Updated Viewmodel Shading Fix - FOSE to 2.2

Visuals:
- Removed Instant and Faster Pipboy because I realized the vanilla animation speed isn't that bad

LOD:
- Regenerated LOD with new resources and generated terrain LOD as well

Mod Additions

Utilities:
- Decompressed BSAs
- OGG Vorbis Libraries
- fose fps fix
- Triple Buffering - FOSE
- ButcherPete FOSE
- Yet Another Steam Overlay Fixer - fixes Steam playtime tracking not working when running the game through MO2

Bugfixes:
- Interior Optimization Project

Visuals:
- Character Overhaul - replaces FO3 Redesigned
- Atmospheric Lighting Tweaks
- Enhanced Vanilla Stars
- HD NASA Moon

LOD:
- Red Rocket - LOD Improved
- Arefu LOD
- Much Needed LOD FO3
- More LOD

## 1.1.0

- Added Sunlight Fix - FOSE

- Added Viewmodel Shading Fix - FOSE

- Added zLib Updated - FOSE

- Updated Stewie's Tweaks Essentials INI to version 1.01

- Replaced Simple Sprinting with Marathoner

- Replaced Clarity with True Weathers (Still included in the list if you prefer it)

## 1.0.1

- Fix Vanilla UI Plus not downloading

- Remove ModOrganizer.ini to prevent copying over the installation paths from my install. You might want eye protection for this one as MO2 will now use the default light theme

## Version 1.0.0
Initial Release
