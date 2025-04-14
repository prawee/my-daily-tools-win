# How to install `DBeaver` with scoop

## Finding
```bash
PS C:\> scoop search dbeaver
Results from local buckets...

Name    Version Source Binaries
----    ------- ------ --------
dbeaver 25.0.2  extras


PS C:\>
```

## Install
```bash
PS C:\> scoop install dbeaver
Installing 'dbeaver' (25.0.2) [64bit] from 'extras' bucket
dbeaver-ce-25.0.2-win32.win32.x86_64.zip (124.6 MB) [=========================================================================================================================] 100%
Checking hash of dbeaver-ce-25.0.2-win32.win32.x86_64.zip ... ok.
Extracting dbeaver-ce-25.0.2-win32.win32.x86_64.zip ... done.
Linking ~\scoop\apps\dbeaver\current => ~\scoop\apps\dbeaver\25.0.2
Creating shim for 'dbeaver'.
Making C:\Users\Admin\scoop\shims\dbeaver.exe a GUI binary.
Creating shim for 'dbeaver-cli'.
Creating shortcut for DBeaver (dbeaver.exe)
'dbeaver' (25.0.2) was installed successfully!
'dbeaver' suggests installing 'java/oraclejdk' or 'java/oraclejre8' or 'java/openjdk11'.
PS C:\>
```