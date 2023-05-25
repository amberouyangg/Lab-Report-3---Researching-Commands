### Researching Commands
Out of the commands less, find, and grep, I chose to research about the command 'find'.

### Command-line option 1:
```
-type
```
Source: <https://linuxize.com/post/linux-type-command/>
### Command Example: 
```
find ./technical -type d
```
This command is useful for finding all the directories inside the 
./technical directory and its subdirectories.
### Output:
```
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/government/About_LSC
./technical/government/Alcohol_Problems
./technical/government/Env_Prot_Agen
./technical/government/Gen_Account_Office
./technical/government/Media
./technical/government/Post_Rate_Comm
./technical/plos
```
### Command Example:
```
find ./technical -type l
```
This command would be useful for finding all the symbolic links inside the 
 ./technical directory and its subdirectories. However, since there is none inside the 
 ./technical directory, it doesn't return anything.
### Output:
```

```
### Command-line option 2:
```
-name
```
Source: <https://www.geeksforgeeks.org/find-command-in-linux-with-examples/#>
### Command Example:
```
find ./technical -name "*.txt"
```
This command would be useful for finding all the files with ".txt" in the ./technical directory.
### Output:
```
./technical/biomed/1471-2458-3-9.txt
./technical/biomed/1471-2466-1-1.txt
./technical/biomed/1471-2466-2-3.txt
./technical/biomed/1471-2466-2-4.txt
./technical/biomed/1471-2466-3-1.txt
./technical/biomed/1471-2474-2-1.txt
./technical/biomed/1471-2474-2-2.txt
./technical/biomed/1471-2474-2-3.txt
... etc.
```
### Command Example:
```
find ./technical -name "journal*"
```
This command would be useful for finding all the files in the 
./technical directory that start with "journal".
### Output:
```
./technical/plos/journal.pbio.0020001.txt
./technical/plos/journal.pbio.0020010.txt
./technical/plos/journal.pbio.0020012.txt
./technical/plos/journal.pbio.0020013.txt
./technical/plos/journal.pbio.0020019.txt
./technical/plos/journal.pbio.0020028.txt
... etc.
```
### Command-line option 3:
```
-mtime
```
Source: <https://www.hostinger.com/tutorials/linux-find-command>
### Command Example:
```
find ./technical -mtime -3
```
This command is useful for finding all the files in the 
./technical directory and its subdirectories that were modified within the last 3 days. 
### Output:
```
./technical/biomed/1471-2458-3-9.txt
./technical/biomed/1471-2466-1-1.txt
./technical/biomed/1471-2466-2-3.txt
./technical/biomed/1471-2466-2-4.txt
./technical/biomed/1471-2466-3-1.txt
./technical/biomed/1471-2474-2-1.txt
... etc.
```
### Command Example:
```
find ./technical -mtime +5
```
This command is useful for finding all the files in the 
./technical directory and its subdirectories that were 
modified more than 5 days ago. 
### Output:
```
./technical/biomed/1471-2458-3-9.txt
./technical/biomed/1471-2466-1-1.txt
./technical/biomed/1471-2466-2-3.txt
./technical/biomed/1471-2466-2-4.txt
./technical/biomed/1471-2466-3-1.txt
./technical/biomed/1471-2474-2-1.txt
... etc.
```
### Command-line option 4:
```
-samefile
```
Source: <https://www.computerhope.com/unix/ufind.htm>
### Command Example:
```
find ./technical -samefile ./technical/plos/pmed.0020281.txt
```
This command is useful for finding files with the same name as what was inputted after *-samename*.
### Output:
```
./technical/plos/pmed.0020281.txt
```
### Command Example:
```
find ./technical -samefile ./technical/government/En
v_Prot_Agen/bill.txt
```
This command is useful for finding files with the same name as what was searched 
for in the ./technical directory and the subdirectories, /government and 
/Env_Prot_Agen.
### Output:
```
./technical/government/Env_Prot_Agen/bill.txt
```
