# Lab 4 - NOT FINALIZED

## Lab Procedure
Document your progress in a plain text file named `Lab04-LastName.txt`  
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
`ssh -i /path/to/private/key ubuntu@ElasticIP`  

If you've lost or forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 1 - Processes
**Log in to your AWS Edu environment:**

1. Craft a command that snapshots processes being run by and for your user, `ubuntu`
    * Note: you need to use to correct flags to see all process being run.
    * Helpful commands: `grep, ps, |`

2. `sleep` is a neat command that creates a process that does nothing for the amount of time specified.  I very  
much recommend reading through the rest of this section before performing it.
    * Run a `sleep` command that runs for 5 minutes.  Can you enter anything?  Do **not** exit the terminal or  
    press `Ctrl+C`
    * Since we have remote access to this machine, we can open *another* connection to AWS to see what is going on.  
    Open another terminal and connect to AWS.  
        * What does `ps l` show us?
    * `kill` the `sleep` command running in the other terminal using its process ID.
    * Switch to the terminal you wrote the `sleep` command in.  Is there a message there?
    * Run the command again, but this time set it to run in the background.
    * Use the job ID to bring it back to the foreground, and send a signal to terminate it with `Ctrl+C`

## Submission
Upload your file named `Lab04-LastName.txt` to the Pilot Dropbox.