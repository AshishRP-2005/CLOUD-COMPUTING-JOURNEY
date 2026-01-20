## `usermod` command
- used to modify the user account

## Changing User Directory
- `sudo usermod -d /home/wayne batman`
  - `-d` = directory
  - `/home/wayne` = the directory you want to change to
  - `batman` = User Name
## Changing User shell
- default shell is `sh` called bourne shell
- `bash` = bourne again shell, it offers more freedom
- `sudo usermod -s /bin/bash joker` = changes user shell to `bash`

## Adding user to a group
- grouped users share same permissions
- `sudo` it is the group with admin privelleges
- `sudo usermod -aG sudo joker`
  - `-aG` = add to group without removing from other groups
  - `sudo` = the `sudo` that appears second time in the command is the group to which  `joker` is to be added
## To Switch User
- `su - joker` = changes from current user to `joker`
- to quit use command `exit`
## Locking and Unlocking User Accounts
- `sudo passwd -l joker` = locks user, doesn't aallow you to switch to the user  `joker`
- `sudo passwd -u joker` = unlocks user
## Deleting a User
- `sudo userdel -r joker`
  - `userdel` = as the name suggests deletes the user
  - `-r` = deletes home directory and mail spool
