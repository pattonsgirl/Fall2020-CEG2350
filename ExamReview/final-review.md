## Processes

1. Task Manager (Linux [top] vs. Windows)
2. init process / kernel level vs user level processes
   a. parent vs child process
3. System calls (way for programs / APIs to interact with the operating system)
   - systemd - systemctl & journalctl
   - Fork & exec
4. Commands: kill, ps, top, nice, bg, fg, jobs, nohup, ~~killall~~, screen
5. Preemptive (interruptible) and non-preemptive scheduling, priorities, signals
6. CPU & kernel memory management
7. Thread vs Fork
8. Single CPU multi-tasking
9. Multiple CPUs ~~and SMP (Symmetric multiprocessing)~~

## Git (version control)

1. Git servers vs. clients
2. Git commands & what they do:
   - push
   - pull
   - commit
   - add
   - init
   - clone
   - **branching**
     - creating
     - merging

## Networking

1. Host names, IP addresses, Subnets, DNS, URLs
2. Protocols: HTTP vs HTTPS
3. TCP and UDP
4. Ports vs sockets, clients and servers, secure shell, sftp
   - Application opens a socket which is connected to a port
5. X11 in terms of graphical “forwarding” and role of a GUI
6. Web browsers (URLs, SSL certs) and clients (ping, wget, traceroute)
7. Physical pieces of a network
   - hosts, routers, switches, ISPs, wireless, LAN
8. Firewalls
9. OSI layers (encapsulation / packets, application, transport, network, datalink, physical)

## System Management

1. Updates (Linux vs. Windows)
2. Installing packages with make
3. Virus scanning & types of computer diseases
4. Creating archives, password locking files
5. System restore (automatic, manual, backups)
6. Windows Registry
7. Boot scripts & init.d
8. Open source movement
9. Torrents

## Computer-ception

1. Virtual machines (GUI style) and hypervisors
   - set up with an amount of RAM it can take up
   - full installation, including kernel - runs within hypervisor
   - hypervisor manages resources to share with host system
2. Containers
   - relies on host kernel
   - environment in which you can install tools / packages / etc without changing host configuration
3. Cloud computing (Google, AWS, Azure)
   - Idea of "coding" infrastructure via configuration files
