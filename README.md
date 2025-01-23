<img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/refs/heads/main/images/logo.jpeg" target="_blank"></a>

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
- [Installation](#installation)
    - [Clean Install](#clean-installation)
    - [Starting the Game](#starting-fallout-3)
    - [Installation](#installation)
- [Post Installation](#post-installation)
- [Extra Stuff you should know](#extra-stuff-you-should-know)
- [Credits](#credits)

# Introduction
A lightweight vanilla plus Wabbajack mod list for Fallout 3. Intended to bring a Viva New Vegas-like experience to Fallout 3

# List Contents
You can look [here](https://loadorderlibrary.com/lists/waters-of-life-1) if you're curious about what mods are included.

  # Requirements
  - A fresh installation of the **English** version of the game with the all of the DLCs from Steam or GOG
  * Only the English version is supported. I understand that this may be frustrating for non-English speaking users, but due to the core file differences between the different versions, only one version can be supported. 
  * The game MUST be installed outside of any default Windows folders, such as `Program Files`, your `Desktop`, or `Documents`. If you have your Steam library in any of these locations, please follow [these](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) instructions to move it.

- [Microsoft Visual C++ Redistributable Package](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)

- The latest release of [Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) installed outside of any default Windows folders.

- The latest .wabbajack file for this modlist downloaded from either the [releases](https://github.com/zpok3/Waters-of-Life/releases) page or the [Nexus](https://www.nexusmods.com/fallout3/mods/26081) page.

# Installation:

## Clean Installation
Waters of Life requires a completely clean installation of Fallout 3. This means completely deleting both the game folder and also the folder located in `Documents\My Games\Fallout3` then reinstalling the game through Steam/GOG. The game MUST be installed outside of any default Windows folders, such as `Program Files`, your `Desktop`, or `Documents`. If you have your Steam library in any of these locations, please follow [these](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) instructions to move it.

## Starting Fallout 3
Start the game and exit once you're at the main menu. This will ensure any settings files needed by Wabbajack are created.

## Installation

1. Create a folder for Wabbajack outside of any default Windows folders.

Example: `C:\Modding\Wabbajack`

2. Place the downloaded Wabbajack.exe in this folder and run it.
3. Select `Install from Disk` in the Wabbajack app. You will have to manually select where you downloaded the wabbajack file in the `Target Modlist` box.
4. In **Installation Location**, select a folder that is not:
  * The Steam folder,
  * Any default Windows folders,
  * The Game folder,
  * The folder where you put Wabbajack.exe.

Example: `C:\Modding\Waters of Life`

5. **Begin** the installation.
6. Accept the Nexus Mods API request.
7. If you are not a Premium user you will need to manually click download for each mod.
8. Once complete Wabbajack, will show a green **Installation Complete** screen.
  * If you see a red **Installation Failed** screen, try log-in again through the Wabbajack settings, then reinstall the list to the same folder.

# Post Installation

## Exclusions
1. Open Windows Security.
2. Open **Virus and Threat Protection**.
3. Click **Manage Settings** under **Virus and threat Protection settings**.
4. Scroll down and click **Add or remove exclusions** under **Exclusions**.
5. Add a **Folder** exclusion and point it to the **Installation Location** folder.
  * If you are using a third-party antivirus, you will need to find the exclusions menu and add one to the same folder.

## Root Mods
1. In your **Installation Location**, open the `__root mods` folder.
2. Copy **everything** to the game's **Root** folder (the folder where you installed Fallout 3).
3. Still in the game's Root folder, double-click on **Patcher.exe** to run it.
4. A command prompt should show up, run for a few seconds, then read as follows:

>Patching completed successfully.
>
>Press any key to continue . . .

5. Close the command prompt and a file named **Fallout3_backup.exe** should appear in the game's **Root** folder.

## BSA Decompressor
Decompresses the vanilla BSA files to reduce loading times and stuttering. Can also fix certain sound effects not playing. As of 1.2.0rc1 these are included in the list but if Wabbajack breaks them somehow here are instructions to decompress them.
1. In your **Installation Location**, open the `__bsa decompressor` folder.
2. Run **FO3 BSA Decompressor.exe**
3. The **Fallout 3** and **Decompressed Archives** path should be filled by default (Root and Data folder respectively).

If they aren't, close the program and re-run the game's launcher to generate the required registry key.
  * If you intend to install **Tale of Two Wastelands** or don't want to verify your game files everytime you need to update the list, you can redirect the **Decompressed Archives** path to the folder `\mods\[NoDelete] Decompressed BSAs\` in your **Installation Location**.
4. Click **Decompress**, wait for the process to finish, then exit out of the program once finished.

## Mod Organizer 2 Setup
1. Launch **ModOrganizer.exe** from your **Installation Location**.
2. If you see a pop-up called **Register?**, select **Yes**.
3. If you use the **Steam** version of the game, enable the mod **Yet Another Steam Overlay Fixer** under the **Post Installation** separator.

## Game Settings
There are three profiles you can choose from; the default profile, the Classic profile, and the ModdingLinked Basics profile. As the INI files are profile specific, you must use the drop-down menu on the top of your modlist in MO2 to select the profile you would like to configure settings for.
1. Open the game launcher using the **Fallout Launcher** option in MO2. You may need to add it manually if you have the Steam version of the game by clicking **<Edit...>** from the executables dropdown menu, selecting the + icon and choosing **Add from file...**.
2. Inside the launcher click **Options** and do the following:
    1. Select **Ultra** preset.
* If you have a very weak PC, you can select the **Medium** preset instead.

  2. Set **Resolution** to your monitor's native resolution.
* If you can't find the right resolution in the launcher's list, do the following:
    
    1. Close the launcher.
    2. Click the <img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/refs/heads/main/images/tools%20menu.png" target="_blank"></a> button and select **INI Editor**.
    3. Select the **FalloutPrefs.ini** tab.
    4. Change the following settings in the `[Display]` section:
    * `iSize W` = your screen width
    * `iSize H` = your screen height
    * If you use an Ultrawide display also follow these steps: [Extra Stuff you should know](#extra-stuff-you-should-know)
3. Close the launcher.

## Performance
I recommend capping your FPS to `120` or lower as that is the recommended limit with the High FPS Fix. For a list of recommended FPS limiters and how to set them up, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters)

**DXVK:** Highly recommended, to use it just enable the latest version of **DXVK** under the **Post Installation** separator in MO2. Version 2.0 of DXVK requires a GPU that supports Vulkan 1.3 - here are the minimum required GPUs: 

**AMD**: Radeon RX 400 series or newer (except RX 455 OEM).

**NVIDIA**: GeForce 900 series or newer.

**Intel**: Intel HD 510/530 or newer.

If you have issues with the latest version or your GPU doesn't support Vulkan 1.3 you can try the 1.10.3 version. If you are having issues on an Intel iGPU you can try the 1.10.1 version.
For more information on DXVK and HDR, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#DXVK)

## Launching the Game
1. Make sure the dropdown box on the right is set to `Fallout 3` and press the Run button.
2. You're all set! Everything is already configured by default so you can hop right into a new game!

# Updating the List

1. Add the [NoDelete] prefix to the name any mods you added after installation.
2. **Verify files** on **Steam** or **GOG Galaxy**.
3. Reinstall the list with the "**Overwrite Installation**" checkbox enabled.
4. Rerun the Anniversary Patcher and optionally the BSA Decompressor (unless you installed it to `\mods\[NoDelete] Decompressed BSAs`).

# Extra Stuff you should know
**Ultrawide Support:** 

Enable `bUltrawideSupport` in the mod `Stewie Tweaks Essentials INI`

**Classic Profile:** Same as the default profile but uses Enhanced Night Sky, krzymar HI-RES Moon, and Clarity instead of Enhanced Vanilla Stars, Accurate NASA Stars, HD NASA Moon, Atmospheric Lighting Tweaks, and True Weathers.

**ModdingLinked Basics Profile:** Just the Utilities and Bug Fixes from the FO3 Mod Guide written by ModdingLinked.

# Credits
[Qolore7](https://github.com/Qolore7) for most of the install steps which I grabbed from [Lost Liberty](https://github.com/Qolore7/lost-liberty/tree/main)
