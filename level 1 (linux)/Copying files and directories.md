#COPYING FILES

[cp file.txt file2.text] - new file called file2.txt is created and contents of file.txt is copied to file2.txt

[cp file.txt directory/] - copies the file.txt into the specified directory under the same name

#COPYING DIRECTORIES

[ cp -r testdir testdir_copy ] - Creates a new directory called testdir_copy and copies contents of the testdir to it using the recursive flag {-r]

##note :  -r recursive flag/option must be used for the directory to be copied or else it wouldnt work, cuz without recursion copy wouldnt descend into the complete tree {copy by default only copies files}
