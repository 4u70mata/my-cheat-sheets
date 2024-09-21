#### Linux short cheat-sheet focused on installation, file management, and using pipes:

| **Category**         | **Command**                                       | **Description**                                 |
|----------------------|---------------------------------------------------|-------------------------------------------------|
| **File Management**   | `ls -l`                                          | List files                                      |
|                      | `cd /path/to/directory`                          | Change directory                                |
|                      | `mkdir directory_name`                           | Create a directory                              |
|                      | `rm filename`                                    | Remove a file                                   |
|                      | `rm -r directory_name`                           | Remove a directory and its contents             |
|                      | `cp source_file destination_file`                | Copy files                                      |
|                      | `mv source_file destination_file`                | Move files                                      |
| **Compression**      | `tar -czvf archive_name.tar.gz /path/to/directory` | Compress a directory                          |
|                      | `tar -xzvf archive_name.tar.gz`                  | Extract a tar.gz file                           |
|                      | `zip archive_name.zip file1 file2`               | Zip files                                       |
|                      | `unzip archive_name.zip`                          | Unzip a zip file                                |
| **Searching**        | `grep 'search_term' filename`                    | Search for a string in a file                   |
|                      | `grep -r 'search_term' /path/to/directory`      | Recursive search in a directory                 |
|                      | `grep -n 'search_term' filename`                 | Show line numbers with grep                     |
|                      | `grep -c 'search_term' filename`                 | Count occurrences of a string                   |
| **Piping**           | `command1 | command2`                           | Pipe output to another command                  |
|                      | `command > output.txt`                           | Redirect output to a file                       |
|                      | `command >> output.txt`                          | Append output to a file                         |
|                      | `cat filename`                                   | View a file                                     |
| **Package Management**| `sudo apt update`                               | Update package list                             |
|                      | `sudo apt upgrade`                               | Upgrade installed packages                       |
|                      | `sudo apt install package_name`                  | Install a package                               |
|                      | `sudo apt remove package_name`                   | Remove a package                                |
|                      | `apt search package_name`                        | Search for a package                            |
| **System Info**      | `df -h`                                         | Check disk usage                                |
|                      | `free -h`                                       | Check memory usage                              |
|                      | `top`                                           | Show running processes                           |
|                      | `pwd`                                           | Check your current path                         |
| **Miscellaneous**    | `man command_name`                              | View the manual for a command                   |
|                      | `touch filename`                                 | Create an empty file                            |
|                      | `nano filename`                                  | Edit a file using nano                          |
