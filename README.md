# TryHackMe Lab Write-Up
## Linux Fundamentals Part 1 | What is Networking? | Intro to LAN

**Student:** Gedion  
**Group:** George, Gedion Desalegne Group  
**Date:** July 31, 2026  

---

## Introduction

This write-up documents my completion of three TryHackMe rooms:

1. Linux Fundamentals Part 1
2. What is Networking?
3. Intro to LAN

These labs provided hands-on experience with the Linux command line, networking fundamentals, and Local Area Network concepts — all essential skills for cybersecurity.

---

## Lab 1: Linux Fundamentals Part 1

### What I Learned

- How to navigate the Linux file system using `cd`, `ls`, and `pwd`
- Creating and managing files with `touch`, `cp`, `mv`, and `rm`
- Understanding file permissions (read, write, execute)
- Changing permissions with `chmod`
- Using `man` to view command documentation
- System information commands: `whoami`, `id`, `uname`

### Commands I Used

| Command | What It Does |
|---------|--------------|
| `ls -la` | List all files including hidden ones |
| `cd /home` | Change directory to /home |
| `pwd` | Show current directory |
| `mkdir folder` | Create a new folder |
| `touch file.txt` | Create a new file |
| `cp file1 file2` | Copy file1 to file2 |
| `mv file1 /newdir/` | Move file1 to a new folder |
| `rm file.txt` | Delete a file |
| `chmod 755 script.sh` | Set permissions |
| `man ls` | View manual for ls |

### Screenshots

*Figure 1: Navigating the Linux file system*
![Linux Navigation](images/linux-navigation.png)

*Figure 2: File permissions demonstration*
![Linux Permissions](images/linux-permissions.png)

*Figure 3: Completed Linux room tasks*
![Linux Completion](images/linux-completion.png)

---

## Lab 2: What is Networking?

### What I Learned

- The OSI Model (7 layers)
- TCP vs UDP protocols
- IP addressing basics
- Common network ports:
  - HTTP = 80
  - HTTPS = 443
  - SSH = 22
  - DNS = 53
- How routers, switches, and hubs work

### Screenshots

*Figure 4: OSI Model exercise*
![OSI Model](images/osi-model.png)

*Figure 5: IP addressing task*
![IP Addressing](images/ip-addressing.png)

*Figure 6: Port identification exercise*
![Ports](images/ports.png)

---

## Lab 3: Intro to LAN

### What I Learned

- MAC addresses vs IP addresses
- How ARP (Address Resolution Protocol) works
- How DHCP assigns IP addresses
- LAN topologies: star, bus, ring
- Broadcast domains and collisions

### Screenshots

*Figure 7: MAC address identification*
![MAC Address](images/mac-address.png)

*Figure 8: ARP demonstration*
![ARP](images/arp.png)

*Figure 9: DHCP process explanation*
![DHCP](images/dhcp.png)

---

## Summary & Reflection

Completing these three TryHackMe rooms gave me a strong foundation in Linux and networking.

The Linux Fundamentals room helped me become comfortable with the command line. I now understand how to navigate the file system, manage files, and set permissions — essential skills for using security tools like Nmap, Metasploit, and Wireshark.

The Networking room taught me how data moves across networks. Understanding the OSI model, TCP vs UDP, and common ports gives me context for network security analysis.

The Intro to LAN room showed me how devices communicate within local networks. Learning about MAC addresses, ARP, and DHCP helps me understand network scanning and defense strategies.

### Challenges I Faced

The hardest part was memorizing Linux commands and their options. I practiced each command multiple times and used the `man` command to explore different options. Understanding the difference between TCP and UDP also took some time, but the TryHackMe explanations helped.

### Next Steps

I plan to continue with:
- Linux Fundamentals Parts 2 and 3
- Network Security room
- Wireshark 101
- Jr. Penetration Tester learning path

---

## References

- TryHackMe. (2026). *Linux Fundamentals Part 1*. https://tryhackme.com/room/linuxfundamentalspart1
- TryHackMe. (2026). *What is Networking?*. https://tryhackme.com/room/whatisnetworking
- TryHackMe. (2026). *Intro to LAN*. https://tryhackme.com/room/introtolan

---

## Repository Structure

```
TryHackMe-Linux-Networking-Writeup/
├── README.md           # This write-up
└── images/             # All screenshots
    ├── linux-navigation.png
    ├── linux-permissions.png
    ├── linux-completion.png
    ├── osi-model.png
    ├── ip-addressing.png
    ├── ports.png
    ├── mac-address.png
    ├── arp.png
    └── dhcp.png
```

---

**🔗 Repository Link:** https://github.com/niemaDev/TryHackMe-Linux-Networking-Writeup

---

*⚠️ All work, screenshots, and reflections are my own. No AI tools were used in completing the labs or writing this documentation.*
