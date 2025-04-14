# How to install `Microsoft Teams` with scoop

## Searching
```bash
PS C:\> scoop search microsoft-teams
Results from other known buckets...
(add them using 'scoop bucket add <bucket name>')

Name            Source
----            ------
microsoft-teams extras


PS C:\>
```

## Recheck bucket
### List bucket
```bash
PS C:\> scoop bucket list

Name Source                                     Updated              Manifests
---- ------                                     -------              ---------
main https://github.com/ScoopInstaller/Main.git 4/13/2025 3:27:10 AM      1388


PS C:\>
```

### Add bucket
```bash
PS C:\> scoop bucket add extras
Checking repo... OK
The extras bucket was added successfully.
PS C:\>
```

### List bucket again
```bash
PS C:\> scoop bucket list

Name   Source                                     Updated              Manifests
----   ------                                     -------              ---------
main   https://github.com/ScoopInstaller/Main.git 4/13/2025 3:27:10 AM      1388
extras https://github.com/ScoopInstaller/Extras   4/13/2025 3:27:06 AM      2151


PS C:\>
```

## Install
```bash
PS C:\> scoop install extras/microsoft-teams
Installing 'microsoft-teams' (1.8.00.8769) [64bit] from 'extras' bucket
Teams-1.8.00.8769-full.nupkg (157.0 MB) [=========================================================================================] 100%
Checking hash of Teams-1.8.00.8769-full.nupkg ... ok.
Extracting Teams-1.8.00.8769-full.nupkg ... done.
Linking ~\scoop\apps\microsoft-teams\current => ~\scoop\apps\microsoft-teams\1.8.00.8769
Creating shim for 'Teams'.
Making C:\Users\Admin\scoop\shims\teams.exe a GUI binary.
Creating shortcut for Microsoft Teams (Teams.exe)
Running post_install script...done.
'microsoft-teams' (1.8.00.8769) was installed successfully!
PS C:\>
```

***not working ***

## Uninstall
```bash
PS C:\> scoop uninstall microsoft-teams
Uninstalling 'microsoft-teams' (1.8.00.8769).
Removing shim 'Teams.shim'.
Removing shim 'Teams.exe'.
Removing shortcut ~\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Scoop Apps\Microsoft Teams.lnk
Unlinking ~\scoop\apps\microsoft-teams\current
'microsoft-teams' was uninstalled.
PS C:\>
```