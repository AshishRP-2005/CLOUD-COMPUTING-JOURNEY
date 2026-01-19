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

Note 1 - since `chown` can effect system security `sudo` must be used to give it temporary admin access

Note 2 - `-p` flag used with `mkdir` allows for creation of sub-directories at the time of creation of new directory by specifying a path otherwise you will gave to `cd` into each directory and create the sub-directory

# Changing permissions of a file or directory
- use `chmod` - change mode function
## There are 2 methods
- ## Numerical method
  - here we use numerical notaction to change the permisssion. Wkt r = 4, w = 2, x = 1
  - we add the numerical values to give permission
  -  Example
     - `700` = rwx access to user, no access for group and everyone else
     - `542` = r-x access for user, r-- access for group, -w- access for everyone else
  - commands=
    - `sudo chmod 700 example.txt` - changes file permission to `-rwx------`
    - `sudo chmod 754 directory` - changes only directory permission to `drwxr-xr--`
    - `sudo chamod -R 745 directory` - changes the directory and its contents permission to `drwxr--r-x`
-  ## Symbolic method
    - ``
