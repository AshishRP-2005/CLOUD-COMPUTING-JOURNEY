# Print File Content

## To view Complete Content
- [ cat /tmp/hello ] - {concatenation} used to display contents of a file, here from the file hello of the temporary directory
- [ cat -n /tmp/hello ] - this gives the number of the line as well when printing the contents of the file

## To View the top lines
- [ head /tmp/hello ] - outputs the first 10 lines of the content in the files
- [ head -n2 /tmp/hello ] - outputs the first 2 lines of the content, based on the number after n lines are printed
- [ head -c2 /tmp/hello ] - outputs the first 2 bytes of the content, 1 byte = 1 character so basically the first 2 characters are outputed, based on the number afte C characters are printed

## To view last lines of content
- [ tail /tmp/hello ] - prints last 10 lines
- [ tail -n3 /tmp/hello ] - based on number after -n that many lines at the end are printed, here last 3 lines are printed
- [ tail -c3 /tmp/hello ] - based on number after -c that many bytes from the end of the content in the file are printed, here last 3 characters{bytes} are printed

## Notes
- /tmp - this is called as temporary directory and part of tmpfs {temporary file system}, the directory is cleared when the computer reboots
- tmpfs - file storage that uses RAM to be super fast
- [ df -h | greg tmpfs ] - to check for what the tmpfs is being used in the system
