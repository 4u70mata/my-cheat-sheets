### Piping and filtering basics:

| **Pipe Type**        | **Command**                                       | **Description**                                 |
|----------------------|---------------------------------------------------|-------------------------------------------------|
| **Basic Pipe**       | `command1 | command2`                           | Pass output of command1 to command2            |
| **Filter with `grep`** | `command | grep 'search_term'`                 | Filter output for lines containing 'search_term' |
| **Filter with `awk`** | `command | awk '{print $1}'`                     | Select specific columns from the output        |
| **Filter with `sort`**| `command | sort`                                | Sort the output                                 |
| **Filter with `uniq`**| `command | sort | uniq`                        | Remove duplicate lines from sorted output      |
| **Redirecting Errors**| `command 2> error.log`                        | Redirect error messages to a file              |
| **Combining Output** | `command1 | command2 > output.txt`              | Redirect output of command2 to a file after processing the output of command1."  |

#### File-related pipes and redirection

| **Command**                       | **Description**                                      |
|-----------------------------------|------------------------------------------------------|
| `command1 > file.txt`            | Redirect standard output to a file (overwrite)      |
| `command1 >> file.txt`           | Redirect standard output to a file (append)         |
| `command1 2> error.txt`          | Redirect standard error to a file                    |
| `command1 &> output.txt`         | Redirect both stdout and stderr to a file (specific to shells like Bash)   |
| `command1 | command2`            | Pipe output of command1 to command2                  |
| `cat file.txt | grep 'search_term'` | Search for a term in a file using `grep`            |
| `ls | sort > sorted_files.txt`   | List files and sort them, saving to a file          |
| `command | tee file.txt`         | Display output and save it to a file simultaneously   |

Example of scenarios involving pipes, file handling, and common tasks like downloading, unzipping, and moving files : 

| **Scenario**                                           | **Command**                                                  | **Description**                                                 |
|-------------------------------------------------------|--------------------------------------------------------------|-----------------------------------------------------------------|
| **Download a file and save it**                       | `curl -O http://example.com/file.zip`                       | Download a file from a URL.                                    |
| **Download and unzip**                                | `curl -O http://example.com/file.zip && unzip file.zip`    | Download and then unzip the downloaded file.                   |
| **Download, unzip, and move**                         | `curl -O http://example.com/file.zip && unzip file.zip && mv file /destination/` | Download, unzip, and move the extracted file.                  |
| **Search within a file after downloading**            | `curl -O http://example.com/file.txt && grep 'search_term' file.txt` | Download a file and search for a term in it.                   |
| **Download and view contents of a text file**        | `curl -O http://example.com/file.txt && cat file.txt`      | Download a text file and display its contents.                 |
| **Download, sort lines, and save to a new file**     | `curl -O http://example.com/file.txt && sort file.txt > sorted.txt` | Download, sort lines in a file, and save them to a new file.  |
| **Download, unzip, and filter contents**              | `curl -O http://example.com/file.zip && unzip -p file.zip | grep 'search_term'` | Download, unzip, and filter specific lines from the content.   |
| **Combine multiple commands with pipes**              | `curl -O http://example.com/file.zip && unzip file.zip | mv file /destination/` | Download, unzip, and move file in a single flow.               |
| **Create a directory, download, and move**           | `mkdir -p /destination && curl -O http://example.com/file.zip && mv file.zip /destination/` | Create a directory and move the downloaded file into it.      |


Note :I created these resources to help me to enhance efficiency and quick ref of Linux command-line operations, ensuring i can perform common tasks seamlessly in my data engineer workflow.