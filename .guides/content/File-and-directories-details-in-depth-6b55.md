![ls-l-cmd-simple](.guides/img/ls-l-cmd-output-simple.png)

Lets inspect 5 items only: 
The `./` current directory, the `../` parent directory, the `admin/` directory, the `config.php` visible file and the `.htaccess` hidden file respectively.

### Column 1
Represents the item with a `d` if it is a __directory__ or writes a `-` if the item is a __file__ instead.

### Column 2
Represents the **r**ead, **w**rite and e**x**ecute permissions of __the owner__ over the item. The item owner, better known as user, is represented in column 6: _codio_.

### Column 3
Represents the __rwx__ permissions for __the users group__ over the item. A user group is a collection of users registered on the system. More on this later.

### Column 4
Represents the __rwx__ permissions for __others__ over the item. _Others_ may be random people trying to access the content of the file through the internet or a certain program trying to write into the directory or execute file content.

### Column 5
Represents the number of the item _hard links_. A hard link is essentially an item either on the current directory or on a different directory that is linked to the contents of the original item. _This column and feature is not used most of the time_. 

Continue on the next page.