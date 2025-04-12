# How to install `AWS` cli

## Searching 
```bash
PS C:\> scoop search aws
Results from local buckets...

Name                  Version Source Binaries
----                  ------- ------ --------
aws-amplify           13.0.0  main
aws-copilot           1.34.1  main
aws-ecs               1.21.0  main
aws-iam-authenticator 0.6.31  main
aws-nuke              2.25.0  main
aws-sam-cli           1.137.1 main
aws-vault             7.2.0   main
aws                   2.26.1  main
awsqueue              0.0.8   main
awsSts                0.9.1   main
saml2aws              2.36.19 main


PS C:\>
```

## Install
```bash
PS C:\> scoop install aws
Updating Scoop...
WARN  Uncommitted changes detected. Update aborted.
Updating Buckets...
 * da3f7934efb8 tailspin: Update to version 5.2.1                        main         78 minutes ago
 * aa44cdbba21f hugo: Update to version 0.146.3                          main         78 minutes ago
 * cd9eb32edd1a hugo-extended: Update to version 0.146.3                 main         78 minutes ago
 * c9a79b8b2351 golangci-lint: Update to version 2.1.1                   main         78 minutes ago
 * 94602ff19f34 edgedriver: Update to version 135.0.3179.73              main         78 minutes ago
 * d6368490d795 syncthing: Update to version 1.29.5                      main         5 hours ago
 * 8e48ada91e34 stdiscosrv: Update to version 1.29.5                     main         5 hours ago
 * 069551a4a7b5 gawk: Update to version 5.3.2                            main         5 hours ago
 * ee59b070b880 edgedriver: Update to version 135.0.3179.66              main         5 hours ago
 * c88debad8efd conftest: Update to version 0.59.0                       main         5 hours ago
 * 510cef7beb9a suanpan: Update to version 3.7                           main         9 hours ago
 * de0cc45024ea podman-tui: Add version 1.5.0 (#6709)                    main         10 hours ago
 * a83728c93bf4 rtools: Update to version 4.5.6536.6492 (#6708)          main         10 hours ago
Scoop was updated successfully!
Installing 'aws' (2.26.1) [64bit] from 'main' bucket
AWSCLIV2-2.26.1.msi (41.8 MB) [===============================================================================] 100%
Checking hash of AWSCLIV2-2.26.1.msi ... ok.
Extracting AWSCLIV2-2.26.1.msi ... done.
Linking ~\scoop\apps\aws\current => ~\scoop\apps\aws\2.26.1
Creating shim for 'aws'.
Creating shim for 'aws_completer'.
'aws' (2.26.1) was installed successfully!
PS C:\>
```

## Checking
```bash
PS C:\> aws --version
aws-cli/2.26.1 Python/3.13.2 Windows/10 exe/AMD64
PS C:\>
```