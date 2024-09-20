A Quick Ref cheat-sheet comparing common Linux commands with their PowerShell equivalents:


| **Linux Command**           | **PowerShell Equivalent**          | **Description**                       |
|-----------------------------|------------------------------------|---------------------------------------|
| `ls`                        | `Get-ChildItem` or `ls`           | List directory contents               |
| `cd <directory>`            | `Set-Location <directory>` or `cd <directory>` | Change directory                     |
| `pwd`                       | `Get-Location` or `pwd`           | Print working directory               |
| `cat <file>`                | `Get-Content <file>` or `cat <file>` | Display file content                 |
| `cp <source> <dest>`        | `Copy-Item <source> <dest>`       | Copy files                           |
| `mv <source> <dest>`        | `Move-Item <source> <dest>`       | Move or rename files                 |
| `rm <file>`                 | `Remove-Item <file>`              | Remove files                         |
| `mkdir <directory>`         | `New-Item -ItemType Directory <directory>` or `mkdir <directory>` | Create a directory                   |
| `rmdir <directory>`         | `Remove-Item <directory>`          | Remove a directory                   |
| `touch <file>`              | `New-Item <file>`                  | Create a new file                    |
| `echo <text>`               | `Write-Output <text>` or `echo <text>` | Output text                          |
| `grep <pattern> <file>`     | `Select-String -Pattern <pattern> -Path <file>` | Search for patterns in files         |
| `find <directory> -name <name>` | `Get-ChildItem -Path <directory> -Filter <name> -Recurse` | Find files by name                  |
| `chmod`                     | `Set-Acl` (more complex)          | Change file permissions               |
| `ps`                        | `Get-Process`                      | List running processes                |
| `kill <pid>`                | `Stop-Process -Id <pid>`          | Terminate a process                  |
| `top`                       | `Get-Process`                      | Display running processes (use `top` for real-time) |
| `history`                   | `Get-History`                      | Show command history                  |
| `man <command>`             | `Get-Help <command>`               | Show command help                     |
| `which <command>`           | `Get-Command <command>`            | Locate a command's path               |
| `wget <url>`                | `Invoke-WebRequest <url>`          | Download files from the web          |
| `curl <url>`                | `Invoke-WebRequest <url>`          | Transfer data from/to a server       |
