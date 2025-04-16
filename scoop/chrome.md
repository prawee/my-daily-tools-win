# How to install `Google Chrome` with scoop

## Searching
```bash
PS C:\> scoop search googlechrome
Results from local buckets...

Name                Version       Source   Binaries
----                -------       ------   --------
googlechrome        135.0.7049.96 extras
googlechrome-beta   136.0.7103.25 versions
googlechrome-canary 137.0.7126.0  versions
googlechrome-dev    137.0.7117.2  versions


PS C:\>
```

## Installation
```bash
PS C:\> scoop install googlechrome
Installing 'googlechrome' (135.0.7049.96) [64bit] from 'extras' bucket
135.0.7049.96_chrome_installer.exe (114.5 MB) [=========================================================================================================] 100%
Checking hash of 135.0.7049.96_chrome_installer.exe ... ok.
Extracting 135.0.7049.96_chrome_installer.exe ... done.
Running installer script...done.
Linking ~\scoop\apps\googlechrome\current => ~\scoop\apps\googlechrome\135.0.7049.96
Creating shim for 'chrome'.
Making C:\Users\prawe\scoop\shims\chrome.exe a GUI binary.
Creating shortcut for Google Chrome (chrome.exe)
'googlechrome' (135.0.7049.96) was installed successfully!
PS C:\>
```

## Running
```bash
PS C:\> chrome
```

