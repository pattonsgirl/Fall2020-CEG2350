# Quiz 3

1. I have a new script in a folder called "cool_stuff". I need to add the absolute path to the \_\_ enviroment variable to run the script in any directory without specifying the folder everytime.

- PATH

2. Write a regex that only matches 1 or more occurences of o in the following:

```
o
B
Bo
Boooo
Boo
Boooooooo
```

- o+ OR \[o\]

3. Write bash function called foo that prints "Bubbles" to a file called joy.txt

```
foo () {
    echo "Bubble" > joy.txt
}
```

4. I have a script that should change the directory I'm in to somewhere else, but when I call the script (let's assume I've checked PATH) by typing 'my_script' into the terminal, nothing happens (no errors, but no action). How did I need to run my script?

- `source my_script` or `. my_script`

5. Java and C source code can be executed on the command line. So to run a java or c source code file, I only need to:
   ./my_code.c

- False
- Need to create a compiled version, then run the compiled version. For c, you would use `./program`. For java, you would use `java class_name`

6. The make command relies on a special file named SpecialFile to do actions.

- False
- File name is `Makefile`

7. The bootloader calls POST to check that hardware compatibility and connectivity

- False
- The BIOS or UEFI BIOS calls POST. The bootloader passes control to the kernel.

8. The \_\_ interfaces between the hardware and the OS.

- kernel

9. \_\_ and \_\_ are the most common partition tables.

- MBR & GPT
