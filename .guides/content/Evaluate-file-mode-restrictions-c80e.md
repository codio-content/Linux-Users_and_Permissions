The current configuration for the `config.php` file is:

```
-rwxrw-r-- 1 codio codio  0 Jul 30 13:24 config.php
```

Let's remove the __write__ permissions for the owner user:

```
chmod u-w config.php
```

And try to _write_ something into it by using the `echo` command:

```
codio ~/workspace $ echo "<php ?>" > config.php
-bash: config.php: Permission denied
```

### Permissions on the real world
In a real-world example, the `config.php` file may contain the CMS database name and password. This kind of information needs to be well-protected from anyone that is not the system administrator. In this case the `config.php` file settings would probably look like this:

```
-rwxr-x--- 1 admin sysadmin  0 Jul 30 13:24 config.php
```