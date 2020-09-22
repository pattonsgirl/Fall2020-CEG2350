# Lab 5 - NOT FINALIZED

## Lab Procedure
Document your progress in a plain text file named `Lab05-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:
```
Name: Your name
Email: Your email

```

Where questions are presented, answer them in your lab notes.  For each step, include the command you  
used to perform the direction or answer the question posed.  If you did something "wrong" make a note  
of it in your lab.  These are learning experiences.

Unless explicity stated, assume you should perform the lab assignment in your AWS Educate environment.  
`ssh -i /path/to/private/key ubuntu@ElasticIP`  OR `aws-ssh` assuming sucessful completion of Lab 04

If you've lost or forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 2 - Simple Makefile
**Sample Makefiles for Java and C are posted in this repo.  Click to view**
1. Copy your `Lab04` folder to `git/CEG2350/Lab05`.  Write the command(s) you used.
2. Edit the `README.md` file.  Your text can be:
```
Course work for CEG 2350 Spring 2020
```
3. Check the `status` of your git repository.  Write the command you used and any output.
4. Commit and push the folder `Lab05` and its contents to your git repo.  Write the command(s) you used.
5. In `Lab05` create a file called `Makefile`.  Write the command you used.
6. Write contents in `Makefile` so that in the shell the following commands perform the following actions:
    * `make` will compile the program and create an executable version
    * `make run` will compile and execute the program
    * `make clean` will delete the compiled program
7. Copy the contents of your `Makefile` into your lab notes.
8. Commit and push your `Makefile` into your git repo.  Write the command you used.

## Submission
Upload your file named `Lab05-LastName.txt` to the Pilot Dropbox.