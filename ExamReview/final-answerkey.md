## Written Answer

1. Describe an advantage of using a VPN over a proxy for communications.

   - A VPN (Virtual Private Network) not only masks the originating IP, but also creates a secure, encrypted tunnel for communication. A proxy only masks the orginating IP; it does not encrypt the traffic.

2. Compare and contrast TCP to UDP.

   - TCP (Transmission Control Protocol) utilizes the handshake protocol to confirm with the server that data was recieved. It also verifies the order of the packets and will request another transmission of a packet if out of order or if data was corrupted in transmission.
   - UDP (User Datagram Protocol) is used by services that don't care about packet loss or packets arriving out of order. There is no confirmation between client and server that packets were recieved.

3. List a method of verifying file integrity of downloaded files.

   - Any of
     - checksums
     - GPG / PGP keys

4. I have made an SSH key pair on my system. Which key goes in the remote system's authorized_keys file?

   - The public key (id_rsa.pub by default, otherwise the file that ends with .pub)

5. Describe the difference between a thread and a forked / child process.

   - A thread operates within a process - threads share memory space with the process they exist in. A child process is a process in itself - it has its own memory space to operate.

6. Identify and describe the three roles performed by a hardware router. (3 pts)

   - NAT - Network Address Translation between my devices on a private network and the outside world (public network)
   - Firewall - can set rules of traffic allowed in and out
   - DCHP - can hand out IP addresses to devices connected to the router
   - Routing table - manages where packets go

7. What is the purpose of DNS?

   - Domain Name servers translate between IP addresses and URLS / Hostnames

8. How does the kernel manage processes?

   - Selection (via prioritization) of processes
   - CPU time slices (time allocation) of processes to keep them going forward

## Written commands / code

1. Write a series of commands that would do the following:

   - Create a new branch called additions
   - Add a new file called bubbles.txt to the additions branch
   - Merge the additions branch with master / main
     - `git checkout -b additions` OR `git branch additions` then `git checkout additions`
     - `touch bubbles.txt`
     - `git add bubbles.txt` (or `.` or `*`)
     - `git commit -a -m "Added new file"`
     - `git checkout master`
     - `git merge additions`

2. Given a directory named foo, write command(s) to create a tar ball of the directory, then compress the tar ball.

   - `$ tar cvf foo.tar foo`
   - `$ gzip foo.tar`

3. Given a script named bar.sh, write a command that would run the script in the background and then a command that would recall the script to the foreground.

   - Using jobs:
     - `./bar.sh &` OR use `CTRL+Z` on `bar.sh` while it is running, then send to background with `bg`
     - `fg %#` where # is the number associated with the job. Just `fg` is sufficient if its the only job

4. Given a network prefix and CIDR notation of 201.34.56.0/24, answer the following:

   - What is the subnet mask associated with the CIDR notation given?
   - Does the network prefix likely match a public or private IP range?
   - Write an IP address that would be included is the defined range.
     - Subnet mask is 255.255.255.0
     - Public IP. Private IPs start with 10. || 172. || 192.
     - 201.34.56.90 would be an example of a valid IP. Since the prefix is 201.34.56.0, and the subnet mask is 255.255.255.0, only the last set (D) can be changed. So 201.34.56 are "fixed", and .1 through .255 are valid

## Fill in the blank

1. In virtual machines, the \_\_\_\_ manages shared resources, such as CPU, RAM, and disk operations, between the host OS and the guest OS(s).

   - hypervisor

2. Assuming an sftp connection has been established, I can use the command \_\_\_\_ followed by a series of filenames to upload those files to the remote computer.

   - put

3. Assuming an sftp connection has been established, I can use the command \_\_\_\_ followed by a series of filenames to download those files to the local computer.

   - get

4. Port \_\_\_\_ is the default port for HTTPS.

   - 443

5. \_\_\_\_ processes are created when the parent process terminates but the child process is still running.

   - orphan
   - zombie proccess occurs when child terminates, but did not signal termination to parent - therefore is does not get cleaned up in memory

6. The \_\_\_\_ command shows running processes in Linux

   - top OR ps

## True / False

1. SSH commonly uses port 80

   - False, SSH uses port 22

2. Virtual machines have a full version of an Operating System, including a kernel. Containers rely on the host kernel and essentially overlay additional programs that run in the container.

   - True.

3. Caches store commonly requested information, both locally and in remote sites to prevent constant requests for information from the actual server.

   - True

4. The targets and actions written in a Makefile are used with the command makefile

   - False. The `make` command uses the Makefile's targets and actions
