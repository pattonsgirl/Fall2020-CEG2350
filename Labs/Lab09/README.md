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

Needing to install a package from source is not an uncommon request. You will be installing Wireshark from source on your AWS Educate Instance.
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

In a previous lab, you made a key pair on your AWS system and used it to create a passwordless authentication with GitHub. You have also created an ssh alias so that you can use a shortcut command instead of typing out your ssh connection everytime. Now you are going to create an ssh key on your local system, and use this new key to get into your AWS system.

1. On your local machine, identify what method you have been using to ssh in to your AWS system. This is your client. Consistentcy will be important here, especially for Windows users. Are you using Moba + Cygutils? WSL2? For Mac / Linux users, have you been using a local terminal?
2. Create a new ssh key on the client. Use the default directory / names. Do not enter a passphrase when prompted (just hit `Enter` to skip it). Write the command you used.
3. Copy the contents of the public key file to `/home/ubuntu/authorized_keys` on your AWS Educate instance. Write your process.
4. Log out, and `ssh` to your AWS educate system with your private key (not the private key you got from AWS). Write the command you used.

## Part 3: Getting Zippy

Zip two labs, use sftp to transfer to local system.

## Part 5: The Git Part (1 pt)

1. Create a folder in your repository called `Lab09`. Create a file called `README.md`. Copy and paste your lab notes into the file. `add`, `commit` and `push` your file to remote.

## Extra Credit: G@M3R

Install ninvader from the package above. For credit, you need to list how you installed ninvaders succesfully. Since it is a text based C language game, you will need an additional library in C, called `ncurses`.  
Note: You may use the package manager (`apt`) to install the ncurses library, but you may **not** use the package manager (`apt`) to install ninvaders.

## Submission

Upload your file named `Lab09-LastName.txt` to the Pilot Dropbox.
