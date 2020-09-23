# Quiz 2

1. Write a command that will give read and write permissions to anyone on the system / others for a file named readme.txt
* `chmod o+rw readme.txt`

2. The _____ command, when run on a file, will show information such as the inode number, how many links exist to the file, and the path to the hard link (if the file is actually a symbolic link).
* `stat`

3. When used in a regular expression, what is the difference between a * and a + ?
* A `*` matches 0 or more of the pattern specified.  A `+` matches 1 or more of the pattern specified.  So a regex of `t*` would match 0 or more instances of t; a regex of `t+` would match 1 or more instances of t

4. The ____ environment variable, in both Linux and Windows, holds a record of directories to access installed programs, including compilers.
* PATH

5. T/F alias commands are stored in the .git configuration file.
* False.  `alias` commands should be placed in the `.bashrc` or `.bash_profile` file.  The `.git` is a folder that hold git configuration information for a given repository.

6. The following command is run:
```
echo '$PWD' > output.txt
```
What are the contents of output.txt?
* `output.txt` would have the literal words `$PWD` in its contents, nothing else.  The single quotes force a literal iterpretion of the text inside.  

7. To run a script with the bash interpreter, what line needs to go at the top of my script file?
* `#! /bin/bash` needs to be at the beginning of the script to specify usage of the bash language interpreter

8. If I create new files in a git repository, I need to use a git _____ command to have git track them.
* `add` (also accepted `git add`) followed by the specific files or a wildcard (*) to add them for git to track.

9. Given the command below, write a script that echos the second argument.
```
runme.sh bananas oranges
```
* Script contents:
```
#! /bin/bash
echo $2
```
