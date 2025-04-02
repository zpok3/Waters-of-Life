# GOG Guide
Use [this](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-on-Linux-via-Wine) guide. Then add the prefix to Lutris so you can launch the game with GE-Proton after you get it and the modlist installed. And you can write a simple bash script that handles launching Wabbajack for you after you've finished setting up the Wine prefix through CLI.

# Steam Guide
Use [this](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-via-Proton) guide for Steam games. You need [SteamTinkerLaunch](https://github.com/sonic2kk/steamtinkerlaunch?tab=readme-ov-file#how-do-i-install-it) installed. Set Fallout 3's compatibilty tool to SteamTinkerLaunch and click play. Select **MAIN MENU** when the SteamTinkerLaunch window opens. Select **GAME MENU** and add a custom command to run the `ModOrganizer.exe` of the installed mod list. Make sure **Only custom command** is enabled so that the launcher doesn't open once you close the game and MO2. Then scroll down and set **Proton version** to Proton Experimental or latest GE-Proton. Next you will need to use the terminal for these next steps:

You will also need to enable visiblity of dotfiles (if you have the base game instead of GOTY the app id is 22300 instead of 22370):
```
protontricks --no-bwrap -c 'WINEDEBUG=-all wine reg add "HKEY_CURRENT_USER\Software\Wine" /v ShowDotFiles /d Y /f' 22370
```
And some Proton components to ensure everything works with the base game and mods. Things like xact/xact_x64 to fix some audio issues, d3d additions for the use of some graphical functions as well as vcrun2022 (Microsoft Visual C++ Redistributable 2022) for some of the included mods (if you have the base game instead of GOTY the app id is 22300 instead of 22370):
```
protontricks --no-bwrap 22370 -q xact xact_x64 d3dcompiler_47 d3dx11_43 d3dcompiler_43 vcrun2022 fontsmooth=rgb
```
