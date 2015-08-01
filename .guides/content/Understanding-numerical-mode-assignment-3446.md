The following table explains how numerical file modes work:

![chmod-modes](.guides/img/chmod-modes.png)

The `read` permission has a value of __4__ that adds to the value of __2__ of the `write` permission and the `execute` permission has a value of __1__. This value assignment applies for each of the _who_ modes: _user, group, others_. 

### Changing permissions to subdirectories

Lets change the mode of the `~/workspace/content` directory and its subdirectories to be `755`:

```
# Add the -r ecursive option
chmod -r 755 content/
```

By adding the `chmod -r` option, _bash_ uses the _recursive strategy_ to change the modes of the file hierarchies and not just the directory itself. 

### Why `755`?

We gave the `content/` directory and subdirectories the `rwxr-xr-x` permissions for the CMS system to be able to list the files as well as enabling file uploads and edits. 