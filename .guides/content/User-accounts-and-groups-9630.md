__Who is able to see or perform what in a computer system?__

One basic system administration task is to set up a user account for each user at a site. 

A typical user account includes the information a user needs to log in and use a system.

Lets get more details about our user:

```
# Get user group information and id:
codio ~/workspace $ id
```

By default, when a user is created on the UNIX CLI, it is assigned its own `/home/username/` directory and a group named after the chosen _username_.

### What is the importance of user groups?

When you set up a user account, you can add the user to a predefined group of users. A typical use of groups is to __set up group permissions on a file and directory, which allows access only to those users who are part of that group__.

For example, you might have a directory containing confidential files that only a few users should be able to access. 
You could set up a group called _confidential_ that includes the users that are working on the _confidential_ project. 
In addition, you could set up the _confidential_ files with read permission for the _confidential_ group. That way, only the users in the _confidential_ group would be able to read the files.