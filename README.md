#Git Helpers

These scripts are useful for making git in a local servers, adding users to it and make it upload each changed file to public server's ftp after merge.


#How to install

Just copy all files to `/usr/local/bin/` and make them executable
```
chmod +x make-git
chmod +x ftp-git
chmod +x delete-git
```
and you are done.

#How to Use

1- to create a new repository, use `make-git Project-name Existing-user1 Existing-user2 ...`

example: `make-git testproject masih`
note that 'masih' should be a valid user in your operating system

-

2- to add ftp data to a repository, use `ftp-git Project-name FTP-Host FTP-User FTP-Password`

example: `ftp-git testproject ftp.example.com user@example.com somepassword`

-

3- to delete a repository, use `delete-git Project-name`

example: `delete-git testproject`