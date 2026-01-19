# READING A PERMISSON
### The `ls -l` command is used to know the permission of a file or files and sub-directories inside a directory
### The `ls -ld` command is used to know the permission of the directory itself and not its commands

## BASIC INFROMATION TO KNOW
- `r` - file is in read mode, numerical value = 4, allows to see contents of a file or list contents of a directory
- `w` - file is in write mode, numerical value = 2, allows you to add new content to a file or add new files and sub-directories in a directory
- `x` - file is in execute mode, numerical value = 1, allows you to run program files or access files and sub-directories i.e `cd` into them
  
## Permission of a file
- `ls -l file1` - gives long format information about file1 including its permissions
- ### output
  - `-rwxrw-r-- 1 Ashish User 0 Jan 13 15:11 file1`
  -  the `-` at the start represent that it is a file
  -  the first `rwx` means the user can read, write and execute the file
  -  the secod `rw-` means the group can read and write the file
  -  the last `r--` means that everyone else can only read the file
  -  `Ashish` is user id, `User` is group id, `0` is number of bytes, `Jan 13 15:11` is last modified date, `file1` is file name
## Permission of a directory
- `ls -ld ~/dir` if you want permission of the directory itself
- `ls -l ~/dir` if you want permission of the content of the directory
- ### output
  - `drwxrw-r-- 1 Ashish User 0 Jan 13 15:11 dir`
  - `d` represents that it is a directory
  - All remaining information is the same as the file permissions

