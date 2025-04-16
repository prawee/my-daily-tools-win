# How to install Node.js with scoop

## Checking
```bash
PS C:\> node -v
v16.12.0
```

## Searching
```bash
PS C:\> scoop search node
Results from local buckets...

Name           Version                          Source   Binari
                                                         es
----           -------                          ------   ------
eventstore     24.6.0                           main     Eve...
geth           1.15.8                           main     boo...
nodejs-lts     22.14.0                          main
nodejs         23.11.0                          main
pulumi         3.162.0                          main     pul...
sliksvn        1.14.2b                          main     svn...
nodejs-nightly 24.0.0-nightly20250411795dd8eb79 versions
nodejs010      0.10.48                          versions
nodejs012      0.12.18                          versions
nodejs10       10.24.1                          versions
nodejs11       11.15.0                          versions
nodejs12       12.22.12                         versions
nodejs14       14.21.3                          versions
nodejs16       16.20.2                          versions
nodejs18       18.20.8                          versions
nodejs20       20.19.0                          versions
nodejs22       22.14.0                          versions
nodejs4        4.9.1                            versions
nodejs5        5.12.0                           versions
nodejs6        6.17.1                           versions
nodejs7        7.10.1                           versions
nodejs8        8.17.0                           versions
nodejs9        9.11.2                           versions

PS C:\>
```

## Install Node with some version
```bash
PS C:\> scoop install versions/nodejs20
Installing 'nodejs20' (20.19.0) [64bit] from 'versions' bucket
node-v20.19.0-win-x64.7z (18.2 MB) [=====================================] 100%
Checking hash of node-v20.19.0-win-x64.7z ... ok.
Extracting node-v20.19.0-win-x64.7z ... done.
Linking ~\scoop\apps\nodejs20\current => ~\scoop\apps\nodejs20\20.19.0
Adding ~\scoop\apps\nodejs20\current\bin to your path.
Adding ~\scoop\apps\nodejs20\current to your path.
Persisting bin
Persisting cache
Running post_install script...done.
'nodejs20' (20.19.0) was installed successfully!
PS C:\>
```

## Checking again
```bash
PS C:\> node -v
v20.19.0
PS C:\>
```

## Uninstall
```bash
PS C:\> scoop uninstall nodejs20
Uninstalling 'nodejs20' (20.19.0).
Unlinking ~\scoop\apps\nodejs20\current
Removing ~\scoop\apps\nodejs20\current\bin from your path.
Removing ~\scoop\apps\nodejs20\current from your path.
'nodejs20' was uninstalled.
PS C:\>
```
