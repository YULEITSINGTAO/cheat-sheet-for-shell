# Cheat Sheet For Shell
This is a shell cheat sheet to help user
# Basic introduction for Unix system
- File's extension is not important in Unix system

# Filename Reminders

- Case MaTTerS
- File Extensions (e.g. .txt .doc .docx) don't matter
- Avoid spaces in filenames
- Files starting with '.' are hidden by default
- Backup files created by some editors will be appended with ~

# commond 
## Cat: 
- `cat filename` can directly show you the content of your file. 
- `cat filename1 filename2 > newfile` can put two files into one file
- `cat filename1 >> newfile` add filename1 into the end of newfile
- `cat filename1 > newfile` replace the content in newfile using filename

## Sudo (Super User do)
- `sudo su` can make you switch to super user, which has 100% authority.

## Touch
- `touch` used when you just want to creat files but not edit them

## Find
- `find . -maxdepth 1 -type f/d -iname "name.txt" -size ` is used to find the file `"name.txt"`.
- `find . -maxdepth 1 type f/d not -iname "name.txt" -size ` is used to find the file is not named `"name.txt"`.

## Grep
- `grep "keywords" file` is used to find the words in the file
- `grep -i "keywords" file` is used to find the words in the file but not care about case
- `grep -n -i "keywords" file` is used to find the words in the file but not care about case and give you the line's number

## Combine find and grep to do search
- `find . -maxdepth 1 -type f/d -iname "name.txt" -exec grep -i -n "function" {} +`




