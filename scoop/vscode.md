# Install `VSCode` with scoop

## Bucket
```bash
PS C:\> scoop bucket
scoop bucket: cmd '' not supported
Usage: scoop bucket add|list|known|rm [<args>]
```

## Searching
```bash
PS C:\> scoop search vscode
Results from local buckets...

Name      Version  Source Binaries
----      -------  ------ --------
winpython 3.12.4.1 main   winvscode.bat | winvscode.bat
```

## Installation
```bash
PS C:\> scoop bucket add versions
Checking repo... OK
The versions bucket was added successfully.
```

```bash
PS C:\> scoop bucket list

Name     Source                                     Updated
----     ------                                     -------
main     https://github.com/ScoopInstaller/Main.git 4/12/2025 3:28...
versions https://github.com/ScoopInstaller/Versions 4/12/2025 3:36...
```

```bash
PS C:\> scoop install versions/vscode-insiders
Installing '7zip' (24.09) [64bit] from 'main' bucket
7z2409-x64.msi (1.9 MB) [===================================] 100%
Checking hash of 7z2409-x64.msi ... ok.
Extracting 7z2409-x64.msi ... done.
Linking ~\scoop\apps\7zip\current => ~\scoop\apps\7zip\24.09
Creating shim for '7z'.
Creating shim for '7zFM'.
Making C:\Users\ADMIN\scoop\shims\7zfm.exe a GUI binary.
Creating shim for '7zG'.
Making C:\Users\ADMIN\scoop\shims\7zg.exe a GUI binary.
Creating shortcut for 7-Zip (7zFM.exe)
Persisting Codecs
Persisting Formats
Running post_install script...done.
'7zip' (24.09) was installed successfully!
Notes
-----
Add 7-Zip as a context menu option by running:
"C:\Users\ADMIN\scoop\apps\7zip\current\install-context.reg"
Installing 'vscode-insiders' (1.100.0-1744347907130) [64bit] from 'versions' bucket
dl.7z (144.0 MB) [=============================================>                         ]  65%
```

```bash
dl.7z (144.0 MB) [=======================================================================] 100%
Checking hash of dl.7z ... ok.
Extracting dl.7z ... done.
Linking ~\scoop\apps\vscode-insiders\current => ~\scoop\apps\vscode-insiders\1.100.0-1744347907130
Creating shortcut for Visual Studio Code - Insiders (Code - Insiders.exe)
Adding ~\scoop\apps\vscode-insiders\current\bin to your path.
Persisting data
Running post_install script...INFO  [Portable Mode] Copying extensions...
INFO  [Portable Mode] Copying user data...
INFO  Adjusting path in extensions file...
done.
'vscode-insiders' (1.100.0-1744347907130) was installed successfully!
Notes
-----
Add Visual Studio Code as a context menu option by running:
'reg import "C:\Users\ADMIN\scoop\apps\vscode-insiders\current\install-context.reg"'
For file associations, run:
'reg import "C:\Users\ADMIN\scoop\apps\vscode-insiders\current\install-associations.reg"'
```

## Using it
```bash
PS C:\> code-insiders --version
1.100.0-insider
043f699013796cbeae7c8fe9abac9b9eb26b3c51
x64
PS C:\>
```

### Open current source
```bash
PS C:\> code-insiders .
```

## Reference
<https://www.anmalkov.com/blog/use-code-command-to-run-vscode-insiders>
