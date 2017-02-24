The following table explains how numerical file modes work:

![chmod-modes](.guides/img/chmod-modes.png)

Take a look at the _user_ row. 
The __total value of 7__ equals the `rwx` permissions for the _user_ type and is the sum of the _read_, _write_ and _execute_ permission permanent values. 

_read_ will always have a value of `4`, _write_ a value of `2` and _execute_ a value of `1`.

On the other hand, `-` represents 0.

This is why the value of the user _group_ permissions equals to 5, where the _write_ permission is not required.

### Changing permissions to subdirectories

If we wanted to change the mode of the `~/workspace/content` directory (if it existed) and its subdirectories to be `755`:

```
# Add the -R ecursive option
chmod -R 755 content/
```

By adding the `chmod -R` option, _bash_ uses the _recursive strategy_ to change the modes of the file hierarchies and not just the directory itself. 

### Why `755`?

We gave the `content/` directory and subdirectories the `rwxr-xr-x` permissions for the CMS system to be able to list the files as well as enabling file uploads and edits. 