## Part 2 - Log in to your AWS Educate environment:  


1. Run `sudo apt update` - in your lab notes, explain what update does
2. Run `sudo apt upgrade` - in your lab notes, explain what upgrade does
3. Run `sudo apt autoremove` - in your lab notes, explain what autoremove does  
**Useful commands: `man, apt, sudo`**

3. The remainder of this section will deal with theorical questions since we can't go to AWS in person.
    * There are two steps related to resizing partitions - list them.
        * Note the process to *expand* a filesystem.
        * Note the process to *shrink* a filesystem.
        * *Hint*: You can use Google, or you can look at the usage guide for `resize2fs`
    * Let's say we can go to AWS and plug in a brand new hard drive that is 8TB in size.  Assume that when the drive  
    is plugged in, the drive name is `/dev/sdb`
        * What partition table should we select?  Why?
        * What command(s) / program(s) can we use to create a partition table on our new drive? 
            * Note the command and its parameters
        * What command can we use to create a filesystem on our partition?
            * Note the command and its parameters
    * Let's assume the above went well.  Write the command to mount the drive to `/mnt/Lab03`
        * If we wanted to make this permanent, what file would we need to edit?