## Searching for files and within files is useful

In the previous unit, we experienced many practical examples of how the `grep` and `find` commands interact with the content and the file hierarchy respectively. 

We began by _redirecting the stdout_ with the `>` symbol to create new files with the output of a certain command like `echo`, `ls`, among others. 

By using the `>>` utility, we learned how to concatenate or append content to a file. For instance, the `cat` command helped us on reading and appending content into a certain file. 

### Commands are getting more complex, but more useful as well

As the `grep` and `find` examples became more complex, we learned that they work with __operands__. Operands are different to _command options_ in the way that they accept their own parameters which act upon the main _argument_.

We implemented more options to the `ls` command to display even more information about the directory content and learned how `grep` can  compare the content of two or more different files and return their differences or similarities.

### Searching the command history

The `.bash_history` file stores all the commands that are input on any shell session. By using the `ctrl + r` keyboard shortcut, we can access that file as a way of finding previously executed commands. 