# Introduction
So recently I was trying to get Wabbajack running on Linux, specifically for GOG games. I came across [this](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-on-Linux-via-Wine) guide and I tried to get it running with Lutris since I use it to manage my Wine prefixes for my games. I installed Edge Webview2 into the prefix where my game was installed, set default application settings in the prefix to mimic Windows 7 and set it to mimic Windows 10 for Wabbajack.exe as instructed and sadly it didn't work. I could open Wabbajack and reach the Nexus login page, but everything was black and I was unable to log in. So I wrote this as an unofficial addon to their Proton guide with steps to get GOG games working. How? By installing the game into the prefix where Steam runs Wabbajack. That way, Wabbajack will see your installed game and not throw an error about not being able to find the game. Maybe I'm just stupid but idk. Tested only on OpenSUSE Tumbleweed but it should work on other popular distros.

# Requirements
- Offline GOG installer for whatever game you want to install
- Latest VC++ Redists downloaded from [here](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/) to account for any script extender mods/plugins that may need them. Extract them somewhere for use later when we have the prefix ready.
- Steam
- Lutris
- Proton Experimental or [Latest GE-Proton](https://github.com/GloriousEggroll/proton-ge-custom)
- [ProtonUp-Qt](https://flathub.org/apps/net.davidotek.pupgui2) (optional, only if you want an easy way to install and manage compatibility tools for Steam/Lutris).
- Protontricks

# Installation
First, follow [this](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-via-Proton) guide to get Wabbajack running under Proton on your system.

1. Run Protontricks, and select **Non-Steam shortcut: Wabbajack**.

2. Select the option **Select the default wineprefix** and click OK.

3. Select the option **Run an arbitrary executable (.exe/.msi/.ms)** and click OK.

4. Navigate to the location where your GOG offline installer is located and run it.

4. Install to the default location (should be `C:\GOG Games\gametitle`).

5. Click exit once the installer is finished.

6. Don't close Protontricks yet as we still need it.

# Configuring Lutris
1. In Protontricks select **Browse files** and click OK (you can close Protontricks now).

2. Right click the path and select **Copy**.

3. Open Lutris and click the Add Game (+) button in the top left corner.

4. Choose **Add locally installed game**.

5. Configure as follows:

- **Game info**
    - **Name**: Title of the game as listed on [Lutris](https://lutris.net/) if you want the cover art, banner, and icons to be downloaded and applied automatically.
    - **Runner**: Wine (Runs Windows games).

- **Game options**
    - **Executable**: Paste the path you copied in step 5 into the box, click the button with the three dots on it and navigate to the game's launcher (should be located in `/drive_c/GOG Games/gametitle/`if you followed this guide exactly).
    - **Wine prefix**: Paste the path you copied in step 2 into the box.

- **Runner options**
    - **Wine version**: Proton Experimental or Latest GE-Proton.

6. Select **Save**.

7. Click Play, set resolution and graphics preset and exit launcher.

8. Click the wine button next to the Play button, choose **Run EXE inside Wine prefix**, and select **install_all.bat** from the VC++ Redist AIO package you downloaded earlier.

9. Open Steam, run Wabbajack, and install whatever list you want.

10. Return to Lutris, right click on the game you added earlier, select **Configure**, and under **Game options**, set the executable to the **ModOrganizer.exe** of the Wabbajack list you installed.

# Finish
You can now continue with any post installation steps the Wabbajack list you installed may have mentioned that involve either MO2 or the game. And you're done!

# Steam Guide
For Steam games you need [SteamTinkerLaunch](https://github.com/sonic2kk/steamtinkerlaunch?tab=readme-ov-file#how-do-i-install-it) installed. Set Fallout 3's compatibilty tool to SteamTinkerLaunch and click play. Select **MAIN MENU** when the SteamTinkerLaunch window opens. Select **GAME MENU** and add a custom command to run the `ModOrganizer.exe` of the installed mod list. Make sure **Only custom command** is enabled so that the launcher doesn't open once you close the game and MO2. Then scroll down and set **Proton version** to Proton Experimental or latest GE-Proton. Next you will need to use the terminal for these next steps:

You will also need to enable visiblity of dotfiles (if you have the base game instead of GOTY the app id is 22300 instead of 22370):
```
protontricks --no-bwrap -c 'WINEDEBUG=-all wine reg add "HKEY_CURRENT_USER\Software\Wine" /v ShowDotFiles /d Y /f' 22370
```
And some Proton components to ensure everything works with the base game and mods. Things like xact/xact_x64 to fix some audio issues, d3d additions for the use of some graphical functions as well as vcrun2022 (Microsoft Visual C++ Redistributable 2022) for some of the included mods (if you have the base game instead of GOTY the app id is 22300 instead of 22370):
```
protontricks --no-bwrap 22370 -q xact xact_x64 d3dcompiler_47 d3dx11_43 d3dcompiler_43 vcrun2022 fontsmooth=rgb
```
