# How to install `Yarn` with scoop

## Searching
```bash
PS C:\> scoop search yarn
Results from local buckets...

Name Version Source Binaries
---- ------- ------ --------
yarn 1.22.22 main


PS C:\>
```

## Installation
```bash
PS C:\> scoop install yarn
Installing 'yarn' (1.22.22) [64bit] from 'main' bucket
yarn-v1.22.22.tar.gz (1.2 MB) [===============================================================================] 100%
Checking hash of yarn-v1.22.22.tar.gz ... ok.
Extracting yarn-v1.22.22.tar.gz ... done.
Linking ~\scoop\apps\yarn\current => ~\scoop\apps\yarn\1.22.22
Adding ~\scoop\apps\yarn\current\global\node_modules\.bin to your path.
Adding ~\scoop\apps\yarn\current\bin to your path.
Persisting cache
Persisting global
Persisting mirror
yarn config v1.22.22
success Set "cache-folder" to "C:\\Users\\prawe\\scoop\\apps\\yarn\\current\\cache".
Done in 0.05s.
yarn config v1.22.22
success Set "yarn-offline-mirror" to "C:\\Users\\prawe\\scoop\\apps\\yarn\\current\\mirror".
Done in 0.04s.
yarn config v1.22.22
success Set "global-folder" to "C:\\Users\\prawe\\scoop\\apps\\yarn\\current\\global".
Done in 0.05s.
yarn config v1.22.22
success Set "prefix" to "C:\\Users\\prawe\\scoop\\apps\\yarn\\current\\global".
Done in 0.04s.
done.
'yarn' (1.22.22) was installed successfully!
'yarn' suggests installing 'nodejs' or 'nodejs-lts' or 'nvm' or 'nvs'.
PS C:\>
```

## Running with version
```bash
PS C:\> yarn -v
1.22.22
PS C:\>
```
