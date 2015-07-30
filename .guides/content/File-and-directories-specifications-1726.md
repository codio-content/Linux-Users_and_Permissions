## Understanding the `ls -l` command output

On the terminal, get a detailed list of the `~/workspace` directory content. Include hidden files, human readable sizes and file type symbols as well:

```
ls -ahFl
```

__NOTE:__ We are excluding the `.git/` and `.guides/` on the examples.

### A closer look at the output

The easiest way to interpret the command output is as columns:

![ls-l-cmd-output](.guides/img/ls-l-cmd-output-row.png)

Lets understand the permissions concept by actually changing the permissions.