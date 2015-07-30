The `whoami` command returns the _current user_ that happens to be the same as the _owner_ of the item.

### The `chmod` command

Currently, the `config.php` file is enabled with the _r_ and _w_ permissions for the owner user: _codio_. 

Lets update the `config.php` file permissions to be executable as well:

```
# ~/workspace directory
chmod u+x config.php
```