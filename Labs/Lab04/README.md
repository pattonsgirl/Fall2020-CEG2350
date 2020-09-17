# Lab 04

## Lab Procedure
Document your progress in a plain text file named `Lab04-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:
```
Name: Your name
Email: Your email

```

**Where questions are presented, answer them in your lab notes.  For each step, include the command you used to perform the direction or answer the question posed.**  If you did something "wrong" make a note of it in your lab.  These are learning experiences.

If you've lost or forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 1: Regular Expressions (5 pts)
1. Use the package manager `apt` to install a package named `wamerican`.  Write the command you used in your lab notes.
2. Verify `/usr/share/dict/words` exists.  If it does not, see if `/usr/dict/words` exists.
3. For the `grep` command, describe what the `-c` and `-i` options do. (1 pt)
4. For each below, write the `grep` command you used as well as the answer.
* How many words in the `words` file start with a vowel (uppercase OR lowercase)? (1 pt)
* How many words in the `words` file have the word `cat` inside of the word? (1 pt)
    * concatenate, for example, should be a match
* How many words in the `words` file have a non-alphanumeric character in the word? (1 pt)
    * ' , e with a hat are examples of non-alphanumeric characters
* How many words in the `words` file have at least one letter `m` in the word? (1 pt)

## Part 2: Scripting, Paths, and Arguments, Oh My! (4 pts)
1. Create a `Lab04` folder in your git repository in your AWS Educate environment.  Create a folder called `scripts`.  Inside that folder, create two scripts, one named `marco` and one named `polo`.  
2. When the command / script `marco` is run, it should save the current working directory in some manner.  Copy your working `marco` script into your lab notes. (1 pt)
3. When the command / script `polo` is run, it should `cd` you back to the directory where you executed `marco`.  Copy your working `polo` script into your lab notes. (1 pt)
4. Add the folder these scripts are located in to your `PATH`.  (2 pts)
* First use the `export` command in you terminal to test you have properly added to the `PATH`. Write this command in your lab notes. 
* Test that `marco` and `polo` can now be run in any directory.  
* Add your working `export` command to your home directory's `.profile`.

## Part 3: The Git Part (1 pt)
1. Create a `README.md` in your `Lab04` folder that provides a usage guide for `marco` and `polo`.  Copy the contents of you `README.md` into your lab notes.
2. Use `git` commands to `add`, `commit` and `push` the `Lab04` folder to GitHub.  Write the commands you used in your lab notes.

## Extra Credit (1 pt): 
For the `marco` script, when `marco` is run it should check if a path has already been "saved" and ask if the user would like to update the path.  Copy your extra credit `marco` script into your lab notes.

### Credits:  
Exercise based on https://missing.csail.mit.edu/2020/shell-tools/