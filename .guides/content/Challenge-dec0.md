## Changing file permissions

So far, we've learned that the `ls -l` command option returns details for files and directories regarding its type, mode or permissions, size, modification time and name.

File modes may be updated with the `chmod` command which accepts the _mode_ definition by using the: `ugo`, letters for _user, group and others_ respectively. The operands `+-` determine whether to add or remove the _read, write or execute_ modes.

{Check It!|assessment}(test-1413942323)

|||guidance
### Correct answers
1. `ls -alh`
2. `chmod u-w,g-rw+w,o-rwx index.php`
3. `chmod u-rx+w,go+rw-x admin`

|||