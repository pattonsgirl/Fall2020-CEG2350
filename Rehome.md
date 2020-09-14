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

Scripting: ideas:
Find out what shell we are using in AWS.  Hint, read `/etc/passwd` (1 pt)
    * A guide on what is in [/etc/passwd](http://www.linfo.org/etc_passwd.html)
Run a file and check the permission bits

Write bash functions marco and polo that do the following. Whenever you execute marco the current working directory should be saved in some manner, then when you execute polo, no matter what directory you are in, polo should cd you back to the directory where you executed marco. For ease of debugging you can write the code in a file marco.sh and (re)load the definitions to your shell by executing source marco.sh.
Exercise from https://missing.csail.mit.edu/2020/shell-tools/

Debugging shell scripts w/ error messages or https://www.shellcheck.net/#

systems administration:
Create new user on system, create key pair for that user.  Use `sftp` to get the private key, log in as the new user just using ssh (no -i flag)

vim tutor
add customization to .vimrc (plugin, coloring, something)
regex tutorial - https://regexone.com/
Find stuff using /usr/share/dict/words
Different outputs in sed, pros and cons (in-place vs copy) - sed s/REGEX/SUBSTITUTION/ input.txt > input.txt why?

Late git:
Complete assigned sections of https://learngitbranching.js.org/
Fork and find a mistake / update / add another resource and create a pull request to course repo

Makefiles:
add git hooks so code must compile before a commit
Phony targets to avoid same names as targets? https://www.gnu.org/software/make/manual/html_node/Phony-Targets.html

Processes:
Use journalctl on Linux or log show on macOS to get the super user accesses and commands in the last day. If there aren’t any you can execute some harmless commands such as sudo ls and check again.

A common issue is that a port you want to listen on is already taken by another process. Let’s learn how to discover that process pid. First execute python -m http.server 4444 to start a minimal web server listening on port 4444. On a separate terminal run lsof | grep LISTEN to print all listening processes and ports. Find that process pid and terminate it by running kill <PID>.


Networking:
Find an online data set like this one, this one. or maybe one from here. Fetch it using curl and extract out just two columns of numerical data. If you’re fetching HTML data, pup might be helpful. For JSON data, try jq. Find the min and max of one column in a single command, and the sum of the difference between the two columns in another.
Difference between ifconfig and result of curl ipinfo.io

Download file with `wget`.  Convert to different file type.  Use `basename` to keep name but change extension

Sign a git commit
Encrypt and decrypt a file

(https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=CEG-2350&templateURL=https:%2F%2Fwsu-cecs-cf-templates.s3.us-east-2.amazonaws.com%2Fceg2350.yml)  