## Written answer:

1. What is the role of the PATH environment variable?

   - PATH is an environment variable that stores directories to commands & programs installed on the system. Once a directory is listed in PATH, PATH can use the path to the directory when a command / program is typed into the terminal.

2. What is the difference between a hard link and a copy of a file?

   - Copy has a different inode than the original file, and data is stored independent of the original (a change I make in one is not in the other). Hard links have the same inode (a change in one is also done on the other)

3. Given the file below, write all implications of the permissions for the file.

```
dr-x-w-r-- bob sue test
```

- d is for directory.
- User is bob, bob can read and execute.
- Group is sue, sue can write.
- Other can only read.
- Name of the directory is test.

4. Assuming a brand new disk is plugged into a system, what structures does the disk need created for my OS to use it for data storage?

   - Partition table (MBR or GPT)
   - One of more partitions
   - A filesystem on the partition
   - Partition with filesystem should be mounted to OS filesystem structure.
     - Linux: mount & /etc/fstab
     - Windows: drive letters

5. Given the following Makefile, what action is associated with the target go?

```
go: code.c
     gcc -Wall -o runme code.c
```

    - The target compiles a c program called 'runme' from a source code called 'code.c'

6. For the regular expression: `^(\D{3}\s(\d{4}))$`  
   Describe what the regular expression can match, then create an example that would and an example that would not match the expression.

   - Matches 3 non-digit characters, followed by a whitespace character (a space, a tab, or a Windows or Linux new line), followed by 4 digit characters (0 - 9). The ^ indicates it must start with the pattern, and the \$ indicates it ends with the pattern.
   - Example match: `abc 5678`
   - Example fail: `456 ands`

7. Describe the role of virtual memory.

   - Virtual memory is the idea of offsettings hardware memory limitations of RAM with disk space. RAM can then offload inactive memory for processes and recall it later from the disk. In Linux, this part of the disk is called the swap table. In Windows, using the disk for this purpose is called paging.

8. Compare and contrast GPT and MBR partition tables.

   - MBR partition tables are compatible with BIOS, not UEFI BIOS. GPT partition tables are compatible with either since it has an MBR partition table as part of its structure.
   - MBR partition tables generally support 4 partitions (unless one of them is an extended partition). GPT partitions tables have partition limits as set by the OS

9. Describe a difference between a compiled (Java / C) and interpreted (python / bash) language.

   - The source code of a compiled language needs to be compiled before it can be run. The source code of an interpreted language can be run in by its interpreter.

10. Describe the process that happens from when the computer is powered on to the operating system displaying.

- BIOS / UEFI BIOS is loaded from motherboard
- BIOS / UEFI BIOS calls POST - if POST is successful, returns to BIOS
- BIOS / UEFI BIOS calls bootable partition of disk (bootloader)
- Bootloader optionally loads boot menu for kernel / OS selection
- Bootloader calls kernel
- Kernel loads OS

## Written commands / code

1. In a local git repository, a new file is created called hello.txt  
   Write the steps needed to have add it to my remote repository (GitHub).

```
git add hello.txt
git commit -a -m "Adding hello.txt"
git push
```

2. Craft the necessary command(s) to change the permissions on the file so that bob is the owner and can read and write, the group can read and write, and others can only read.

```
-rwxr-x--x sue sue file.txt
```

```
chown bob file.txt - this changes owner
chmod -x file.txt - removes execute for all
chmod g+w file.txt - adds write privileges for group
chmod o+r file.txt - adds read only privileges to others

final form:
-rw-rw-r-- bob sue file.txt
```

3. Given the following Makefile contents, how can you run the target, go?

```
go: code.c
     gcc -Wall -o runme code.c
```

- make go

4. Craft a bash if statement that checks to see if the file scripty.sh is executable.

```
if [-x scripty.sh]; then
   echo "scripty.sh is executable"
fi
```

5. What Linux command can help me find usage and documentation about another command?

- man (help is accepted)

## Fill in the blank

1. The \_\_\_\_ file in my home directory holds configurations for my bash shell, including aliases.

   - .bashrc

2. The \_\_\_\_ command shows me filesystem level information about a file, such as its inode, permissions for user, group, and other, and how many links exist to the inode.

   - stat

3. The \_\_\_\_ is a circuit board with dedicated busses to different hardware components, such as the CPU, RAM, disks, and GPUs.

   - motherboard

4. The file \_\_\_\_ can be used to store mount configurations for disk partitions, assuming they have a file system on the partition.

   - /etc/fstab OR fstab

## True / False

1. The operating system is the first thing that runs after pushing the power button on a computer.

   - False. The BIOS \ UEFI BIOS is first.

2. The CPU runs in a fetch-decode-discard cycle from startup to shutdown.

   - False. The CPU follows the fetch-decode-EXECUTE cycle from startup to shutdown.

3. In regular expressions, the + (plus) will match one or more occurrences of a pattern while a \* (asterisk) will match zero or more occurrences of a pattern.

   - True

4. If C source code is compiled in Linux, the compiled program is also able to run on Windows.

   - False
