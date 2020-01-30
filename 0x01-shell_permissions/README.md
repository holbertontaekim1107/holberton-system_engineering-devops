README.md file for 0x01. Shell, permission.

0.su - command to change your user ID.
1.whoami - command to print the effective userID of the current user.
2.groups - command to print all the groups the current user is part of.
3.chown [user] [file] - command to change owner of the [file] to the [user]
4.touch [file] - command to create [file]
5.chmod u+x [file] - command to add execute permission to the owner of the [file]
6.chmod ug+x,o+r [file] - command to add execute permission to the owner and the group owner, and read permission to other users, to the [file]
7.chmod a+x [file] - command that adds execution permission to all users, to the [file]
8.chmod 007 [file] - command that sets permission to the [file], owner-no permission, group- no permission, other-all permission
9.chmod 753 [file] - command  that sets the mode of the [file] in relation to -rwxr-x-wx
10.chmod --reference=[file1] [file2] - command that sets the mode of the [file2] the same as [file1]'s mode
11.chmod -R a+x */ - command adds execute permission to all subdirectories of the current directory for all the users.
12.mkdir -m=751 [directory] - command that creates a [directory] with permissions 751 in th working directory.
13.chown [owner] [file] - command that changes group [owner] for the [file]
14.chown -R [owner]:[group owner] . - command to change [owner] and [group owner] for all files and directories in working directory.
15.chown -h [owner]:[group owner] [file] - command to change the [owner] and [group owner] of the [file]
16.chown --from=[user] [owner] [file] - command to change the owner of the [file] to [owner] only if it is owned by the [user]

Extra notes
-rwxrwxrwx = - stands for files.
drwxrwxrwx = d stands for directories
-rwx rwx rwx = first set of rwx stands for owner/user
     	     = second set of rwx stands for group owner
	     = third set of rwx stands for othes.
r=reading
w=writing
x=execute

r numeric value=4
w numeric value=2
x numeric value=1

rwx rwx rwx = 111 111 111
rw- r-x --x = 110 101 001
1= on (permission)
0= off (permission)