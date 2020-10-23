# Lab 08 - NOT FINALIZED

## Lab Procedure

Document your progress in a plain text file named `Lab08-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:

```
Name: Your name
Email: Your email

```

**Where questions are presented, answer them in your lab notes. For each step, include the command you used to perform the direction or answer the question posed.** If you did something "wrong" make a note of it in your lab. These are learning experiences.

If you've lost or forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 1: Good listening

Create a process that output / echos message over a port

## Part 2: Getting Zippy

Zip two labs, use sftp to transfer to local system.

## Part 2: [/insert AOL noises here/](https://www.youtube.com/watch?v=D1UY7eDRXrs) (3pts)

For your local system, identify the following information regarding your network connection:

1. Network interface
2. MAC address
3. IP Address
4. Subnet mask
5. Gateway  
   Q. According to the settings above and some defaults discussed in class, are you on a private network? Based on that answer, how do you communicate to the "world" (google.com, wright.edu, etc.)?
6. Type `host` followed by the URL of your favorite website.  
   Q. Copy the command and its results into your lab write up. What can you infer? Do the reverse, `host` followed by the IP address given by the results. Is your favorite website likely hosted on a single system, or is a single system likely serving multiple websites?

## Part ?:

Difference between ifconfig and result of curl ipinfo.io
A common issue is that a port you want to listen on is already taken by another process. Let’s learn how to discover that process pid. First execute python -m http.server 4444 to start a minimal web server listening on port 4444. On a separate terminal run lsof | grep LISTEN to print all listening processes and ports. Find that process pid and terminate it by running kill <PID>.

## Submission

Upload your file named `Lab08-LastName.txt` to the Pilot Dropbox.
