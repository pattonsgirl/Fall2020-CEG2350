# Lab 04 - NOT FINALIZED

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

## Part : Regular Expressions

regex tutorial - https://regexone.com/
Find stuff using /usr/share/dict/words
Different outputs in sed, pros and cons (in-place vs copy) - sed s/REGEX/SUBSTITUTION/ input.txt > input.txt why?


Write bash functions marco and polo that do the following. Whenever you execute marco the current working directory should be saved in some manner, then when you execute polo, no matter what directory you are in, polo should cd you back to the directory where you executed marco. For ease of debugging you can write the code in a file marco.sh and (re)load the definitions to your shell by executing source marco.sh.
Exercise from https://missing.csail.mit.edu/2020/shell-tools/