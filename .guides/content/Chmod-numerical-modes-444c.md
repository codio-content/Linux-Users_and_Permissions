When working with software such as a CMS, you’ll probably find file mode definitions described as numbers. eg. `755`, `777`, `644`, and so on.

These are numerical representations of file and directory permissions.

Let's understand this by examining the following comparison:

```
# String permissions for the .htaccess file:
-rw-r--r--  1 codio codio  233 Jul 30 13:32 .htaccess
```

In order to assign the `rw-r--r--` permissions to the `.htaccess` file, the command would be like:

```
# Commas for faster assignment:
chmod u+rw-x,go+r-wx .htaccess
```

### Using numerical modes:

Using string mode definition to define _who_ is able to read, write or execute files requires a lot of typing. 

The `.htaccess` file mode can also be updated by doing: 

```
# Numerical file mode definition:
chmod 644 .htaccess
```

Want to know how this works? Continue on the next section.