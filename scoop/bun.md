# Install `Bun` cli

## Searching
```bash
PS C:\> scoop search bun
Results from local buckets...

Name       Version                   Source   Binaries
----       -------                   ------   --------
bun        1.2.10                    main
busybox    5579-g5749feb35           main     bunzip2
bzip2      1.0.8.0                   main     bunzip2.exe
gow        0.8.0                     main     bunzip2.exe
unxutils   2007.03.01                main     bunzip2.exe
cfssl      1.6.5                     extras   cfssl-bundle.exe | mkbundle.exe
bun-canary 1.1.22-canary.1+dbd320ccf versions


PS C:\>
```

## Installation
```bash
PS C:\> scoop install bun
Installing 'bun' (1.2.10) [64bit] from 'main' bucket
bun-windows-x64.zip (38.2 MB) [===============================================================================] 100%
Checking hash of bun-windows-x64.zip ... ok.
bun-windows-x64-baseline.zip (38.1 MB) [======================================================================] 100%
Checking hash of bun-windows-x64-baseline.zip ... ok.
Extracting bun-windows-x64.zip ... done.
Extracting bun-windows-x64-baseline.zip ... done.
Running pre_install script...done.
Linking ~\scoop\apps\bun\current => ~\scoop\apps\bun\1.2.10
Creating shim for 'bun'.
Creating shim for 'bunx'.
'bun' (1.2.10) was installed successfully!
'bun' suggests installing 'extras/vcredist2022'.
PS C:\>
```

## Checking
```bash
PS C:\> bun --version
1.2.10
PS C:\>
```
