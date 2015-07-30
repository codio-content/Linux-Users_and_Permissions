## What permissions are we talking about?

```
- r w x rwx r-x  1 codio codio   0 Jul 30 13:25 config.php
  r ead
  w rite
e x ecute
```

There are 3 columns representing the **r**ead, **w**rite and e**x**ecute permissions:

The first _rwx_ column refers to the permissions of the __owner__.
The second _rwx_ column refers to the permissions of the __users group__.
The third _rwx_ column refers to the permissions of all the __other users__.

The `whoami` command returns the _current user_ that happens to be the same as the _owner_ of the item.

### The `chmod` command

Currently, the `config.php` file is enabled with the _r_ and _w_ permissions for the owner user: _codio_. 

Lets update the `config.php` file permissions to be executable as well:

```
# ~/workspace directory
chmod u+x config.php
```