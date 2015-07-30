## What permissions are we talking about?

```
- r w x rwx r-x  1 codio codio   0 Jul 30 13:25 config.php
  r ead
  w rite
e x ecute
```

### Read, write and execute?

The following table shows what read, write and execute permissions mean for ordinary files and for directories:

|         | __File__                          | __Directory__                                |
|---------|-----------------------------------|----------------------------------------------|
| __Read__    | Can read the file             | Can list files in the directory              |
| __Write__   | Can edit the file             | Can create and delete files in the directory |
| __Execute__ | Can run the file as a program | Can change to the directory                  |

### What column relates to who?

There are 3 columns representing the **r**ead, **w**rite and e**x**ecute permissions:

The first _rwx_ column refers to the permissions of the __owner__.
The second _rwx_ column refers to the permissions of the __users group__.
The third _rwx_ column refers to the permissions of all the __other users__.

For example, the `whoami` command returns the current user: _codio_. That happens to be the same as the _owner_ of the item. 
The name of the group to which that item belongs to is _codio_ as well.