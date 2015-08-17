The following table explains how numerical file modes work:

![chmod-modes](.guides/img/chmod-modes.png)

Take a look at the _user_ row. 
The __total value of 7__ which equals to the _rwx_ permissions for the _user_ type, is equal to the sum of the _read_, _write_ and _execute_ permissions __permanent values__. Meaning that _read_ will always have a value of 4, _write_ a value of 2 and _execute_ a value of 1.

In the other hand, `-` represents 0. 
This is why the value of the user _group_ permissions equals to 5, where the _write_ permission is not required.

### Changing permissions to subdirectories

Let's change the mode of the `~/workspace/content` directory and its subdirectories to be `755`:

```
# Add the -r ecursive option
chmod -R 755 content/
```

By adding the `chmod -R` option, _bash_ uses the _recursive strategy_ to change the modes of the file hierarchies and not just the directory itself. 

### Why `755`?

We gave the `content/` directory and subdirectories the `rwxr-xr-x` permissions for the CMS system to be able to list the files as well as enabling file uploads and edits. 