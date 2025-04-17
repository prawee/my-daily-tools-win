# How to install `Steam` with scoop

## Searching
```bash
PS C:\> scoop search steam
Results from local buckets...

Name                        Version    Source   Binaries
----                        -------    ------   --------
archisteamfarm              6.1.4.3    extras
bulk-crap-uninstaller       5.8.3      extras   SteamHelper.exe
steam-desktop-authenticator 1.0.15     extras
steam-library-manager       1.7.2.0    extras
steamcmd                    1743712175 extras
steamguard-cli              0.17.0     extras
steam-mover                 0.1        versions
steam                       nightly    versions


PS C:\>
```

## Installation
```bash
PS C:\> scoop install steam
Updating Scoop...
Updating Buckets...
INFO  Converting 'main' bucket to git repo...
The main bucket was removed successfully.
Checking repo... OK
The main bucket was added successfully.
 * 867f1a29c9d6 onlyoffice-desktopeditors: Update to version 8.3.3       extras       3 hours ago
 * ac403cad9799 multicommander: Update to version 15.4.0.3088            extras       3 hours ago
 * 46a5f8664791 httptoolkit: Update to version 1.20.1                    extras       3 hours ago
 * 08e811538572 freeplane: Update to version 1.12.10                     extras       3 hours ago
 * ee9ed5c93789 cascadeur: Update to version 2025.1.1.92                 extras       3 hours ago
 * 42137fe0a9d9 cheat-engine: Update to version 7.6 (#15310)             extras       6 hours ago
 * ea7fa281ed76 xan: Update to version 0.49.1                            extras       7 hours ago
 * efa02d504b59 uninstalr: Update to version 2.8                         extras       7 hours ago
 * ea6006da0f9a postman: Update to version 11.41.4                       extras       7 hours ago
 * f536976a7c56 opera-gx: Update to version 118.0.5461.50                extras       7 hours ago
 * a1bb9c0ccf97 open-tv: Update to version 1.6.1                         extras       7 hours ago
 * 77c73efab70f jackett: Update to version 0.22.1788                     extras       7 hours ago
 * 3a353439c18a appflowy: Update to version 0.8.9                        extras       7 hours ago
 * e05802d7a687 obs-studio: Update to version 31.0.3 (#15300)            extras       10 hours ago
 * d5db7db8d375 zed: Update to version 0.182.9                           extras       11 hours ago
 * b5e48fc6a578 zed-opengl: Update to version 0.182.9                    extras       11 hours ago
 * 8d4ced8f3e7f yuescript: Update to version 0.27.5                      extras       11 hours ago
 * d6adb1970674 msbuild-structured-log-viewer: Update to version 2.2.474 extras       11 hours ago
 * 187bc1b47747 diskgenius: Update to version 6.0.0.1631                 extras       11 hours ago
 * edca37eb3f04 boinc: Update to version 8.2.1                           extras       11 hours ago
 * 69c6e3555848 vscodium: Update to version 1.99.32562                   extras       15 hours ago
 * 59972e77ce9f mpv-git: Update to version 20250416                      extras       15 hours ago
 * 1e96438408fe hydrus-network: Update to version 618                    extras       15 hours ago
 * d703242ffcf4 beyondcompare: Update to version 5.0.7.30840             extras       15 hours ago
 * a68293c2b4f9 codesnap: Update to version 0.10.8, update gh url, fix.. extras       15 hours ago
 * dc63b03ff095 odict: Update to version 2.4.0, fix checkver             extras       16 hours ago
 * c092ba917149 quickcpu: Update to version 5.0.9.0, fix checkver & au.. extras       17 hours ago
 * bbe807b0344a structurizr-cli: Update to version 2025.03.28, fix aut.. extras       17 hours ago
 * d06207016330 ffmpeg-nightly@1744894643: Fix hash (Closes #2255)       versions     4 minutes ago
 * 3f0df3c57a55 zig-dev: Update to version 0.15.0-dev.369                versions     3 hours ago
 * 5321bf8bc935 vim-tux: Update to version 9.1.1313_20250417             versions     3 hours ago
 * 012a80376e6c qbittorrent-nightly: Update to version 14513292969       versions     3 hours ago
 * b494907c6de5 neochat-nightly: Update to version 11711                 versions     3 hours ago
 * ab666a8a14cd ipfilter-nightly: Update to version 1744866497           versions     3 hours ago
 * 360cc275a49d firefox-nightly: Update to version 139.0a1.20250417041.. versions     3 hours ago
 * 60249be1cefe ffmpeg-shared-nightly: Update to version 119294          versions     3 hours ago
 * 1df69f2769ad ffmpeg-nightly: Update to version 1744894643             versions     3 hours ago
 * e2d23dd05a86 ffmpeg-gyan-nightly: Update to version 2025-04-17        versions     3 hours ago
 * fd893b5873c9 edgedriver-canary: Update to version 137.0.3265.0        versions     3 hours ago
 * 5f86ba169d29 dolphin-nightly: Update to version 5729                  versions     3 hours ago
 * 563eba97a4e2 chromium-dev: Update to version 137.0.7130.0-r1448242    versions     3 hours ago
 * dc526bb138bc vscode-insiders: Update to version 1.100.0-1744866412472 versions     7 hours ago
 * 7341e9530946 r-patched: Update to version 4.5.0-r88149                versions     7 hours ago
 * 2918070de2c5 nodejs-nightly: Update to version 24.0.0-nightly202504.. versions     7 hours ago
 * e010ff23ea02 neovim-nightly: Update to version 0.12.0-157             versions     7 hours ago
 * 21de82c6bc9a kicad-nightly: Update to version 9.99.0.904.g194ee9ef25  versions     7 hours ago
 * 023690fff3bf kicad-lite-nightly: Update to version 9.99.0.904.g194e.. versions     7 hours ago
 * 367dc166bf40 googlechrome-canary: Update to version 137.0.7128.0      versions     7 hours ago
 * 797c61814223 googlechrome-beta: Update to version 136.0.7103.33       versions     7 hours ago
 * cc82f48b88d9 edgedriver-canary: Update to version 137.0.3262.0        versions     7 hours ago
 * 2c8d92f11083 dart-dev: Update to version 3.9.0-23.0.dev               versions     7 hours ago
 * 33830589dfdd chromium-dev: Update to version 137.0.7130.0-r1448162    versions     7 hours ago
 * f4e8fe764c72 brave-beta: Update to version 1.78.84                    versions     7 hours ago
 * aaf7003bedf1 zed-opengl-nightly: Update to version 2025-04-17         versions     11 hours ago
 * 00babba186ed zed-nightly: Update to version 2025-04-17                versions     11 hours ago
 * 6c23364a390e vlc-nightly: Update to version 20250417                  versions     11 hours ago
 * c280fad21190 vlc-nightly-ucrt-llvm: Update to version 20250417        versions     11 hours ago
 * dd3a6f3e31a2 oss-cad-suite-nightly: Update to version 2025-04-17      versions     11 hours ago
 * 81a43efe3765 gitbutler-nightly: Update to version 0.5.1167            versions     11 hours ago
 * a32eb9e048b9 edgedriver-canary: Update to version 137.0.3263.0        versions     11 hours ago
 * 048c2a9d5ca0 chromium-dev: Update to version 137.0.7129.0-r1448124    versions     11 hours ago
 * 7cc5e8c1b3e0 brave-nightly: Update to version 1.79.71                 versions     11 hours ago
 * 3ef691c65b09 vim-nightly: Update to version 9.1.1313                  versions     13 hours ago
 * ff8e90bea56d ruffle-nightly: Update to version 2025-04-17             versions     13 hours ago
 * e153f4fa6413 rstudio-daily: Update to version 2025.04.0-483           versions     13 hours ago
 * 20ad05ea5b4c okular-nightly: Update to version 6107                   versions     13 hours ago
 * 1c2fe090b4d6 micro-nightly: Update to version nightly-2025-04-17      versions     13 hours ago
 * edf6fa0208fb firefox-nightly: Update to version 139.0a1.20250416214.. versions     13 hours ago
 * 8ffd70aa9366 edgedriver-canary: Update to version 137.0.3264.0        versions     13 hours ago
 * fbd445667dae cmake-nightly: Update to version 4.0.20250416            versions     13 hours ago
 * f9813d77c1e7 chromium-dev: Update to version 137.0.7129.0-r1448112    versions     13 hours ago
 * 5f4b2216d9ea chromedriver-canary: Update to version 137.0.7128.0      versions     13 hours ago
 * 6aee5a302862 bottom-nightly: Update to version 14505333729            versions     13 hours ago
Scoop was updated successfully!
WARN  This is a nightly version. Downloaded files won't be verified.
Installing 'steam' (nightly-20250417) [64bit] from 'versions' bucket
SteamSetup.exe (2.3 MB) [===============================================================================================================================] 100%
Extracting SteamSetup.exe ... done.
Running pre_install script...done.
Linking ~\scoop\apps\steam\current => ~\scoop\apps\steam\nightly-20250417
Creating shim for 'Steam'.
Making C:\Users\prawe\scoop\shims\steam.exe a GUI binary.
Creating shortcut for Steam (Steam.exe)
Persisting skins
Persisting steamapps
Persisting userdata
'steam' (nightly-20250417) was installed successfully!
Notes
-----
Changing Steam library folder is HIGHLY recommended.
PS C:\>
```

## Running
```bash
PS C:\> steam
PS C:\>
```
