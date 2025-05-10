# Downgrading Fallout 3: Game of the Year Edition
I currently suspect that the updated launcher included in the Steam version of the game is the cause of issues that people keep running into. Here's a guide on using both the Steam console and [DepotDownloader](https://github.com/SteamRE/DepotDownloader) to downgrade the game.

## Steam Console
1. Press `Win + R` and enter this command:
```
steam://open/console
```
> [!tip]
> Alternatively you can enter this into the address bar of your web browser.

2. In the console enter one of these commands:

For the original 1.7.0.4 update released on October 12, 2021:
```
download_depot 22370 22371 4929549459338680299
```

For the 1.7.0.3 update:
```
download_depot 22370 22371 6752416544246981300
```

3. The console should print where the files have been downloaded to.

## DepotDownloader
1. Download the latest [DepotDownloader-framework.zip](https://github.com/SteamRE/DepotDownloader/releases/latest) and if you don't already have it, install the latest [Microsoft .NET SDK 9.0](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).

2. Extract the contents of `DepotDownloader-framework.zip` somewhere easily accessible.

3. In the folder you extracted it to, right click and select `Open in Terminal` (you need [Windows Terminal](https://aka.ms/terminal) for this option to be available).

4. Now you can run one of these commands (replace `<username>` with your username):

For the original 1.7.0.4 update released on October 12, 2021:
```
dotnet DepotDownloader.dll -app 22370 -depot 22371 -manifest 4929549459338680299 -username <username>
```

For the 1.7.0.3 update:
```
dotnet DepotDownloader.dll -app 22370 -depot 22371 -manifest 6752416544246981300 -username <username>
```

> [!tip]
> You can add `-dir` to specify where you want to download the files. If you don't, the files will be downloaded to wherever you're running DepotDownloader from.
> 
> You can add `-qr` to show a QR code to scan with the Steam app on your phone instead of entering your password.
>
> If you have it setup, you can add `-no-mobile` if you would like to manually enter your 2FA code instead of approving access within the Steam mobile app.

5. Now you will need to enter your password, and depending on your security settings you may also need to enter a single use code sent via email or approve access within the Steam mobile app.

## Installing the downloaded files
Simply move the downloaded files into the root folder of the game and overwrite when prompted. If you've already installed the list and attempted to run the game, you'll need to rerun the Anniversary Patcher and switch MO2 to use `Fallout3Launcher.exe` instead of `FalloutLauncherSteam.exe`. Next, clear RootBuilder's root folder backup and hash cache by deleting whatever's in `plugins\data\RootBuilder` located wherever you installed the modlist to.
