# Comparison of the content in differernt files

## diff command
- the diff command is used to compare content in 2 different files
- [ diff file1 file2 ] - compares content between the 2 files
- ## example output
  - 1c1 - this means first line of file1 and first line of file2 is different
  - `<` this is file1 - this line exists in file1
  - `------` - separator
  - `>` this is file2 - this line exists in file 2

# Comparison of Directories
## command used is - [ diff -r ~/Directory1 ~/Directory2 ]
- compares the folder structure and file content in the 2 directories
- ## output
  - only in directory 1 /folder/file - the particular sub directory or file is only present in the specified directory
  - files....  and .... differ - similiar named files exist in both directories but their content is different 
  - no output - both directories are identical
## note 
- [ -r ] - this flag must be used when comparing directories otherwise it will only compare the names of the directory and wont dive into the sub-directories and files present in the directories
- [ diff -rq dir1 dir2 ] - the `-q` flag called brief flag is used to get which line by line changes are needed to make both directories the same
