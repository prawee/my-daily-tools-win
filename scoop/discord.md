# How to install `Discord` with scoop

## Searching
```bash
PS C:\> scoop search discord
Results from local buckets...

Name                  Version     Source   Binaries
----                  -------     ------   --------
discord-rpc-extension 0.3.0       extras
discord               1.0.9188-21 extras
discordchatexporter   2.44.2      extras
discord-canary        0.0.316     versions
discord-ptb           1.0.1059-25 versions


PS C:\>
```

## Installation
```bash
PS C:\> scoop install discord
WARN  Purging previous failed installation of discord.
ERROR 'discord' isn't installed correctly.
Removing older version (1.0.9188-21).
'discord' was uninstalled.
Installing 'discord' (1.0.9188-21) [64bit] from 'extras' bucket
discord-portable-win64-1.0.9188-21.7z (78.1 MB) [=======================================================================================================] 100%
Checking hash of discord-portable-win64-1.0.9188-21.7z ... ok.
Extracting discord-portable-win64-1.0.9188-21.7z ... done.
Linking ~\scoop\apps\discord\current => ~\scoop\apps\discord\1.0.9188-21
Creating shortcut for Discord (discord-portable.exe)
Persisting data
Persisting log
'discord' (1.0.9188-21) was installed successfully!
PS C:\>
```
