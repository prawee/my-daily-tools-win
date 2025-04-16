# How to install `Oh My Posh` with scoop

## Searching
```bash
PS C:\> scoop search oh-my-posh
Results from local buckets...

Name       Version Source Binaries
----       ------- ------ --------
oh-my-posh 25.13.0 main


PS C:\>
```

## Installation
```bash
PS C:\> scoop install main/oh-my-posh
Updating Scoop...
WARN  Uncommitted changes detected. Update aborted.
Updating Buckets...
 * d0fb25f2de7b weasyprint: Update to version 65.1                       main         54 minutes ago
 * cf2528aa27e0 pnpm: Update to version 10.8.1                           main         54 minutes ago
 * 108e464d8909 meilisearch: Update to version 1.14.0                    main         54 minutes ago
 * ee4eaf612e06 mediamtx: Update to version 1.12.0                       main         54 minutes ago
 * 96afebdba456 flyway: Update to version 11.7.1                         main         54 minutes ago
 * 8be75ea42e0e cwrsync: Update to version 6.4.2                         main         54 minutes ago
 * 7a1428efa7b8 clink: Update to version 1.7.16                          main         54 minutes ago
 * 132e23067602 stirling-pdf: Update to version 0.45.5                   extras       54 minutes ago
 * 5554b28fb859 q-dir: Update to version 12.17                           extras       54 minutes ago
 * f1338fa937cb picview: Update to version 3.1.1                         extras       54 minutes ago
 * 7b601e12e415 natscli: Update to version 0.2.2                         extras       54 minutes ago
 * 4d502f786cd7 materialgram: Update to version 5.13.1.1                 extras       54 minutes ago
 * d985c31abe10 lazygit: Update to version 0.49.0                        extras       54 minutes ago
 * 5352bf954a67 gitbutler: Update to version 0.14.18                     extras       54 minutes ago
Scoop was updated successfully!
Installing 'oh-my-posh' (25.13.0) [64bit] from 'main' bucket
themes.zip (127.5 KB) [=========================================================================================================================================================================================] 100%
Checking hash of themes.zip ... ok.
posh-windows-amd64.exe (18.2 MB) [==============================================================================================================================================================================] 100%
Checking hash of posh-windows-amd64.exe ... ok.
Extracting themes.zip ... done.
Linking ~\scoop\apps\oh-my-posh\current => ~\scoop\apps\oh-my-posh\25.13.0
Creating shim for 'oh-my-posh'.
'oh-my-posh' (25.13.0) was installed successfully!
Notes
-----
Refer to 'https://ohmyposh.dev/docs/installation/prompt' for shell specific configurations.
PS C:\>
```

## Running
```bash
PS C:\> oh-my-posh version
25.13.0
PS C:\>
```

## Install Font
```bash
PS C:\> oh-my-posh font install

    ⣟  Installing Meslo
```
```bash 
    Successfully installed Meslo 🚀

    The following font families are now available for configuration:

      • MesloLGL Nerd Font
      • MesloLGL Nerd Font Mono
      • MesloLGL Nerd Font Propo
      • MesloLGLDZ Nerd Font
      • MesloLGLDZ Nerd Font Mono
      • MesloLGLDZ Nerd Font Propo
      • MesloLGM Nerd Font
      • MesloLGM Nerd Font Mono
      • MesloLGM Nerd Font Propo
      • MesloLGMDZ Nerd Font
      • MesloLGMDZ Nerd Font Mono
      • MesloLGMDZ Nerd Font Propo
      • MesloLGS Nerd Font
      • MesloLGS Nerd Font Mono
      • MesloLGS Nerd Font Propo
      • MesloLGSDZ Nerd Font
      • MesloLGSDZ Nerd Font Mono
      • MesloLGSDZ Nerd Font Propo

PS C:\>
```

## Profile
### Path
```bash
PS C:\> $profile
C:\Users\Admin\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
PS C:\> 
```

### Edit
```bash
PS C:\> code $profile
PS C:\>
```

```bash
oh-my-posh init pwsh --config 'https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/jandedobbeleer.omp.json' | Invoke-Expression
```

## Running

Close `Terminal` and open it again

## Uninstall
```bash
PS C:\> scoop uninstall oh-my-posh                                pwsh  18:03:48 
Uninstalling 'oh-my-posh' (25.13.0).
Removing shim 'oh-my-posh.shim'.
Removing shim 'oh-my-posh.exe'.
Unlinking ~\scoop\apps\oh-my-posh\current
'oh-my-posh' was uninstalled.
PS C:\>
```
