# How to install `Table Plus` with scoop

## Searching
```bash
PS C:\> scoop search tableplus
Results from local buckets...

Name      Version   Source Binaries
----      -------   ------ --------
tableplus 6.4.8.310 extras


PS C:\>
```

## Installation
```bash
PS C:\> scoop install tableplus
Installing 'innounp' (2.64.3) [64bit] from 'main' bucket
innounp-2.zip (537.6 KB) [=============================================================================================================================================] 100%    
Checking hash of innounp-2.zip ... ok.
Extracting innounp-2.zip ... done.
Linking ~\scoop\apps\innounp\current => ~\scoop\apps\innounp\2.64.3
Creating shim for 'innounp'.
'innounp' (2.64.3) was installed successfully!
Installing 'tableplus' (6.4.8.310) [64bit] from 'extras' bucket
TablePlusSetup.exe (173.7 MB) [========================================================================================================================================] 100%    
Checking hash of TablePlusSetup.exe ... ok.
Extracting TablePlusSetup.exe ... done.
Running pre_install script...done.
Linking ~\scoop\apps\tableplus\current => ~\scoop\apps\tableplus\6.4.8.310
Creating shim for 'TablePlus'.
Making C:\Users\Admin\scoop\shims\tableplus.exe a GUI binary.
Creating shortcut for TablePlus (TablePlus.exe)
'tableplus' (6.4.8.310) was installed successfully!
PS C:\>
```

## Uninstall
```bash
PS C:\> scoop uninstall tableplus                              
Uninstalling 'tableplus' (6.4.8.310).
Removing shim 'TablePlus.shim'.
Removing shim 'TablePlus.exe'.
Removing shortcut ~\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Scoop Apps\TablePlus.lnk
Unlinking ~\scoop\apps\tableplus\current
'tableplus' was uninstalled.
PS C:\>
```
