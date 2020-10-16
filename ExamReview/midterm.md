## Basics

1. Operating systems as jargon – Windows, Linux, Mac
2. Linux distributions: Debian, RedHat, etc
3. Intro to course tools (AWS & MobaXTerm)
4. Intro to shells (bash, sh, zsh, powershell, ssh) and commands (man, vim, history)
5. Intro to ssh & key pairs
6. Intro to git (clone, commit, push, add)

## Files, directories, and OS structure

1. OS structure in Linux (and Mac) vs Windows
2. Files vs directories
   - Commands: ls, cp, mkdir, rmdir, vim, mv, rm, cat, touch, head/tail, less/more
3. Importance of names and extensions (file)
4. Ownership & sharing
   - rwx permissions in Linux (and Windows counterpart)
   - user vs. group vs. other
   - chmod, chown
   - User types and groups: sudo vs. admin vs. “other” (sudo, adduser, deluser)
5. Hard links & soft links (ln)
6. Inodes
7. File locks

## Scripting

1. Aliases & customizations (.bashrc, ~~.vimrc~~)
2. Commands: grep, diff, find, file, wc, sort, uniq, whereis, which
3. IO redirection (<, >, |, tee)
4. PATH (order of execution)
5. Scripting languages: bash, python
6. Regular expressions (grep, ~~sed~~, test)
7. ~~Alternate data streams (od, /dev/null)~~
8. ~~Requiring root to run~~

## Command line programming

1. Assembly/machine language programming
   - Bits (1), bytes (8 bits), word (16, 32, or 64 bits)
2. Interpreters
3. Libraries & dynamic linking (loads and links the shared libraries needed by an executable when it is executed)
4. Memory handling in programming (static vs. stack vs. heap)
5. Makefiles
6. Compiling programs (Linux is not Windows)
   - Linux ELF (Executable & Linkable Format)
   - Windows EXE
7. Overview of command line debugging
8. Commands: ldd, make

## Data storage and access:

1. Computer Hardware Basics
   - CPU
     - CPU cycle: instruction fetch, decode, and execution
   - RAM
   - Motherboard
   - HDD vs SSD
   - GPU (in terms of integrated vs dedicated)
   - Virtual memory: swap tables / paging
2. Booting of OS
   - Power on self-test (POST)
   - BIOS vs UEFI
   - Partition Tables: GPT vs MBR
   - Boot loaders: NTLDR, GRUB
3. Fragmentation
4. Sequential and random access
5. ~~Compression (gzip, tar)~~
6. File systems: vfat, ntfs, ext
   - ~~implementations / fragmentation / performance~~
7. ~~Network file share: SFTP, NFS, Samba~~
8. Commands: df, du, mount, umount, etc/fstab
9. Devices and drivers
