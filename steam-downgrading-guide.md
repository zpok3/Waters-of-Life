# Downgrading Fallout 3: Game of the Year Edition
If you use the Steam version of the game and it doesn't start through MO2, it may be related to the [updated launcher](https://store.steampowered.com/news/app/22370/view/4160842270244401930?l=english). Here's a guide on using both the Steam console and [DepotDownloader](https://github.com/SteamRE/DepotDownloader) to downgrade the game. Steps are provided for both the base game and the Game of the Year edition.

## Steam Console
1. Press `Win + R` and enter this command:
```
steam://open/console
```
> [!tip]
> Alternatively you can enter this into the address bar of your web browser.

2. In the console enter one of these commands:

For the original 1.7.0.4 update for GOTY released on October 12, 2021:
```
download_depot 22370 22371 4929549459338680299
```

For the 1.7.0.3 update for GOTY:
```
download_depot 22370 22371 6752416544246981300
```

For the original 1.7.0.4 update for the base game released on October 12, 2021:
```
download_depot 22300 22301 7414504515121985658
```

For the 1.7.0.3 update for the base game:
```
download_depot 22300 22301 3579248769415824205
```

3. The console should print where the files have been downloaded to.

## DepotDownloader
1. Download the latest [DepotDownloader-framework.zip](https://github.com/SteamRE/DepotDownloader/releases/latest) and if you don't already have it, install the latest [Microsoft .NET SDK 9.0](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).

2. Extract the contents of `DepotDownloader-framework.zip` somewhere easily accessible.

3. In the folder you extracted it to, right click and select `Open in Terminal` (you need [Windows Terminal](https://aka.ms/terminal) for this option to be available).

4. Now you can run one of these commands (replace `<username>` with your username):

For the original 1.7.0.4 update for GOTY released on October 12, 2021:
```
dotnet DepotDownloader.dll -app 22370 -depot 22371 -manifest 4929549459338680299 -username <username>
```

For the 1.7.0.3 update for GOTY:
```
dotnet DepotDownloader.dll -app 22370 -depot 22371 -manifest 6752416544246981300 -username <username>
```

For the original 1.7.0.4 update for the base game released on October 12, 2021:
```
dotnet DepotDownloader.dll -app 22300 -depot 22301 -manifest 7414504515121985658 -username <username>
```

For the 1.7.0.3 update for the base game:
```
dotnet DepotDownloader.dll -app 22300 -depot 22301 -manifest 3579248769415824205 -username <username>
```

> [!tip]
> You can add `-dir` to specify where you want to download the files. If you don't, the files will be downloaded to wherever you're running DepotDownloader from.
> 
> You can add `-qr` to show a QR code to scan with the Steam app on your phone instead of entering your password.
>
> If you have it setup, you can add `-no-mobile` if you would like to manually enter your 2FA code instead of approving access within the Steam mobile app.

5. Now you will need to enter your password, and depending on your security settings you may also need to enter a single use code sent via email or approve access within the Steam mobile app.

## Installing the downloaded files
1. From wherever the files have been downloaded, move them into the root folder of the game and overwrite when prompted.
2. If you've already installed the list and attempted to run the game, you'll need to rerun the Anniversary Patcher.
3. If you've manually added the launcher to MO2, you'll need to switch MO2 to use `Fallout3Launcher.exe` instead of `FalloutLauncherSteam.exe`.
4. If you've already attempted to run the game through MO2, you'll need to clear RootBuilder's root folder backup and hash cache by deleting whatever's in `plugins\data\RootBuilder` located wherever you installed the modlist to.

## Finish
You should now be ready to run the game, which hopefully will start up without any issues.
