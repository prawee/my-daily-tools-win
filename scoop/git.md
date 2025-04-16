# How to install `Git` with scoop

## Searching
```bash
PS C:\> scoop search git
Results from local buckets...

Name                        Version          Source Binaries
----                        -------          ------ --------
biodiff                     1.2.1            main   git-biodiff.exe
git-absorb                  0.7.0            main
git-annex                   10.20250416      main
git-branchless              0.10.0           main
git-bug                     0.8.0            main
git-chglog                  0.15.4           main
git-cliff                   2.8.0            main
git-crypt                   0.7.0            main
git-filter-repo             2.47.0           main
git-interactive-rebase-tool 2.3.0            main
git-istage                  0.3.108          main
git-lfs                     3.6.1            main
git-machete                 3.34.1           main
git-quick-stats             2.5.8            main
git-sizer                   1.5.0            main
git-tfs                     0.34.0           main
git-town                    18.3.2           main
git-up                      2.3.0            main
git-with-openssh            2.48.1.windows.1 main
git-xargs                   0.1.16           main
git                         2.49.0           main
gitea                       1.23.7           main
gitignore                   0.2018.07.25     main
gitkube                     0.3.0            main
gitlab-release-cli          0.23.0           main
gitlab-runner               17.10.1          main
gitleaks                    8.24.3           main
gitomatic                   0.2              main
gitql                       0.37.0           main
gitsign                     0.13.0           main
gitui                       0.27.0           main
gitversion                  6.1.0            main
legit                       1.2.0            main
mingit-busybox              2.49.0           main
mingit                      2.49.0           main
psgithub                    0.15.240         main
psutils                     0.2023.06.28     main   gitignore.ps1
stgit                       2.5.3            main


PS C:\>
```

## Installation
```bash
PS C:\> scoop install main/git
Installing '7zip' (24.09) [64bit] from 'main' bucket
7z2409-x64.msi (1.9 MB) [=====================================================================================] 100%
Checking hash of 7z2409-x64.msi ... ok.
Extracting 7z2409-x64.msi ... done.
Linking ~\scoop\apps\7zip\current => ~\scoop\apps\7zip\24.09
Creating shim for '7z'.
Creating shim for '7zFM'.
Making C:\Users\prawe\scoop\shims\7zfm.exe a GUI binary.
Creating shim for '7zG'.
Making C:\Users\prawe\scoop\shims\7zg.exe a GUI binary.
Creating shortcut for 7-Zip (7zFM.exe)
Persisting Codecs
Persisting Formats
Running post_install script...done.
'7zip' (24.09) was installed successfully!
Notes
-----
Add 7-Zip as a context menu option by running: "C:\Users\prawe\scoop\apps\7zip\current\install-context.reg"
Installing 'git' (2.49.0) [64bit] from 'main' bucket
PortableGit-2.49.0-64-bit.7z.exe (61.2 MB) [==================================================================] 100%
Checking hash of PortableGit-2.49.0-64-bit.7z.exe ... ok.
Extracting PortableGit-2.49.0-64-bit.7z.exe ... done.
Linking ~\scoop\apps\git\current => ~\scoop\apps\git\2.49.0
Creating shim for 'sh'.
Creating shim for 'bash'.
Creating shim for 'git'.
Creating shim for 'gitk'.
Making C:\Users\prawe\scoop\shims\gitk.exe a GUI binary.
Creating shim for 'git-gui'.
Making C:\Users\prawe\scoop\shims\git-gui.exe a GUI binary.
Creating shim for 'scalar'.
Creating shim for 'tig'.
Creating shim for 'git-bash'.
Making C:\Users\prawe\scoop\shims\git-bash.exe a GUI binary.
Creating shortcut for Git Bash (git-bash.exe)
Creating shortcut for Git GUI (git-gui.exe)
Running post_install script...done.
'git' (2.49.0) was installed successfully!
Notes
-----
Set Git Credential Manager Core by running: "git config --global credential.helper manager"

To add context menu entries, run 'C:\Users\prawe\scoop\apps\git\current\install-context.reg'

To create file-associations for .git* and .sh files, run
'C:\Users\prawe\scoop\apps\git\current\install-file-associations.reg'
PS C:\>
```

## Using with version
```bash
PS C:\> git -v
git version 2.49.0.windows.1
PS C:\>
```
