# ADDING USERS
- we use `sudo` for all commands related to user management because without admin access linux will deny any changes regarding user management
## `useradd` command
- used to create a new user
- `sudo useradd joker` = creates a user called joker but doesn't create a home directory for it
- `sudo useradd -m batman` = creates a user called batman with a home directory called batman { because of the `-m` flag }
## Verifying user existence
- `sudo grep -w 'joker' /etc/passwd` = command used to check if the sepecified user exists
   - `grep` = text search tool, it checks for a patter and prints it
   - `-w` = tells to check for whole word
   - `'joker'` = the word that needs to be searched
   - `/etc/passwd` = this is the phonebook for user accounts
   - output - `joker:x:5001:5002::/home/joker:bin/sh`
     - x = secure password that is stored elsewhere
     - 5001 = uid
     - 5002 = gid
     - /home/directory = home directory
     - bin/sh = default shell
## Verify Home Directory
- 
