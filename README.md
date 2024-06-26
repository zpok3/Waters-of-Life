<img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/main/logo.jpeg" target="_blank"></a>

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
    - [Downloading and Installing](#downloading-and-installing)
- [Post Installation and Startup](#post-installation-and-startup)
- [Extra Stuff you should know](#extra-stuff-you-should-know)
- [Credits](#credits)

# Introduction
A lightweight vanilla plus Wabbajack mod list for Fallout 3. Waters of Life aims to create a more difficult gameplay experience, along with improving visuals without totally abandoning the vanilla aesthetic.

# List Contents
You can look [here](https://loadorderlibrary.com/lists/waters-of-life-1) if you're curious about what mods are included.

  # Requirements
  - An fresh installation of the **English** version of the game with the all of the DLCs from Steam or GOG
  * Only the English version is supported. I understand that this may be frustrating for non-English speaking users, but due to the core file differences between the different versions, only one version can be supported. 
  * The game MUST be installed outside of any default Windows folders, such as `Program Files`, your `Desktop`, or `Documents`. If you have your Steam library in any of these locations, please follow [these](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) instructions to move it.

- [Microsoft Visual C++ Redistributable Package](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)

- The latest release of [Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) installed outside of any default Windows folders.

# Installation:

## Clean Installation
Waters of Life requires a completely clean installation of Fallout 3. This means completely deleting both the game folder and also the folder located in `Documents\My Games\Fallout3` then reinstalling the game through Steam/GOG. The game MUST be installed outside of any default Windows folders, such as `Program Files`, your `Desktop`, or `Documents`. If you have your Steam library in any of these locations, please follow [these](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) instructions to move it.

## Starting Fallout 3
Start the game and exit once you're at the main menu. This will ensure any settings files needed by Wabbajack are created.

## Downloading and Installing

1. Create a folder for the modist outside of any default Windows folders called **Waters of Life** (I recommend `C:\Games\Waters of Life`) 
2. Launch the Wabbajack app and select `Browse Modlists` (Alternatively use [this](https://github.com/zpok3/Waters-of-Life/releases) link to download the wabbajack file and use `Install from Disk` in the Wabbajack app. You will have to manually select where you downloaded the wabbajack file in the `Target Modlist` box - skip to step 5 if you choose this option)
3. Make sure `Show Unofficial Lists` is checked and search for `Waters of Life`
4. Select the **Download** icon in the bottom right, then select he **Play** icon once the download is finished
5. In the **Modlist Installation Location** box, select the `Waters of Life` folder you created in the first step
  * The Resource Download Location box should automatically fill in `Waters of Life\Downloads`, but you can move this folder to a different drive if are low on space
6. Click the Go/Begin button and wait for Wabbajack to finish

# Post Installation and Startup

1. Open the installation folder and double click on the program called `ModOrganizer.exe`.
2. After running `ModOrganizer.exe` from the modlist installation directory, you will get an error regarding MO2 being unable to open instance 'Portable', select OK and select `Fallout 3` from the list of games.
3. You can change the theme in MO2's settings if you don't want to be flashbanged everytime you open MO2 - I recommend 1809 Dark Mode or vs15 Dark. Select 
<img src= "https://raw.githubusercontent.com/ModdingLinked/Viva-New-Vegas/master/img/mo2%20settings.webp" target="_blank"></a>
and go to the Themes tab if you'd like to do this.
4. Select the **Fallout 3 Launcher** option from the drop-down in the top left then select **Run**
  > If you have the GOG version of the game, you may need to add the launcher to MO2 yourself. You can do so by clicking the **Executables Menu** icon (the two colored gears) in the top bar of MO2, selecting the **+** then **Add from file...**
5. The launcher should run and there should be two pop-ups about detecting your hardware and applying settings
6. Select **Options** then select whichever preset you think is best for your PC. I recommend **Ultra** for most PCs, but the **High** preset will provide noticeably better performance for only a minor visual downgrade.
  > For even further performance gains, I highly recommend disabling shadows. Fallout 3 does not have real-time shadows like modern games, only shadows for actors. These are hardly noticeable in most cases but do have an    impact on performance
7. Set the Resolution option to your preference (The launcher usually does not set it to your monitor's max resolution)
8. Exit out of the launcher
9. Back in MO2, right-click on the mod in the left pane called `Fallout Anniversary Patcher` and select **Open in Explorer**
10. Inside the opened folder, move all of the files to the game's `Root` folder (i.e. where you installed Fallout 3)
11. Once the file has been moved, double-click `Patcher.exe` to run the patcher 
12. A command prompt should show up, run for a few seconds, then read as follows:

>Patching completed successfully.
>
>Press any key to continue . . .

11. Exit out of the command prompt
12. **FPS Limiters:** I recommend capping your FPS to `60` or if you want to be really safe, limit to `50`. For a list of recommended FPS limiters and how to set them up, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters)
13. If you would like to play at above 60 FPS, install [Fallout Stutter Remover](https://www.nexusmods.com/fallout3/mods/8886) and [this ini preset](https://github.com/zpok3/Waters-of-Life/releases/download/v.1.0/fsr.high.fps.preset.7z) for it
14. By default `fMaximumFPS` is set to 144, you can run a benchmark in Point Lookout or something to find where you should set this to
15. **DXVK:** Version 2.3 of DXVK requires a GPU that supports Vulkan 1.3 - you can look up your GPU on the [TechPowerUp GPU Database](https://www.techpowerup.com/gpu-specs) to check. For information on DXVK, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#DXVK) - this is **Required** if you have an AMD GPU. OneTweak is already enabled and the game is set to windowed in `FalloutCustom.ini` so all you have to do is enable DXVK in the left pane of MO2 once you've figured out which version is best for you.
16. Make sure the dropdown box on the right is set to `Fallout 3` and press the Run button.
17. You're all set! Everything is already configured by default so you can hop right into a new game!

## Optional Steps

**BSA Decompressor:** Decompresses the Fallout 3 BSAs to reduce load times and stuttering.
1. In MO2, right click on `FO3 BSA Decompressor` under the left pane and select **Open in Explorer**
2. Open the `FO3 BSA Decompressor` folder and double click on `FO3 BSA Decompressor.exe`
3. The path to Fallout 3 installation should automatically fill, if it doesn't just select `Browse` and navigate to where you installed Fallout 3
4. Make sure any applications that can keep BSA archives open like MO2 are closed before clicking `Decompress`
5. Select `Exit` once decompression has completed

**Fallout 3 Heap Replacer:** In MO2, right click on `Fallout 3 Heap Replacer` under the left pane and select **Open in Explorer**
1. Open the F3HR folder and double click on `cpu_info.exe`
2. A command prompt will open and should read (it doesn't have to say AVX2, but most Intel CPUs from 2013 or later and AMD CPUs from 2017 or later should support it. Just pick whatever it tells you to use):

>=> Use AVX2 <=
>
>Press any key to continue . . .

3. Back in MO2, double click on `Fallout 3 Heap Replacer` and select the `Filetree` tab
4. Expand the `F3HR` folder and the `AVX2` folder (or whatever the cpu info told you to use)
5. Drag the `d3dx9_38.dll` into the `root` folder that contains `d3dx9_38.tmp` and enable the mod in the left pane of MO2

# Updating the List

1. Download the latest version of the Wabbajack list from the [Releases](https://github.com/zpok3/Waters-of-Life/releases) page.

2. In the Wabbajack app, select `Install From Disk`

3. In the `Target Modlist` box, navigate to the location you downloaded `Waters.of.Life.wabbajack` to.

4. Tick the `Overwrite Installation` box underneath the start button.

5. Make sure the contents of the `Mod List Installation Location` box match where you originally installed the modlist before clicking the start button.

# Extra Stuff you should know
**Ultrawide Support:** In `FalloutCustom.ini` under `[Display]` add the lines:

`iSize W=Your Horizontal Resolution` 

and 

`iSize H=Your Vertical Resolution`

Change the numbers to your screen resolution and enable `bUltrawideSupport` in the mod `Stewie Tweaks Essentials INI`

**Alt-tab in Fullscreen Exclusive:** You will need to set `bFull Screen` to `1` in `FalloutCustom.ini` and use one of the **DXVK** versions under the `Post Installation` separator in MO2. Alternatively if you cannot use DXVK and want the best performance in D3D9, you can disable `bDontMirrorTexturesInRAM` in the mod `Stewie Tweaks Essentials INI`

**Enhanced Night Sky:** A classic alternative to Accurate NASA Stars. You can find it under the `Visuals` separator in MO2. Enable it and disable Accurate Night Sky if you want.

# Credits
[Qolore7](https://github.com/Qolore7) for most of the install steps which I grabbed from [Lost Liberty](https://github.com/Qolore7/lost-liberty/tree/main)
