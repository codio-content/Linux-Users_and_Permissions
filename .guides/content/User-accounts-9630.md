The concept of system owners or commonly known as _users_, has always been a security concern.

__Who is able to see or perform what in a computer system?__

One basic system administration task is to set up a user account for each user at a site. A typical user account includes the information a user needs to log in and use a system, without having the system's root password.

Lets get more details about our user:

```
# Get user group information and id:
codio ~/workspace $ id
```

By observing the results of this command, the `ls -l` command output gets an immediate association with the `uid` (_user id_ and username) and the `gid` (_group id_ and default group name) and how our `/home/codio/workspace` files belong to the _codio_ user. 

### Adding users

Now that we know how to get the user details, lets add a new user: 

```
# The command name is pretty straight forward:
codio ~/workspace $ useradd admin
```