# Changing Ownership
Owner can change the permission of the file or directory

## Use command `chown`
### Changing Ownership of file
 - better to understand with an example
 - ## Example
   - `-rw-r--r-x 2 Ashish User 23 Jan 14:11 Example.txt` - here the owners are Ashish{user}  and User{group}
   - `sudo chown Poojitha:root Example.txt` - now we changed the user to Poojitha and group to root
   - `-rw-r--r-x 2 Poojitha root 23 Jan 14:11 Example.txt` - when `ls -l Example.txt` is used this will be the output

### Changing Ownership of directory
  - `mkdir -p new/dir` - creates a new directory called new with sub directory dir
  - `sudo chown root:User new` - this will only change the ownership of the directory and not its contents
  - `sudo chown -R root:User new` - changes ownership of the directory and its content because of the recursive flag  `-R`
