# Install `HeidiSQL` with scoop

## Searching
```bash
PS C:\> scoop search heidisql
Results from local buckets...

Name     Version Source Binaries
----     ------- ------ --------
heidisql 12.10   extras

PS C:\>
```

## Installation
```bash
PS C:\> scoop install heidisql
Updating Scoop...
Updating Buckets...
 * 83b8e936ba30 swig: Update to version 4.3.1                            main         2 hours ago
 * 9eb5c19c29ff emscripten: Update to version 4.0.7                      main         2 hours ago
 * a66b963c5aee dolt: Update to version 1.51.4                           main         2 hours ago
 * 020f4ccbbfea chromedriver: Update to version 135.0.7049.95            main         2 hours ago
 * a2db48335770 schismtracker: Update to version 20250415                extras       2 hours ago
 * 630251e189cf rimage: Update to version 0.11.0                         extras       2 hours ago
 * 8ad7b0dd56de goofcord: Update to version 1.9.0                        extras       2 hours ago
 * d72ee5365482 gisto: Update to version 2.2.0                           extras       2 hours ago
 * beed2683bd74 firefox-eme-free: Update to version 137.0.2              extras       2 hours ago
 * 84f7560988c9 fiji: Update to version 20250415-1717                    extras       2 hours ago
 * a9e4bbf9184d vim-nightly: Update to version 9.1.1308                  versions     44 minutes ago
 * 06af26df5632 ruffle-nightly: Update to version 2025-04-16             versions     44 minutes ago
 * db868ca59385 rstudio-daily: Update to version 2025.04.0-478           versions     44 minutes ago
 * e7c27787c4b4 okular-nightly: Update to version 6103                   versions     44 minutes ago
 * b3b3ee47a8cb micro-nightly: Update to version nightly-2025-04-16      versions     44 minutes ago
 * 2de9190af80d lapce-nightly: Update to version 1744764398              versions     44 minutes ago
 * 1c5abce32c14 firefox-nightly: Update to version 139.0a1.20250415212.. versions     44 minutes ago
 * 37394806dfc9 dolphin-nightly: Update to version 5704                  versions     44 minutes ago
 * 27de54a40c75 dbeaver-ea: Update to version 25.0.4-2025-04-15          versions     44 minutes ago
 * 16a4f9381c8c cmake-nightly: Update to version 4.0.20250415            versions     44 minutes ago
 * cf2ffce2df90 chromium-dev: Update to version 137.0.7127.0-r1447498    versions     44 minutes ago
 * 7a6f66b524de bottom-nightly: Update to version 14482034571            versions     44 minutes ago
Scoop was updated successfully!
Installing 'heidisql' (12.10) [64bit] from 'extras' bucket
HeidiSQL_12.10_64_Portable.zip (27.5 MB) [=======================] 100%
Checking hash of HeidiSQL_12.10_64_Portable.zip ... ok.
Extracting HeidiSQL_12.10_64_Portable.zip ... done.
Running pre_install script...done.
Linking ~\scoop\apps\heidisql\current => ~\scoop\apps\heidisql\12.10
Creating shim for 'heidisql'.
Making C:\Users\ADMIN\scoop\shims\heidisql.exe a GUI binary.
Creating shortcut for HeidiSQL (heidisql.exe)
Persisting portable_settings.txt
'heidisql' (12.10) was installed successfully!

PS C:\>
```

## Running
```bash
PS C:\> heidisql
```

## Uninstall
```bash
PS C:\> scoop uninstall heidisql
Uninstalling 'heidisql' (12.10).
Removing shim 'heidisql.shim'.
Removing shim 'heidisql.exe'.
Removing shortcut ~\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Scoop Apps\HeidiSQL.lnk
Unlinking ~\scoop\apps\heidisql\current
'heidisql' was uninstalled.
PS C:\>
```
