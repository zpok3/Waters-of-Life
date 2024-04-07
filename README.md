<img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/main/logo.jpeg" target="_blank"></a>

---
# Waters-of-Life
A vanilla plus Wabbajack mod list for Fallout 3

---

<p align="center">
  <a href="https://www.nexusmods.com/fallout3/mods/26081">Nexus Page</a> ·
  <a href="README.md">Installation</a> ·

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
3. Launch the Wabbajack app and select `Browse Modlists`
4. Make sure `Show Unofficial Lists` is checked and search for `Waters of Life`
5. Select the **Download** icon in the bottom right, then select he **Play** icon once the download is finished
7. In the **Modlist Installation Location** box, select the `Waters of Life` folder you created in the first step
  * The Resource Download Location box should automatically fill in `Waters of Life\Downloads`, but you can move this folder to a different drive if are low on space
8. Click the Go/Begin button and wait for Wabbajack to finish

# Post Installation and Startup

1. Open the installation folder and double click on the program called `ModOrganizer.exe`.
2. Select the **Fallout 3 Launcher** option from the drop-down in the top left then select **Run**
  > If you have the GOG version of the game, you may need to add the launcher to MO2 yourself. You can do so by clicking the **Executables Menu** icon (the two colored gears) in the top bar of MO2, selecting the **+** then **Add from file...**
3. The launcher should run and there should be two pop-ups about detecting your hardware and applying settings
4. Select **Options** then select whichever preset you think is best for your PC. I recommend **Ultra** for most PCs, but the **High** preset will provide noticeably better performance for only a minor visual downgrade.
  > For even further performance gains, I highly recommend disabling shadows. Fallout 3 does not have real-time shadows like modern games, only shadows for actors. These are hardly noticeable in most cases but do have an    impact on performance
5. Set the Resolution option to your preference (The launcher usually does not set it to your monitor's max resolution)
6. Exit out of the launcher
7. Back in MO2, right-click on the mod in the left pane called `Fallout Anniversary Patcher` and select **Open in Explorer**
8. Inside the opened folder, move all of the files to the game's `Root` folder (i.e. where you installed Fallout 3)
9. Once the file has been moved, double-click `Patcher.exe` to run the patcher 
9. A command prompt should show up, run for a few seconds, then read as follows:

>Patching completed successfully.
>
>Press any key to continue . . .

10. Exit out of the command prompt
11. DXVK: Version 2.3 of DXVK requires a GPU that supports Vulkan 1.3 - for information on which version to choose, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#DXVK) - this is **Required** if you have an AMD GPU.
12. Fallout 3 Heap Replacer: In MO2, right click on `Fallout 3 Heap Replacer` under the left pane and select **Open in Explorer**
13. Open the F3HR folder and double click on `cpu_info.exe`
14. A command prompt will open and should read:

>=> Use AVX2 <=
>
>Press any key to continue . . .

11. Make sure the dropdown box on the right is set to `Fallout 3` and press the Run button.
12. You're all set! Everything is already configured by default so you can hop right into a new game!
