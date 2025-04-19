# How to install `Serverless` with scoop

## Searching
```bash
PS C:\> scoop search serverless
Results from local buckets...

Name       Version Source Binaries
----       ------- ------ --------
serverless 3.39.0  main


PS C:\>
```

## Installation
```bash
PS C:\> scoop install serverless
Updating Scoop...
Updating Buckets...
 * 784caeac0146 trid: Update to version 2.24-25.04.19                    main         3 hours ago
 * a3b762b2bc84 fq: Update to version 0.15.0                             main         3 hours ago
 * 4b393baa6f3e cc65: Update to version 14549760042                      main         3 hours ago
 * 0a0fb5e79978 sing-box@1.11.8: Fix hash (Closes #6741)                 main         6 hours ago
 * 5f558e317850 ungoogled-chromium: Update to version 135.0.7049.95-1.1  extras       3 hours ago
 * 430ea44f459e syncthingtray: Update to version 1.7.6                   extras       3 hours ago
 * f7183d20e71e syncthingctl: Update to version 1.7.6                    extras       3 hours ago
 * 2b30dad31767 qbittorrent-enhanced: Update to version 5.0.5.10         extras       3 hours ago
 * 73929f511722 mpc-hc-fork: Update to version 2.4.2                     extras       3 hours ago
 * 8d066abc7336 gpxsee: Update to version 13.39                          extras       3 hours ago
 * e0f712b0140c chromium: Update to version 135.0.7049.85-r1427262       extras       3 hours ago
 * 98f60220cc61 labplot-nightly: Update to version 8688                  versions     3 hours ago
 * 036cd16ed68c firefox-nightly: Update to version 139.0a1.20250419094.. versions     3 hours ago
 * b4f3dbc64368 ffmpeg-yt-dlp: Update to version 7.1.1-6-20250419        versions     3 hours ago
 * a06348707e41 ffmpeg-shared-nightly: Update to version 119298          versions     3 hours ago
 * 61ef50d36153 ffmpeg-nightly: Update to version 1745070199             versions     3 hours ago
 * 8d5b395c38b9 dolphin-nightly: Update to version 5747                  versions     3 hours ago
 * c0076bce01d2 chromium-nosync: Update to version 135.0.7049.85-r1427.. versions     3 hours ago
 * a003d5925d50 chromium-dev: Update to version 137.0.7135.0-r1449167    versions     3 hours ago
 * bc7cf467f474 ffmpeg-nightly@1744983377: Fix hash (Closes #2258)       versions     4 hours ago
Scoop was updated successfully!
Installing 'serverless' (3.39.0) [64bit] from 'main' bucket
serverless-win-x64.exe (138.3 MB) [===========================================================================] 100%
Checking hash of serverless-win-x64.exe ... ok.
Linking ~\scoop\apps\serverless\current => ~\scoop\apps\serverless\3.39.0
Creating shim for 'serverless'.
'serverless' (3.39.0) was installed successfully!
PS C:\>
```

## Version
```bash
PS C:\> serverless --version
Framework Core: 3.39.0 (standalone)
Plugin: 7.2.3
SDK: 4.5.1

PS C:\>
```

## Note
Can be another install with `npm install -g serverless`
