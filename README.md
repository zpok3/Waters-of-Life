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
  - [Terminology](#key-terminology)
- [Setup](#setup)
    - [Preparation](#preparation)
    - [Clean Install](#clean-installation)
    - [Starting the Game](#starting-fallout-3)
- [Installation](#installation)
- [Post Installation](#post-installation)
- [Extra Stuff you should know](#extra-stuff-you-should-know)
- [Credits](#credits)

# Introduction
A lightweight vanilla plus Wabbajack mod list for Fallout 3. Intended to bring a Viva New Vegas-like experience to Fallout 3. Well, not quite since the Fallout 3 modding scene is pretty dead. Anyways it's Wabbajack only since I'm just a guy who does this for a hobby so I can't commit to writing a real guide.

# List Contents
You can look [here](https://loadorderlibrary.com/lists/waters-of-life-2) if you're curious about what mods are included.

# Requirements
- A fresh installation of the **English** version of the game with the all of the DLCs from Steam or GOG.
- Only the English version is supported. I understand that this may be frustrating for non-English speaking users, but due to the core file differences between the different versions, only one version can be supported. 
- Approximately 25GB of free space, game included (21GB with all the downloads deleted afterwards).
- Windows 10 or higher (64 bit).
  - [Wabbajack via Proton guide](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-via-Proton) and [my supplementary Linux guide](https://github.com/zpok3/Waters-of-Life/blob/main/Linux-Guide.md) to install Wabbajack lists on Linux available here.

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
- The latest .wabbajack file for this modlist downloaded (you will need to extract it from the archive before you can use it) from either the [releases](https://github.com/zpok3/Waters-of-Life/releases) page or the [Nexus](https://www.nexusmods.com/fallout3/mods/26081) page.
- A [Nexus Mods](https://users.nexusmods.com/register) account (Premium is recommended for uncapped download speeds and fully automated modlist installation).

# Key Terminology
- **Root folder**: The folder that the game is installed in.
  - Example: `C:\GOG Games\Fallout 3`
- **Data folder**: Where all of the game's assets are located.
  - Example: `C:\GOG Games\Fallout 3\Data`
- **Installation location**: The folder where Mod Organizer 2 and all the mods are located.
  - Example: `C:\Modding\Waters of Life`

# Setup:
## Preparation
**Enabling file extensions:**
1. Open File Explorer.
2. Select the **View** tab at the top.
3. Enable **File name extensions** in the **Show** section.

**Disabling Base Address Randomization:**
Base Address Randomization is a security feature in Windows that allows program's starting address to be randomized, which is not the expected behavior in 32-bit programs like Fallout 3. This **leads to crashes** in a modded game. This is disabled by default but it's recommended to make sure it's disabled as a sanity check.
1. Open **Windows Security** from your **Start Menu**.
2. Click on **App and Browser control** in the left sidebar.
3. Click on **Exploit Protection Settings** under **Exploit Protection**.
4. Ensure **Force randomization for images (Mandatory ASLR)** is set to **Use default (Off)**.
-  If you don't want to change the global setting, you can add an exception just for the game:
1. Click on **Program settings**.
2. Click on **Add program to customize**.
3. Select **Add program by name**.
4. Enter `Fallout3.exe` in the box and save.
5. Find the newly created entry on the list and click **Edit**.
6. Find **Force randomization for images (Mandatory ASLR)**.
7. Check **Override system settings**, and set the toggle to **Off**.
## Clean Installation
Waters of Life requires a completely clean installation of Fallout 3. This means completely deleting both the game folder and all INI files located in `Documents\My Games\Fallout3` then reinstalling the game through Steam/GOG. The game MUST be installed outside of any default Windows folders, such as `Program Files (x86)`, `Program Files`, your `Desktop`, or `Documents`. Additionally, it is recommended to install the game on an SSD if possible to improve load times and decrease stuttering.
Example of a safe install location:
`C:\Games`

**Steam:**
- The following instructions are only for anyone who has only one drive in their system along with Steam installed in `Program Files (x86)` as Steam only allows one library folder per drive.
- Skip to step 1 of **Installing the game** if you have Steam installed outside of `Program Files (x86)` or have a secondary drive to install games to.
1. Completely exit out of Steam using Task Manager or System Tray.
2. Download **steam_library_setup_tool-3.2.exe** from [here](https://github.com/LostDragonist/steam-library-setup-tool/releases/download/3.2/steam_library_setup_tool-3.2.exe).
3. Run the file and click **Add Row** to add a new entry.
4. Type the chosen path under **Path**, e.g. `C:\Games\SteamLibrary`.
5. Click **Accept** and then **Yes** if prompted to create a new folder.
6. Click **OK** when the tool asks to exit.
- **Installing the game:**
1. Open Steam and go to your **Library**.
2. Find Fallout 3 in the list and click **Install**.
3. Under **Install to:**, select a library folder of your choice that is outside of any default Windows folders. If you created a custom Steam Library earlier, it will be the second **C:\** entry.
4. Select **Next** and wait for the install to finish.

**GOG:**
1. In GOG Galaxy, go to your **Library**
1. In GOG Galaxy, select **Fallout 3: Game of the Year Edition** and click **Install**.
2. Set the **Install to** folder to a folder of your choice, e.g. `C:\GOG Games`.

## Starting Fallout 3
Start the game and exit once you're at the main menu. This will ensure any settings files needed by Wabbajack are created.

# Installation

1. Create a folder for Wabbajack outside of any default Windows folders.

Example: `C:\Modding\Wabbajack`

2. Place the downloaded Wabbajack.exe in this folder and run it.
3. Select `Install from Disk` in the Wabbajack app. You will have to manually select where you downloaded the .wabbajack file in the `Target Modlist` box.
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
Here we will run the Fallout Anniversary Patcher, its features include a Mod Limit Fix, Intel HD Graphics Bypass, Games for Windows Live Disabler, and specifically for Steam/Epic it applies a 4GB/LAA patch and downgrades the game executable to 1.7.0.3 for mod compatibility.
1. In your **Installation Location**, open the `__root mods` folder.
2. Copy **everything** to the game's **Root** folder (the folder where you installed Fallout 3).
3. Still in the game's Root folder, double-click on **Patcher.exe** to run it.
4. A command prompt should show up, run for a few seconds, then read as follows:

>Patching completed successfully.
>
>Press any key to continue . . .

5. Close the command prompt and a file named **Fallout3_backup.exe** should appear in the game's **Root** folder.

## BSA Decompressor
Decompresses the vanilla BSA files to reduce loading times and stuttering. Increases the size of the game to about 1.64GB if you decompress directly into the **Data** folder, otherwise it takes up about a 3.38GB if it's in a mod folder in the **Installation location**.
1. In your **Installation Location**, open the `__bsa decompressor` folder.
2. Run **FO3 BSA Decompressor.exe**
3. The **Fallout 3** and **Decompressed Archives** path should be filled by default (Root and Data folder respectively).

If they aren't, close the program and re-run the game's launcher to generate the required registry key.
  * If you intend to install **Tale of Two Wastelands** or don't want to verify your game files everytime you need to update the list, you can create a folder called `[NoDelete] Decompressed BSAs` in the `mods` folder located your **Installation Location** and redirect the **Decompressed Archives** path to that folder. Make sure to enable it in the left pane of whatever profile you would like to use once you open Mod Organizer.
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
I recommend capping your FPS to `120` or lower as that is the recommended limit with the High FPS Fix. For instructions on how to set up [Rivatuner Statistics Server (RTSS)](https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/) (if you use MSI Afterburner you probably already have this installed), please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters). It's written for New Vegas but you can very easily apply it to Fallout 3 by replacing the part where you select `FalloutNV.exe` with selecting `Fallout3.exe`.

**DXVK:** Highly recommended, better latency than D3D9 windowed and variable refresh rate works without any problems. and to use it just enable the latest version of **DXVK** under the **Post Installation** separator in MO2. Version 2.0 of DXVK requires a GPU that supports Vulkan 1.3 - here are the minimum required GPUs (source: [TechPowerUp GPU Database](https://www.techpowerup.com/gpu-specs/)): 

**AMD**: Radeon RX 400 series or newer (except RX 455 OEM).

**NVIDIA**: GeForce 900 series or newer.

**Intel**: Intel HD 510/530 or newer.

If you have issues with the latest version or your GPU doesn't support Vulkan 1.3 you can try the 1.10.3 version. If you are having issues on an Intel iGPU you can try the 1.10.1 version.
For more information on DXVK, VRR, HDR, and Alt-Tabbing, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#DXVK). 

## Launching the Game
1. Make sure the dropdown box on the right is set to **Fallout 3** and press the Run button.
- **Q**: Aren't you supposed to use the FOSE loader?
- **A**: The Fallout Anniversary Patcher which we ran earlier enables the game executable to load FOSE automatically if available.
2. You're all set! Everything is already configured by default so you can hop right into a new game!

# Updating the List

1. Add the [NoDelete] prefix to the name any mods you added after installation.
2. **Verify files** on **Steam** or **GOG Galaxy** (only if you output your decompressed BSAs directly into your game's **Data** folder, otherwise skip to step 3).
3. Reinstall the list with the "**Overwrite Installation**" checkbox enabled.
4. Rerun the Anniversary Patcher (unless you skipped step 2) and optionally the BSA Decompressor (unless you installed it to `\mods\[NoDelete] Decompressed BSAs`).

# Extra Stuff you should know
**Ultrawide Support:** 

Enable `bUltrawideSupport` in the mod `Stewie Tweaks Essentials INI`

**Classic Profile:** Same as the default profile but uses Enhanced Night Sky, krzymar HI-RES Moon, and Clarity instead of Enhanced Vanilla Stars, Accurate NASA Stars, HD NASA Moon, Atmospheric Lighting Tweaks, and True Weathers.

**ModdingLinked Basics Profile:** Just the Utilities and Bug Fixes from the FO3 Mod Guide written by ModdingLinked.

# Credits
[Qolore7](https://github.com/Qolore7) for most of the install steps which I grabbed from [Lost Liberty](https://github.com/Qolore7/lost-liberty/tree/main).

[Ungeziefi](https://github.com/Ungeziefi) and [Wall SoGB](https://github.com/WallSoGB) for the resources available at [ModdingLinked](https://moddinglinked.com/index.html).
