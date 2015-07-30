|||definition
## Command: `chmod`
__Definition:__ Change the mode or access control of the listed files or directories.

__mode = permissions__

__Note:__ Only the owner of a file or the super-user is permitted to change the mode of a file.
|||

Remove the _owner user_ permissions to read, write and execute the `config.php` file and test the result with the `cat` command: 

```
chmod u-rwx config.php
```

Result: 

```
----rw-r-- 1 codio codio  0 Jul 30 13:24 config.php
```

Now, lets try to __read__ the file:

```
codio ~/workspace $ cat config.php
cat: config.php: Permission denied
```

Fortunately for us, we are the owners of the `config.php` file so we can add the file permissions back: 

```
chmod u+rwx config.php
```