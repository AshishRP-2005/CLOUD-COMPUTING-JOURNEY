# REMOVING FILES

[rm file.txt] - removes file.txt

[rm -i file.txt] - asks confirmation before removing the file, if y is entered it removes the file if anything else is entered action is cancelled

# REMOVING DIRECTORIES 

[rm directory] - for this command to work the directory mus be empty, i.e there should be no files in the directory

[rm -r directory1] - this command is used when there are files in the directories it uses recursion to move through each file and subdirectory to delete them

[rm -rf directory] - this command is dangerous it forcefully removes the directory, if you have access you can even delete system files, use with caution

- note : [ls -R directory] - this command is used to list the content of the directory in recursive order, i.e even sub directories are listed
