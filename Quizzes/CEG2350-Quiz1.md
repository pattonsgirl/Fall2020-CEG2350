1. Write only the flags that are in the command below.
`ssh -i /home/demo/key.pem user@10.0.0.0`

* -i, identity_file  
    * ssh is the command, -i is the flag that specifies to use the key file, /home/demo/key.pem is the path to the key, user@10.0.0.0 is the username of the system (10.0.0.0) that we would to log in to.

2. What does the `mkdir` command do?

* `mkdir` makes a directory of the name given.  Usage is `mkdir folder_name`

3. What command displays a manual for a given command?

* `man` is a command that displays a manual (if it exits) for a given command.  Usage is `man command_name`

4. _______ is a command that is used to switch from one directory to another.

* `cd` 

5. T/F A private key can be shared publicly.  Others should have permission to edit my private key.

* False.  Private keys must be protected, even in terms of user permissions - for example, the "other" category in Linux cannot have edit permissions to my key.




