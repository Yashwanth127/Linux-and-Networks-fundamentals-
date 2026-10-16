# Linux Basic Commands

## 1. pwd

Meaning: Print Working Directory

Shows the current directory where you are working.

Command:
pwd

Example:
pwd

Output:
/home/yashwanth


## 2. ls

Meaning: List

Shows files and folders in the current directory.

Command:
ls

Example:
ls


## 3. ls -l

Shows files and folders with detailed information.

Command:
ls -l

It shows:
- Permissions
- Owner
- Group
- File size
- Date
- File name


## 4. ls -a

Shows all files, including hidden files.

Command:
ls -a

Hidden files usually start with .


## 5. ls -la

Shows hidden files with detailed information.

Command:
ls -la

-l = detailed information
-a = hidden files


## 6. cd

Meaning: Change Directory

Used to move from one directory to another.

Command:
cd Documents

Go back one directory:

cd ..

Go to home directory:

cd ~

Go to root directory:

cd /


## 7. mkdir

Meaning: Make Directory

Used to create a new folder.

Command:
mkdir test

Create multiple folders:

mkdir folder1 folder2 folder3


## 8. touch

Used to create an empty file.

Command:
touch notes.txt

Create multiple files:

touch file1.txt file2.txt file3.txt


## 9. cat

Used to display the contents of a file.

Command:
cat notes.txt

Example:

echo "Hello Linux" > notes.txt
cat notes.txt

Output:
Hello Linux


## 10. less

Used to read a file page by page.

Command:
less notes.txt

Useful for large files.

Inside less:

Space = Next page
b = Previous page
q = Quit


## 11. cp

Meaning: Copy

Used to copy a file or folder.

Copy a file:

cp notes.txt backup.txt

Copy a file into another folder:

cp notes.txt Documents/

Copy a folder:

cp -r project backup_project

-r = recursive


## 12. mv

Meaning: Move

Used to move a file or folder.

Example:

mv notes.txt Documents/

It can also be used to rename a file.

Example:

mv old.txt new.txt

old.txt is renamed to new.txt.


## 13. rm

Meaning: Remove

Used to delete a file.

Command:

rm test.txt

Delete multiple files:

rm file1.txt file2.txt

Delete a folder and its contents:

rm -r project

Be careful with rm because deleted files may not be recoverable.


## 14. find

Used to search for files and directories.

Find a file:

find . -name "notes.txt"

. means current directory.

Find all .txt files:

find . -name "*.txt"

Find only files:

find . -type f -name "test.txt"

Find only directories:

find . -type d -name "project"


## 15. grep

Used to search for text inside files.

Example:

grep "Linux" notes.txt

If notes.txt contains:

Linux
Python
AWS
Linux commands

Output:

Linux
Linux commands

Case-insensitive search:

grep -i "linux" notes.txt

-i means ignore uppercase/lowercase differences.


## 16. |

Meaning: Pipe

Used to send the output of one command to another command.

Example:

ls | grep "txt"

First ls shows the files.

Then grep searches for txt in the output.

Another example:

ps aux | grep "python"


## 17. >

Used to redirect output into a file.

Example:

echo "Hello Linux" > notes.txt

This creates notes.txt and writes:

Hello Linux

Important:

> overwrites existing content.

Example:

echo "First" > notes.txt
echo "Second" > notes.txt

Now the file contains only:

Second


## 18. >>

Used to append content to a file.

Example:

echo "First" > notes.txt
echo "Second" >> notes.txt

Now the file contains:

First
Second

Important:

>  = overwrite
>> = append


## Quick Memory

pwd
→ Shows where I am.

ls
→ Shows files and folders.

ls -l
→ Shows detailed file information.

ls -a
→ Shows hidden files.

ls -la
→ Shows hidden files + detailed information.

cd
→ Changes directory.

mkdir
→ Creates a directory.

touch
→ Creates an empty file.

cat
→ Displays file contents.

less
→ Reads a file page by page.

cp
→ Copies files/folders.

mv
→ Moves or renames files/folders.

rm
→ Deletes files/folders.

find
→ Searches for files/folders.

grep
→ Searches for text.

|
→ Connects two commands.

>
→ Writes/overwrites a file.

>>
→ Appends to a file.
