## The `chmod` command

Currently, the `config.php` file is enabled with the `r` and `w` permissions for the owner user, _codio_: 

```
-rw-rw-r--  1 codio codio   0 Jul 30 13:25 config.php
```

Let's update the `config.php` file permissions to be executable as well, meaning that the file can be run as a program:

```
# 'u' for owner user, '+' for adding, 'x' for the execute permission:
chmod u+x config.php
```

The output of the `ls -l` command should have been updated to: 

```
-rwxrw-r-- 1 codio codio  0 Jul 30 13:24 config.php
```

Can you tell the difference? 