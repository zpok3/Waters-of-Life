![waters of life logo](images/waters%20of%20life%20wj%20image.webp)

---

<p align="center">
  <a href="https://www.nexusmods.com/fallout3/mods/26081">Nexus Page</a> ·
  <a href="README.md">Installation</a> ·
   <a href="changelog.md">Changelog</a> ·
<a href="planned-additions.md">Planned Additions</a> ·
<a href="gameplay-guide.md">Gameplay Guide</a> ·

   ---
# Read-Me
- [Introduction](#introduction)
  - [List Contents](#list-contents)
  - [Requirements](#requirements)
- [Setup](#setup)
    - [Preparation](#preparation)
    - [Clean Install](#clean-installation)
    - [Starting the Game](#starting-fallout-3)
- [Installation](#installation)
- [Post Installation](#post-installation)
- [Extra stuff you should know](#extra-stuff-you-should-know)
- [Credits](#credits)

# Introduction
Waters of Life is a lightweight vanilla plus Wabbajack mod list for Fallout 3. It features essential vanilla bug fixes, performance optimizations, restored cut content, and a few gameplay features you might be used to from more modern games. If you want an easy to install modlist that doesn't stray too far from vanilla, look no further!

## List Contents
You can look [here](https://loadorderlibrary.com/lists/waters-of-life-4) if you're curious about what mods are included.

## Requirements
- An **English** copy of the game with the all of the DLCs from [Steam](https://store.steampowered.com/app/22370/Fallout_3_Game_of_the_Year_Edition/) or [GOG](https://www.gog.com/en/game/fallout_3_game_of_the_year_edition).
  - Only the English version is supported. I understand that this may be frustrating for non-English speaking users, but due to the core file differences between the different versions, only one version can be supported.
> [!tip]
> The GOG version is recommended due to minor issues with the Steam version of the game. Steps are provided for potential solutions.
- Windows 10 or higher (64 bit).
- The latest VC++ Redistributables:
  - [VC++ AIO](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)
1. Extract the archive and run `install_all.bat` as an administrator.
    - [2015-2022 X64](https://aka.ms/vs/17/release/vc_redist.x64.exe)
    - [2015-2022 X86](https://aka.ms/vs/17/release/vc_redist.x86.exe)
    - Restart your PC.
- A text editor ([Notepad++](https://notepad-plus-plus.org/) is recommended but the default Windows notepad will work).
- An archiving tool ([Nanazip](https://apps.microsoft.com/store/detail/nanazip/9N8G7TSCL18R?hl=en-us&gl=us) is recommended).
- The latest GPU drivers (either [NVIDIA](https://www.nvidia.com/Download/index.aspx), [AMD](https://www.amd.com/en/support) or [Intel](https://www.intel.com/content/www/us/en/search.html#q=&sort=relevancy&f:@tabfilter=[Downloads]&f:@stm_10385_en=[Graphics])).
- The latest release of [Wabbajack](https://www.wabbajack.org/).
- A [Nexus Mods](https://users.nexusmods.com/register) account (Premium is recommended for uncapped download speeds and fully automated modlist installation).

## Recommended Specs
I don't really know exact specs but if your PC can easily run the game at 1080p max settings at 60+ FPS, you can probably run this list just fine.

# Setup
## Preparation
**Enabling file extensions:**
1. Open File Explorer.
2. Select the `View` tab at the top.
3. Enable `File name extensions` in the `Show` section.

**Disabling Base Address Randomization:**

Base Address Randomization is a security feature in Windows that allows program's starting address to be randomized, which is not the expected behavior in 32-bit programs like Fallout 3. This **leads to crashes** in a modded game. This is disabled by default but it's recommended to make sure it's disabled as a sanity check.
1. Open `Windows Security` from your Start Menu.
2. Click on `App and Browser control` in the left sidebar.
3. Click on `Exploit Protection Settings` under `Exploit Protection`.
4. Ensure `Force randomization for images (Mandatory ASLR)` is set to `Use default (Off)`.

> [!tip]
If you don't want to change the global setting, you can add an exception just for the game:
> 1. Click on `Program settings`.
> 2. Click on `Add program to customize`.
> 3. Select `Add program by name`.
> 4. Enter `Fallout3.exe` in the box and save.
> 5. Find the newly created entry on the list and click `Edit`.
> 6. Find `Force randomization for images (Mandatory ASLR)`.
> 7. Check `Override system settings`, and set the toggle to `Off`.

## Clean Installation
Waters of Life requires a completely clean installation of Fallout 3. This means completely deleting both the game folder and all INI files located in `Documents\My Games\Fallout3` then reinstalling the game through Steam/GOG. The game MUST be installed outside of any default Windows folders, such as `Program Files (x86)`, `Program Files`, your `Desktop`, or `Documents`. Additionally, it is recommended to install the game on an SSD if possible to improve load times and decrease stuttering.

<details>
<summary>Steam Install Instructions</summary>

- The following instructions are only for anyone who has Steam installed in `Program Files (x86)` AND only have a single drive installed as Steam only allows one library folder per drive.
- Skip to step 1 of `Installing the game` if you have Steam installed outside of `Program Files (x86)` or have a separate drive to install games to.

1. Completely exit out of Steam using Task Manager or System Tray.
2. Download `steam_library_setup_tool-3.2.exe` from [here](https://github.com/LostDragonist/steam-library-setup-tool/releases/download/3.2/steam_library_setup_tool-3.2.exe).
3. Run the file and click `Add Row` to add a new entry.
4. Type the chosen path under `Path`, e.g. `C:\Games\SteamLibrary`.
5. Click `Accept` and then `Yes` if prompted to create a new folder.
6. Click `OK` when the tool asks to exit.

**Installing the game:**
1. Open Steam and go to your `Library`.
2. Find Fallout 3 in the list and click `Install`.
3. Under `Install to:`, select a library folder of your choice that is outside of any default Windows folders. If you created a custom Steam Library earlier, it will be the second **(C:)** entry.
4. Select `Next` and wait for the install to finish.

</details>

<details>
<summary>GOG Install Instructions</summary>

1. In GOG Galaxy, go to your `Library`.
2. Select `Fallout 3: Game of the Year Edition` and click `Install`.
3. Set the `Install to` folder to a folder of your choice, e.g. `C:\GOG Games`.

</details>

## Starting Fallout 3
Start the game and exit once you're at the main menu. This will ensure any settings files needed by Wabbajack are created.

> [!important]
**Key Terminology**
>
> As we go through this install guide there are two folders that we will refer to often:
> - **Root folder**: The folder that the game is installed in.
>    - For Steam: `Steam\steamapps\common\Fallout 3 goty`
>    - For GOG: `GOG Galaxy\Games\Fallout 3` (unless you manually changed it)
> - **Data folder**: Where all of the game's assets are located.
>    - For Steam: `Steam\steamapps\common\Fallout 3 goty\Data`
>    - For GOG: `GOG Galaxy\Games\Fallout 3\Data` (unless you manually changed it)

# Installation

1. Create a folder for Wabbajack outside of any default Windows folders.
  - Example: `C:\Modding\Wabbajack`

2. Place the downloaded Wabbajack.exe in this folder and run it.
3. Select `Browse Modlists`, check the `Non-featured` box and set the game to `Fallout 3`. Then select Waters of Life and click `Download and Install`.
4. In `Installation Location`, select a folder that is not:
  * The Steam folder,
  * Any default Windows folders,
  * The Game folder,
  * The folder where you put Wabbajack.exe.

Example: `C:\Modding\Waters of Life`

**Update**: The default location `C:\Modlists\WOL` that is set by Wabbajack 4.0.0.0+ should work just fine.

5. Click `Install` to begin the installation.
6. Accept the Nexus Mods API request.
7. If you are not a Premium user you will need to manually click download for each mod.
8. Once complete, Wabbajack will show a green `Installation Complete` screen.
> [!important]
> As of version 1.2.6 you will have to manually download [Pintocat's Metro Map replacer](https://taleoftwowastelands.com/viewtopic.php@t=7779) and place it into the modlist's downloads folder, then click `Retry`. This is due to a Wabbajack bug where automated Google Drive downloads don't work. They are [aware](https://github.com/wabbajack-tools/wabbajack/issues/2782) of the issue.

> [!tip]
> If you see a red `Installation Failed` screen, try log-in again through the Wabbajack settings, then reinstall the list to the same folder.

# Post Installation

## Exclusions
This operation is required because Windows can block MO2 and mod files from loading due to how MO2's virtualized filesystem works.
1. Open Windows Security.
2. Open `Virus and Threat Protection`.
3. Click `Manage Settings` under `Virus and threat Protection settings`.
4. Scroll down and click `Add or remove exclusions` under `Exclusions`.
5. Add a `Folder` exclusion and point it to the `Installation Location` folder.
> [!important]
> If you are using a third-party antivirus, you will need to find the exclusions menu and add one to the same folder.

## Root Mods
Next we will run the Fallout Anniversary Patcher, its features include a Mod Limit Fix, Intel HD Graphics Bypass, Games for Windows Live Disabler, and specifically for Steam/Epic it applies a 4GB/LAA patch and downgrades the game executable to 1.7.0.3 for mod compatibility.
1. In your `Installation Location` folder, open the `__Root Mods` folder.
2. Copy **everything** to the game's `Root` folder.
3. Still in the game's `Root` folder, double-click on `Patcher.exe` to run it.
4. A command prompt should show up, run for a few seconds, then read as follows:

>Patching completed successfully.
>
>Press any key to continue . . .

5. Close the command prompt and a file named `Fallout3_backup.exe` should appear in the game's `Root` folder.

## BSA Decompressor
Decompresses the vanilla BSA files to reduce loading times and stuttering. Increases the size of the game by about 1.64GB if you decompress directly into the `Data` folder, otherwise it takes up about 3.38GB if it's in a mod folder in the `Installation Location` folder.
1. In your `Installation Location` folder, open the `__BSA Decompressor` folder.
2. Run `FO3 BSA Decompressor.exe`.
3. The `Fallout 3` and `Decompressed Archives` path should be filled by default (Root and Data folder respectively).

If they aren't, close the program and re-run the game's launcher to generate the required registry key.

> [!tip]
> If you intend to install [Tale of Two Wastelands](https://thebestoftimes.moddinglinked.com/) or don't want to verify your game files everytime you need to update the list, you can output the decompressed BSAs to a mod in MO2:
> 1. In MO2 click the ![mo2 open folders menu](images/folders%20menu.webp) button and select `Open Mods folder`.
> 2. Create a folder called `[NoDelete] Decompressed BSAs` and then copy its path (open the folder, right click the address bar, and select `Copy address as text`).
> 3. Close MO2.
> 4. Paste the path you copied in step 2 into the `Decompressed Archives` text field.

4. Click `Decompress`, wait for the process to finish, then exit out of the program once finished.

## Mod Organizer 2 Setup
1. Launch `ModOrganizer.exe` from your `Installation Location` folder.
2. If you see a pop-up called `Register?`, select `Yes`.
3. If you use the **Steam** version of the game, enable the mod `Yet Another Steam Overlay Fixer` (additionally enable the mod `Supplementary Files - Fallout 3 (Regular)` if you have that instead of the GOTY edition) under the `Patches and Optionals` separator.
4. If you would like to play through the intro of the game, disable the mods `Fallout 3 Quick Start` and `Fugacity - Fallout 3 Quick Start Patch`, also under the `Patches and Optionals` separator.

> [!note]
> If you output the decompressed BSAs to a mod folder, a mod called `[NoDelete] Decompressed BSAs` should appear in the bottom of the left pane of MO2. Make sure to enable it as well. If it is greyed out you may have output the decompressed BSAs to the wrong folder. Find out where they are (tip: only three of the base game's BSAs are decompressed - Meshes, Misc and Textures) and move them to the folder you created earlier.
> 
> Additionally, something I completely forgot about is that for most of the list's life it did not include a `ModOrganizer.ini`, meaning the end user would have to go through instance creation when they first start MO2. This may have masked issues related to a mismatched Steam App ID for users who have the base game + all DLC purchased separately instead of the GOTY edition. To fix this (if it applies to you), in MO2 go to `Settings -> Workarounds` and change the Steam App ID to `22300`.

## Game Settings
There are four profiles you can choose from; the default profile, the Classic profile, the ModdingLinked Basics profile, and the ModdingLinked Extended profile. Since the INI files are profile specific, you must use the drop-down menu on the top of your modlist in MO2 to select the profile you would like to configure settings for.
1. Open the game launcher using the `Fallout Launcher` option in MO2. You may need to add it manually if you have the Steam version of the game by clicking `<Edit...>` from the executables dropdown menu, selecting the + icon and choosing `Add from file...`.
> [!important]
> If you use Steam, the game may not start when you try to run it through MO2. The problem may have something to do with the [updated launcher](https://store.steampowered.com/news/app/22370/view/4160842270244401930?l=english). To fix this you can follow this [guide](https://github.com/zpok3/Waters-of-Life/blob/main/steam-downgrading-guide.md) to downgrade the game. Or you can try resetting your INIs by clicking the ![mo2 folders menu](images/folders%20menu.webp) button, selecting `Open Profile folder`, and deleting `fallout.ini` and `falloutprefs.ini`. Then refresh MO2 by pressing `F5` and follow [these](#ini-settings) steps to configure some settings that will have been reset by this process.

2. Inside the launcher click `Options` and do the following:
    1. Select `Ultra` preset.
* If you have a very weak PC, you can select the `Medium` preset instead.

  2. Set `Resolution` to your monitor's native resolution.
* If you can't find the right resolution in the launcher's list, do the following:
    
    1. Close the launcher.
    2. Click the ![mo2 tools menu](images/tools%20menu.webp) button and select `INI Editor`.
    3. Select the `FalloutPrefs.ini` tab.
    4. Change the following settings in the `[Display]` section:
    * `iSize W` = your screen width
    * `iSize H` = your screen height
> [!note]
If you use an Ultrawide display also follow [these](#ultrawide-support) steps.

3. Close the launcher.

## Performance Guide
- **Set an FPS Limit**: It's recommended  to limit your FPS to `120` or lower as the game can still have issues even with the High FPS Fix. For instructions on how to set up [Rivatuner Statistics Server](https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/) (if you use MSI Afterburner you probably already have this installed), please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters). It's written for New Vegas but you can very easily apply it to Fallout 3 by replacing the part where you select `FalloutNV.exe` with selecting `Fallout3.exe`.
- **DXVK with DXGI**: Highly recommended if you want improved input latency and VRR support.  Version 2.0 of DXVK requires a GPU that supports Vulkan 1.3 - if you have an AMD Radeon RX 400 series GPU or newer (except RX 455 OEM), NVIDIA GeForce 900 series GPU or newer, or Intel HD 510/530 GPU or newer you should be able to use DXVK 2.0 (source: [TechPowerUp GPU Database](https://www.techpowerup.com/gpu-specs/)).
  - If you use an AMD GPU, all you have to do is enable the mod `DXVK` under the `Patches and Optionals` separator in MO2. If you use a Nvidia GPU you'll also need to follow steps 2-6 under [**Enabling Flip Model (DXVK with DXGI)**](https://performance.moddinglinked.com/falloutnv.html#dxvk-flip).
  - If you have issues with the latest version or your GPU doesn't support Vulkan 1.3 you can try the 1.10.3 version. If you are having issues on an Intel iGPU you can try the 1.10.1 version.
For more information on DXVK, VRR, HDR, and Alt-Tabbing, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html). 

## Launching the Game
1. Make sure the dropdown box on the right is set to `Fallout 3` and press the Run button.

> [!note]
> We run the game directly instead of through the FOSE loader because the Fallout Anniversary Patcher we ran earlier enables the game executable to load FOSE automatically if available.

2. You're all set! Everything is already configured by default so you can hop right into a new game!

# Updating the List

1. Add the [NoDelete] prefix to the name any mods you added after installation.
Example: `[NoDelete] My awesome mod`
2. **Verify files** on **Steam** or **GOG Galaxy** (only if you output your decompressed BSAs directly into your game's `Data` folder, otherwise skip to step 3).
3. Rerun the Anniversary Patcher (unless you skipped step 2) and optionally the BSA Decompressor (unless you installed it as a mod in MO2).

# Extra stuff you should know

## Ultrawide Support 
- Enable `bUltrawideSupport` in the mod `Stewie Tweaks Essentials INI` (or whatever Stewies Tweaks INI is active for the current profile since there are a handful of them to account for some profiles not having Iron Sights Plus).

## Mod Profiles
- **Classic Profile:** Same as the default profile but uses Enhanced Night Sky, krzymar HI-RES Moon, Alternative Megaton Lighting Plus, and Clarity instead of Enhanced Vanilla Stars, Accurate NASA Stars, HD NASA Moon, Atmospheric Lighting Tweaks, Megaton Illuminated, and True Weathers.

- **ModdingLinked Basics Profile:** Just the Utilities and Bug Fixes from the [FO3 Mod Guide](https://thebestoftimes.moddinglinked.com/fo3.html) written by ModdingLinked.

- **ModdingLinked Extended Profile:** The full version of the FO3 Mod Guide written by ModdingLinked.

## INI Settings
If you had to reset your INIs to get the game to start, these are a few settings that will be reset that you must reapply.
- Go to `Settings -> Controls -> Action Mapping` and set your run key to `L-Shift` to allow sprinting (default and Classic profiles only):
![run key](images/run%20key.webp)
> [!tip]
> Alternatively, open MO2's INI editor, select `falloutprefs.ini`, find `Run=002AFFFF` and replace it with `Run=0036FFFF`.
-  Go to `Settings -> Display` and set the HUD color to these colors:
![hud colors](images/hud%20colors.webp)
> [!tip]
> Alternatively, open MO2's INI editor, select `falloutprefs.ini`, find `uHUDColor=452952319` and replace it with `uHUDColor=2868873471`
- Scroll down and enable `General Subtitles`. Alternatively, open MO2's INI editor, select `falloutprefs.ini`, find `bGeneralSubtitles` and enable it (replace 0 with 1).

# Credits
[Qolore7](https://github.com/Qolore7) for some of the more obscure mods that I found via his Wabbajack list Lost Liberty.

[Ungeziefi](https://github.com/Ungeziefi) and [Wall SoGB](https://github.com/WallSoGB) for the resources available at [ModdingLinked](https://moddinglinked.com/index.html).

Belts the Puppet for helping me figure out what's wrong with my INIs.
