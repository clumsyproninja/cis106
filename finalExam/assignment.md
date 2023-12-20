---
name: Andeivi Mejia Taveras
semester: Fall 23
Course: CIS 106 Linux Fundamentals
---

# Final Assignment

## Question 1

### awk
- Description: Awk is useful for manipulation of data files, text retrieval and processing
- Syntax: `awk + options + {awk command} + file`
- Examples:
  - First field: `awk -F';' '{print $1}' /etc/passwd`
  - Start from a line: `awk 'NR > 3 {print}' /etc/passwd`
  - Change field to uppercase: `awk -F: {print toupper($1)}`

### cat
- Description: Concatenate files and print on the standard output
- Syntax: `cat + options + file`
- Examples:
  - See content: `cat /Documents/test.md`
  - See content with line numbers: `cat -n /Downloads/settings.py`
  - Show line ends: `cat -E /Documents/test.md`

### cp
- Description: copy files and directories
- Syntax: `cp + option + file`
- Examples:
  - Copy a file: `cp /Downloads/settings.py /Documents/python/`
  - Copy multiple files: `cp /Downloads/settings.py /Downloads/menu.py /Documents/python/`
  - Copy directories recursively: `cp -r /Downloads/python/ /Documents/python-backup/`

### cut
- Description: Remove sections from each line of files
- Syntax: `cut + option + file`
- Examples:
  - First field: `cut -d ';' -f1 /etc/passwd`
  - Replace delimiter: `cut -d ';' -f1,2 --output-delimiter=' is ' /etc/passwd`
  - Range of characters: `cut -c 1-7,16-23 database.txt`

### grep
- Description: searches for patterns in each file
- Syntax: `grep + option + file`
- Examples:
  - Ignore case: `grep -i 'toyota' /Documents/cars.txt`
  - Show line number: `grep -n 'toyota' /Documents/cars.txt`
  - Count number of matches: `grep -c 'toyota' /Documents/cars.txt`

### head
- Description: Display beginning of a file, default 10
- Syntax: `head + option + file`
- Examples:
  - Show first 10 lines: `head /Documents/games.txt `
  - Show first line: `head -n 1 /Documents/games.txt`
  - Show first 20 characters: `head -c 20 /Documents/games.txt`

### ls
- Description: List directory contents
- Syntax: `ls + option + directory`
- Examples:
  - List directories: `ls /Pictures`
  - Long-list directories: `ls -l /Pictures`
  - List and classify: `ls -F /Pictures`

### man
- Description: Display the manual page for a command
- Syntax: `man + option + command`
- Examples:
  - Show manual page for command: `man ls`
  - Show description: `man -f ls`
  - Search for commands related to keyword: `man -k pattern`

### mkdir
- Description: Creates new directories
- Syntax: `mkdir + options + directory`
- Examples:
  - Create directory: `mkdir newFolder`
  - Create nested directories: `mkdir -p newFolder/files`
  - Create multiple nested directories: `mkdir -p newFolder/files/{old,new}`

### mv
- Description: Move or rename files
- Syntax: `mv + options + files`
- Examples:
  - Move a file: `mv /Downloads/games.txt /Documents/`
  - Rename a file: `mv /Downloads/unknown.txt /Downloads/games.txt`
  - Move all .txt files: `mv /Downloads/*.txt /Documents/txtFiles`

### tac
- Description: Display a file in reverse
- Syntax: `tac + option + file`
- Examples:
  - Display file in reverse order: `tac file.txt`
  - Reversed with delimiter: `tac -s delimiter file.csv`
  - Concatenate and display files in reverse order: `tac file.txt file2.txt`

### tail
- Description: Display last part of files
- Syntax: `tail + option + files`
- Examples:
  - Display last 10 lines: `tail ../file.txt`
  - Display last 5 lines: `tail -5 ../file.txt`
  - Display last line: `tail -1 ../file.txt`

### touch
- Description: Create empty files
- Syntax: `touch + options + file`
- Examples:
  - Create new file: `touch newFile.md`
  - Create multiple files: `touch newFile.md ../newFile.txt`
  - Update access and modification times: `touch -c file.txt`

### tr
- Description: Translate or delete characters
- Syntax: `tr + options + file`
- Examples:
  - Convert lowercase to uppercase: `cat assignment.txt | tr 'a-z' 'A-Z`
  - Delete delimiter: `cat /etc/passwd | tr ';' ''`
  - Delete vowels: `echo 'remove vowels' | tr -d 'aeiou'`

### tree
- Description: Display directory structure as a tree
- Syntax: `tree + options + directory`
- Examples:
  - Display current directory tree: `tree`
  - Display tree up to 2 depth levels: `tree -L 2`
  - Display only directories: `tree -d`


## Question 2

### How to work with multiple terminals open?
Press add terminal right or bottom in tilix. (Top left buttons)

### How to work with manual pages?
Use the man command along with the command name. Press Q to exit.

### How to parse (search) for specific words in the manual page
Use -k option to search for keywords.

### How to redirect output (> and |)
The ">" allows to redirect output to a file. "|" can be used to pipe output from one command to another

### How to append the output of a command to a file
Use ">>" to append output to a file

### How to use wildcards
The "*" matches any character, the "?" matches a single character

### For copying and moving multiple files at the same time
Use cp for copying files and mv for moving

### How to use brace expansion
Brace expansion generations sequences. For example, `mv file{1,2,3} destination`, enables moving multiple files named "file1, file2, file3" to be moved.

### For creating entire directory structures in a single command
Use mkdir -p to create parent directories along with the target directory. For example, `mkdir -p parent/child/grandchild`