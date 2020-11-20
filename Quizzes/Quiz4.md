# Quiz 4

1. Describe TCP.

- TCP is the handshake protocol. It confirms that packets have arrived and the client is in constant communication with the host.

2. Given a network prefix & CIDR notation of 10.2.78.0/23, write the corresponding netmask.

- 255.255.254.0

3. \_\_\_ is the parent of all processes in Linux.

- init (systemd is also accepted)

4. \_\_\_ is responsible for maintaining the page table and managing running processes.

- kernel

5. What is the benefit of a multi-core CPU?

- A process can be run on each core

6. Describe a key difference between running a process in the foreground / background of a terminal versus detaching it from the terminal using a tool like screen.

- By detaching a process, it can stay alive even if the user logs out.

7. Write a command (or commands) that will create and switch to a new branch in a git repository called "hotfix".

- `git checkout -b hotfix`

8. T/F Layer 4 of the OSI network model handles presenting data, such as the visual page the browser displays.

- False. Layer 7 is the presentation layer. Layer 4 handles TCP / UDP procotols

9. T/F When entering a URL, the system has a series of local files it references before going to a default DNS server.

- True. The system checks files such as `/etc/hosts` and `/etc/resolv.conf` before checking a default DNS server, usually maintained by the ISP.
