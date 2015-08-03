The concept of system owners or c as _users_ has always been a security concern: 

__Who is able to see or perform what in a computer system?__

Unix, the operating system over which this CLI is built on, is one of those systems that rely its whole structure on user permissions. 

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