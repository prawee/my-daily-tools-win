# How to install scoop cli for windows (like brew)

Open your `Windows PowerShell` with normal mode

## Installation
### Into root of C drive
```bash
PS C:\Users\ADMIN> cd C:/
PS C:\>
```

### Put this command (2 line)
```bash
PS C:\> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
PS C:\> Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
Initializing...
Downloading...
```

### Waiting a minute
```bash
Creating shim...
Adding ~\scoop\shims to your path.
Scoop was installed successfully!
Type 'scoop help' for instructions.
PS C:\>
```

## Version
```bash
PS C:\> scoop -V | scoop --version | scoop -v

Current Scoop version:
859d1db5 (HEAD -> master, tag: v0.5.2, origin/master, origin/HEAD) chore(release): Bump to version 0.5.2 (#6080)

'main' bucket:
4031f7090 (HEAD -> master, origin/master, origin/HEAD) vcpkg: Update to version 2025.04.09

PS C:\>
```

## List
```bash
PS C:\> scoop list
There aren't any apps installed.
PS C:\>
```

## Available commands
```bash
PS C:\> scoop

Usage: scoop <command> [<args>]

Available commands are listed below.

Type 'scoop help <command>' to get more help for a specific command.

Command    Summary
-------    -------
alias      Manage scoop aliases
bucket     Manage Scoop buckets
cache      Show or clear the download cache
cat        Show content of specified manifest.
checkup    Check for potential problems
cleanup    Cleanup apps by removing old versions
config     Get or set configuration values
create     Create a custom app manifest
depends    List dependencies for an app, in the order they'...
download   Download apps in the cache folder and verify hashes
export     Exports installed apps, buckets (and optionally ...
help       Show help for a command
hold       Hold an app to disable updates
home       Opens the app homepage
import     Imports apps, buckets and configs from a Scoopfi...
info       Display information about an app
install    Install apps
list       List installed apps
prefix     Returns the path to the specified app
reset      Reset an app to resolve conflicts
search     Search available apps
shim       Manipulate Scoop shims
status     Show status and check for new app versions
unhold     Unhold an app to enable updates
uninstall  Uninstall an app
update     Update apps, or Scoop itself
virustotal Look for app's hash or url on virustotal.com
which      Locate a shim/executable (similar to 'which' on ...

PS C:\>
```




