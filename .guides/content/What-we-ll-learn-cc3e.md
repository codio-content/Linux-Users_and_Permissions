## Time to understand the `ls -l` command output

We know that by adding the `-l` option to the `ls` command, the output displays more details about the files and directories in the current working directory. 

These details include: 

- Whether the item is a file or a directory
- The file or directory specific permissions
- The user who owns the file or directory
- The user group that is allowed to read, write or execute the item
- The size of the item
- The modification time of the item
- The name of the item

In this unit we will learn how to modify these specifications by understanding file and directory permissions as well as adding new users and groups.

### Why is this useful?

These file and directory specifications were created for security and organization reasons.

Web servers for example, are meant to be accessed by many users as well as other software, but there are certain types of files or directories that should not be publicly accessible.