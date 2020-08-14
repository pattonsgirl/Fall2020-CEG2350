# Lab 2

## Lab Procedure
Document your progress in a plain text file named `Lab02-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:
```
Name: Your name
Email: Your email

```
## Part 1 - Paths
1. Write the full path to you key file and the command(s) you used to find it. (1 pt)
**Useful Commands: `pwd, ls, cd`**

## Part 2 - Directories, Files, and Permissions
For each step, include the command you used to perform the direction or answer the question posed.  If you did something "wrong" make a note of it in your lab.  These are learning experiences - writing them down will help you ask good questions later.
`ssh` in to your AWS environment.  If you've forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

#### A. Play with directories & naming (2 pts)
1. Create a directory called `Lab02`
2. In `Lab02`, create one directory called `DirA` and one directory called `Directory B`
3. What happens to the path name of `Directory B`?  Which of the folders uses a better naming convention?
4. Rename `Directory B` to `DirB`  
**Useful commands: `man, mkdir, cd, ls, pwd, mv`**

#### B. Create and edit a file (1 pt)
1. In `DirA`, create a file called `test.txt`
2. Put at least three lines of text in `test.txt` using `vim`
**Useful commands: `touch, vim`**

#### C. Play with hidden files (1 pt)
1. Make a copy of `test.txt`
2. Rename it to `.hidden.txt`
3. Type `ls`.  Can you see both files?  Use flags for `ls` to see your file.  
**Useful commands: `cp, mv, ls`**

#### D. Play with permissions (2 pts)
1. What are the permission settings for user, group, and other of the files in `DirA`?  What is the current  
owner and group name?  
2. Use `sudo` to make a copy of `test.txt` called `su-test.txt`
3. What are the permission settings for user, group, and other for `su-test.txt`?  What is the current  
owner and group name?
4. Can your user write to `su-test.txt`?  If not, how can you write to the file without changing the permissions? 
5. Change the file permissions so you can read and write to the file as your user (not using `sudo`).  
**Useful Commands: `chmod, chown, chgrp, ls, sudo, cp, cat`**

#### E. Play with hard links, soft links, and inodes (3 pts)
1. By default, what does `ln` followed by a filename do?  
2. Use `ln` to create a file named `hard.txt` from `test.txt`
3. Note the inode number of `hard.txt` and `test.txt`.  Are they the same?
4. Create a symbolic link called `sym.txt` from `hard.txt`
5. Note the inode number of `sym.txt`.  Is it the same as `hard.txt`?
6. Delete `test.txt`.  Is `hard.txt` and `sym.txt` still readable?
7. Delete `hard.txt`.  Is `sym.txt` still readable?  Why or why not?
8. Make a new file called `hard.txt` with some text in it.  Can `sym.txt` be read now?  Why or why not?
9. Move `hard.txt` to `DirB`.  Can you read `sym.txt`?
10. Delete `sym.txt`
11. Create a symbolic link from `hard.txt` in `DirB` to `newsym.txt` in `DirA`  
**Useful Commands: `ln, test, stat, cp, mv, rm`**

## Submission
Upload your file named Lab02-LastName.txt to the Pilot Dropbox.