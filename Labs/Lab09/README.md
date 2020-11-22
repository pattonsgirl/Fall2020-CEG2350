# Lab 09 - NOT FINALIZED

## Lab Procedure

Document your progress in a plain text file named `Lab09-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:

```
Name: Your name
Email: Your email
```

**Where questions are presented, answer them in your lab notes. For each step, include the command you used to perform the direction or answer the question posed.** If you did something "wrong" make a note of it in your lab. These are learning experiences.

If you've lost or forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 1: Makey Makey

Needing to install a package from source is not an uncommon request. You are going to install an OwnCloud server on your AWS Educate instance. OwnCloud is essentially an open source version of DropBox or Office365.  
Note: You may **not** use the package manager (`apt`).

1. Download the APR
2. Unpack the installation files
   - Useful commands: `gzip`, `tar`
   - Note: you will need flags for the above commands
3. Look in the unpacked directory. Is there a `Makefile`? Run the `configure` script. Is there a `Makefile` now?
4. Use the `Makefile`.
5. Download the apache HTTP server installation files
   - Useful commands: `wget`
6. Check the signature on your downloaded file and compare it to the official signature from the site.
7. Unpack the installation files
   - Useful commands: `gzip`, `tar`
   - Note: you will need flags for the above commands
8. Go into the directory.

## Part 2: SSH

1. On your local machine, use one of the SSH clients you have installed:

- WSL 2
- MobaXterm + cygutils

2. Configure /etc/hosts
3. Configure ~/.ssh/config
4. In your client of choice, create a new key pair
   - Note: use the defaults (ie. ~/.ssh/id_rsa)
5. Copy your public key into the `authorized_keys` file on your AWS system.
6. SSH from your local machine to the AWS machine

## Part 3: Getting Zippy

Zip two labs, use sftp to transfer to local system.

## Part 4: Conflict Managment

1. Switch to the `development` branch

## Submission

Upload your file named `Lab09-LastName.txt` to the Pilot Dropbox.
