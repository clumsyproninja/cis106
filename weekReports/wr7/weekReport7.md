---
name: Andeivi Mejia Taveras
semester: Spring 23
course: cis106
---

# Week Report 7

## cat command
- Command is used for: display file content
- Formula: `cat + option + files(s) to display`
- Example 1: Display content
  - `cat file.txt`
- Example 2: Display content with line numbers
  - `cat -n file.txt`

## tac command
- Command is used for: display file content in reverse
- Formula: `tac + option + file(s) to display`
- Example 1: Display content in reverse
  - `tac games.md`
- Example 2: Display content in reverse absolute path
  - `tac ~/Documents/Books/bible.txt`

## head command
- Command is used for: displays top N number of lines of a file
- Formula: `head + option + files(s)`
- Example 1: Display the first 10 of a file
  - `head Documents/Books/dracula.txt`
- Example 2: Display the first 5 lines
  - `head -5 Documents/users.txt`

## tail command
- Command is used for: displays last N number of lines of a file
- Formula: `tail + option + files(s)`
- Example 1: Display the last 10 lines of a file
  - `tail Documents/Books/dracula.txt`
- Example 2: Display the last 5 lines of a file
  - `tail -5 Documents/user.txt`

## cut command
- Command is used for: extract specific section of each line of a file
- Formula: `cut + option + file(s)` 
- Example 1: List all users in your system
  - `cut -d ':' -f1 /etc/passwd`
- Example 2: List all users in your system with login shell
  - `cut -d ':' -f1,7 /etc/passwd`

## paste command
- Command is used for: join files horizontally in columns
- Formula: `paste + option + files`
- Example 1: Merge two files
  - `paste users.lst ip_address.lst`
- Example 2: Merge files using a different delimiter
  - `paste -d ':' users.lst ip_addresses.lst`

## sort command
- Command is used for: sorting files (alphabetically, reverse, number, and by month)
- Formula: `sort + option + file`
- Example 1: Sort a file
  - `sort Downloads/passwords.txt`
- Example 2: Sort a file with numeric data
  - `sort -n phonecalls.txt`

## wc command
- Command is used for: print number of lines, characters, and bytes in a file
- Formula: `wc + option + file(s)`
- Example 1: Display number of characters in a file
  - `wc -m users.txt`
- Example 2: Display number of lines in a file
  - `wc -l users.txt`

## tr command
- Command is used for: translating or deleting characters from standard output
- Formula: `Standard output | tr + option + set + set`
- Example 1: Translate white space into tabs
  - `cat program.py | tr "[:space:]" '\t'`
- Example 2: Translate tabs into space
  - `cat home.html | tr -s "[:space:]" ' '`

## diff command
- Command is used for: compares files and displays the differences between them
- Formula: `diff + option + file1 + file2`
- Example 1: Display the differences of two files
  - `diff cars.csv cars-backup.csv`
- Example 2: Display difference in column format
  - `diff -y program.py chess.py`

## grep command
- Command is used for: search text in a given file
- Formula: `grep + option + search criteria + file(s)`
- Example 1: Search any line that contains the word dracula regardless of case in file 
  - `grep 'dracula' ~/Documents/Books/dracula.txt`
- Example 2: Search any line that does not contain the word 'war' in file
  - `grep -v 'war' ~/Documents/Books/war-and-peace.txt`

## awk command
- Command is used for: processing and displaying text
- Formula: `awk + options + {awk command} + file + file to save (optional)`
- Example 1: First field of /etc/passwd file
  - `awk -F: '{print $1}' /etc/passwd`
- Example 2: Last field of /etc/passwd file
  - `awk -F: '{print $NF}' /etc/passwd`
- Example 3: First and last field with an ' = ' delimiter of /etc/passwd file
  - `awk -F: '{print $1," = ",$NF}' /etc/passwd`
- Example 4: Display the first and third field of /etc/passwd file
  - `awk -F: '{print $1,$3}' /etc/passwd`
- Example 5: Display starting from a given line (excluding lines)
  - `awk 'NR > 3 {print}' /etc/passwd`


## sed command
- Command is used for: search, find and replace, insert, and delete things from a file without opening them
- Formula: `sed + options + sed script + file`
- Example 1: Replace number of occurrences of a pattern in a file
  - `sed 's/pizza/rice/4' shopping-list.lst`
- Example 2: Replace all occurrence of the pattern in a file
  - `sed 's/pizza/rice/g' shopping-list.lst`
- Example 3: Replace from given number of occurrence to the rest in a file
  - `sed 's/pizza/rice/3g' shopping-list.lst`
- Example 4: Delete particular line 
  - `sed '5d' shopping-list.lst`
- Example 5: Insert one blank line after each line
  - `sed G shopping-list.lst`


