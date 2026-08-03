# TryHackMe Lab Write-Up
## Linux Fundamentals Part 1 | What is Networking? | Intro to LAN

**Student:** Nimet Eyayu Alemu  
**ID:** CTC-3382-26          
**Group:** George, Gedion Desalegne Group  
**Date:** August 3, 2026  

---

## Introduction

Hey! This document contains write-up for three TryHackMe rooms that I completed as part of my cybersecurity training at INSA Cyber talent Summer Camp 2026. I completed three TryHackMe rooms - linux Fundamentals Part 1, What is networking?, and Intro to LAN. These labs were great for beginners in cyber security because they contain basics of Linux and networking. I'm gonna share what I learned from each room and show some screenshots of my work.
Why These Labs Matter
In cybersecurity, Linux and networking are the foundation of everything we do. Whether you're conducting penetration tests, defending networks, or analyzing traffic, you have  to understand these basics. These labs gave me hands-on experience that I can apply in real-world scenarios.
This Report contains
•	Key concepts I learned from each lab
•	Commands I actually used (with explanations)
•	Screenshots showing my work
•	Reflect  challenges that I face in the process and what I enjoyed

---

## Lab 1: Linux Fundamentals Part 1

### What I Learned

In this room i learn basic and  fundamental linux commands: 
first let us see the definition of linux. Linux is a free and open source  operating system just like windows and macs. It widely used in servers, cloud computing, cybersecurity and software development. Linux isn't one operating system  it's a family built on UNIX. Because of it’s open-source, there are many versions called "distributions" or "distros".

and this is also concept like terminal and basic commands. here is commands i learn through this room
- **Navigation commands** like `cd`, `ls`, and `pwd` - these help you move around and see what's in folders
- **Creating and managing files** with `touch`, `cp`, `mv`, and `rm`
- **File permissions** - understanding read, write, execute and using `chmod` to change them
- **Finding stuff** with `grep` - this was actually really useful

### Commands I Actually Used to solve the questions

Here are some commands I practiced:

| Command | What It Does |
|---------|--------------|
| `ls` | Shows what files/folders are in current directory |
| `cd folder4` | Changes directory to folder4 |
| `pwd` | Shows where I currently am |
| `cat note.txt` | Shows what's inside a file |
| `grep THM access.log` | Searches for "THM" in the file |
| `echo TryHackMe` | Prints "TryHackMe" on screen |
| `whoami` | Shows my username |

### What I Did

First, I click start lab machine button to connect to the machine. I was at `tryhackme@linux1` which was my username.

I used `ls` and saw there were folders named folder1 to folder4 and a file called `access.log`. I explored each folder and in folder4 I found a file called `note.txt` which had "Hello World!" inside.

I also used `grep` to search for "THM" in the `access.log` file. The command was `grep THM /home/tryhackme/access.log` and I found the flag `THM{ACCESS}`. That was pretty satisfying!

I practiced `echo TryHackMe` which just displayed the text, and `whoami` which showed I was logged in as `tryhackme`. Basic stuff but good to practice.
the most useful command that i learn is the command find because when i try to find a specific file it becomes a headache when we're having to look through every single one just to try and look for specific files. if i know the file name that i went i can just use  find -name passwords.txt(name of the file) where the command will look through every folder in our current directory for that specific file. and of course i couldn't pass without mension The command grep this allows us to search the contents of files for specific values that we are looking for.if we went to see all files that has a specific file extention.
there are operators in linux such us:
&	This operator allows you to run commands in the background of your terminal.
&&	This operator allows you to combine multiple commands together in one line of your terminal.
>	This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere.
>>	
This operator does the same function of the > operator but appends the output rather than replacing (meaning nothing is overwritten).
In this room we've covered the following:

Understanding why Linux is so commonplace today
Interacting with your first-ever Linux machine!
Ran some of the most fundamental commands
Had an introduction to navigating around the filesystem & how we can use commands like find and grep to make finding data even more efficient!
 Power up your commands by learning about some of the important shell operators.

### Screenshots

*Figure 1: Checking what files are in my directory*

![Linux Navigation](images/linux-ls.png)

*Figure 2: Finding the flag using grep*
![Linux Grep](images/linux-grep.png)

*Figure 3: Interacting with the Linux machine and using whoami*
![Linux Whoami](images/linux-whoami.png)

*Figure 4: Exploring folders and finding the note.txt file*
![Linux Folders](images/linux-folders.png)

*Figure 5: Reading note.txt and seeing "Hello World!"*
![Linux Hello World](images/linux-hello.png)

*Figure 6: Using echo and trying to navigate*
![Linux Echo](images/linux-echo.png)

*Figure 7: More practice with commands*
![Linux Practice](images/linux-practice.png)

---

## Lab 2: What is Networking?

### What I Learned

In this room i learn about networking concepts. Here is what i learned:

