# Lab 3 - NOT FINALIZED

## Lab Procedure
Document your progress in a plain text file named `Lab03-LastName.txt`  
where LastName is your last name

At the top of the file please enter your personal details as follows:
```
Name: Your name
Email: Your email

```

For each step, include the command you used to perform the direction or answer the question posed.  If you did something "wrong" make a note of it in your lab.  These are learning experiences - writing them down will help you ask good questions later.

`ssh` in to your AWS environment.  If you've forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.

## Part 1 - Self Discovery
Find out the following information about your personal system.  List the command(s) or website(s) you used to collect this information.
1. BIOS version / mode.
2. Installed memory size.
3. Virtual memory size.  Does you system have a pagefile or a swapfile?  What does this mean?
4. File system on installed disk(s).
5. Number of partitions.  Which partition is your primary partition?

## Part 2 - Exploring the File System
`ssh` in to your AWS environment.  If you've forgotten your key, you'll need to provision a new stack in AWS Educate and create a new key.  
See [Remaking your AWS Educate environment](../../..) for instructions.
1. In AWS, read `/boot/grub/menu.lst`.  According to this file, what options would the grub menu present?  
2. In AWS, run `sudo parted -l`
    * What is the primary disk in the `/dev` folder?  
    * What type of partition table is our AWS environment using? 
        * Hint: If it looks unfamilar, use Google to find the common name
    * How many Gigabytes (GB) of storage do we have?
    * Use `df -T` to find out the file system used by this device.  
    * Hint: What is the top of the Linux directory structure?
3. Use `df -h`
    * How much space is used and how much space is free?
4. [Set file system of partition] Run `parted` on the disk (use the answer you found in Part 1-3)
    * How can you view the options for `parted`?
5. [Mount partition]
6. [Add partition to /etc/fstab]

## Submission
Upload your file named `Lab03-LastName.txt` to the Pilot Dropbox.