- What an **IP address** is - it stands for Internet Protocol and has 4 parts called octets (like 10.112.177.231)
- **MAC addresses** - these are physical addresses for devices, like `04:9E:44:99:A3:12`
- **Ping** uses ICMP protocol to check if a server is alive

### What I Did

I learned the fundamental networking concepts first of all about networking. Networks are simply connected thing just like my connection of many friends.a network can be formed by anywhere from 2 devices to billions.the other fundamental concept that i learned through this room is internet. The Internet is one giant network that consists of many small networks within itself. there are two types of network private and public.
the main concept on this room is IP addresses it uses to identify devices on a network it is just like students id if the student changes school there id also change . MAC addresses are like physical serial numbers for network cards it is like fingerprint you were born with it every device gets mac address from the manufacture when it produced. there are two types of ip address the old one ipv4 and the new ipv6.
the interesting thing with MAC addresses is that they can be faked or "spoofed" in a process known as spoofing. This spoofing occurs when a networked device pretends to identify as another using its MAC address. for preventing to happen this we need a body garde that is  A firewall.it make sure the communication between two device is safe from other thired party.

I also learned about ping - it's a command to check if a server is online. I pinged `8.8.8.8` (Google's DNS) and got the flag `THM{I_PINGED_THE_SERVER}`.

### Screenshots

*Figure 8: Understanding IP and MAC addresses*
![Networking IP MAC](images/networking-ip-mac.png)

*Figure 9: Learning about the Internet and who invented WWW*
![Networking Internet](images/networking-internet.png)

*Figure 10: Using ping to check if a server is online*
![Networking Ping](images/networking-ping.png)

---

## Lab 3: Intro to LAN

### What I Learned

In this room i learn about Local Area Networks. Here is the main content:

- **LAN** stands for Local Area Network
- **Routers** do routing (obvious, right? lol)
- **Switches** connect multiple devices on a network
- **Topologies** - bus topology is cheap but star topology is expensive
- **Subnetting** - dividing networks into smaller pieces
- **Subnet masks** have 32 bits and octets range from 0-255
- **ARP** stands for Address Resolution Protocol
- **DHCP** - devices use DHCP Discover, Request, and ACK to get IP addresses

### What I Did
in this room we see about lan. A LAN (Local Area Network) is a group of computers and electronic devices connected together across a small local area, such as a home network, an office building, or a school. Common examples include a home Wi-Fi connecting your phone and smart TV, or an office network sharing a single printer. we cover 3 types of Local Area Network (LAN) Topologies  here they are:
Star Topology
is a devices are individually connected via a central networking device such as a switch or hub
Bus Topology
This type of connection relies upon a single connection which is known as a backbone cable.it is just like leaf off of a tree in the sense that devices.
Ring Topology
it has some similarity to token topology. Devices such as computers are connected directly to each other to form a loop, meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology.
I learned about different network topologies. Bus topology is cheaper but star topology is expensive. I did an interactive lab where I found topology flaws and got the flag `THM{TOPOLOGY_FLAWS}`.

I also learned about subnetting which is dividing networks into smaller parts it is just like slicing up a cake for your friends- super useful for security and efficiency.

I learned about ARP (Address Resolution Protocol) which helps devices find each other using MAC addresses.

And DHCP - this is how devices get IP addresses automatically. They send a Discover packet, then Request, then get an ACK (acknowledgment).

### Screenshots

*Figure 11: Learning about LAN and network devices*
![LAN Basics](images/lan-basics.png)

*Figure 12: Topologies and flags*
![LAN Topologies](images/lan-topologies.png)

*Figure 13: Understanding subnetting*
![LAN Subnetting](images/lan-subnetting.png)

*Figure 14: Subnet mask questions*
![LAN Subnet Mask](images/lan-subnetmask.png)

*Figure 15: ARP (Address Resolution Protocol)*
![LAN ARP](images/lan-arp.png)

*Figure 16: DHCP packets (Discover, Request, ACK)*
![LAN DHCP](images/lan-dhcp.png)

---

## Summary & Reflection

Honestly, these labs were really fun and useful! The Linux one was my favorite because I got to actually type commands and see things happen. I already knew some basic commands but I learned new stuff like `grep` which is really useful for finding things in files.

The networking rooms helped me understand how the internet actually works. Before this, I knew what an IP address was but I didn't really understand MAC addresses or why we need both. Now I get it - IP is like your home address and MAC is like your physical house, both are needed!

The LAN room was interesting because I never really thought about how networks are set up. I didn't know there were different topologies or what subnetting was. It makes sense though - businesses need to separate their employee network from guest WiFi for security.


## References

- TryHackMe. (2026). *Linux Fundamentals Part 1*. https://tryhackme.com/room/linuxfundamentalspart1
- TryHackMe. (2026). *What is Networking?*. https://tryhackme.com/room/whatisnetworking
- TryHackMe. (2026). *Intro to LAN*. https://tryhackme.com/room/introtolan


---

**🔗 Repository Link:** https://github.com/niemaDev/TryHackMe-Linux-Networking-Writeup

---
