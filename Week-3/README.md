## WEEK 3

Snort is a network intrusion detection system (NIDS) that uses signatures and rule sets to monitor real-time network traffic and detect malicious activities via packet analysis.

Today we will install Snort and write Snort rules that would be able to detect this traffic.

### LAB 3 - Overview and Walkthrough


By the end of this lab you will:

- [ ] Employ the pytbull-ng testing framework to view network attacks in real-time
- [ ] Configure Snort to track network communication
- [ ] Write a custom Snort rule to prevent specific network activity

### Project 3 - Overview and Walkthrough

Overview

Now that you have dabbled in the IDS/IPS Snort let's move onto generating and identifying traffic capable of tripping IDS alerts.

In Project 1 we analyzed SMTP (Simple Mail Transfer Protocol) traffic -- the protocol used for emails. You encountered another Layer 7 protocol, HTTP, whenever you use browser to request web pages. FTP (File Transfer Protocol) is a protocol that allows for file transfer from one system to another, but has its share of vulnerabilities. In this project we will launch a Directory Traversal attack on an FTP server that we have installed. Then we will do some packet sniffing of another attack and try to track down which files the attacker was able to access.

Imagine the following situation:

You have been hired by the IRS to investigate the Fairly Oddparents Corp. They are suspected of some shady business and are withholding vital information about the company; we have been granted access to the company server and permission to access their files.

(Reminder: It is NEVER okay to use your cybersecurity knowledge to attack people/companies/systems/etc. in real life.)

The Fairly Oddparents Corp. has only publicly released what is found in the general folder, and announced their earnings in general/reports.txt... but Timmy, Wanda, and Cosmo are suspected to be hiding the original reports in their personal folders...

Since we don't have access to those folders, this is where the Directory Traversal attack comes in. While there are many ways to navigate file systems, here you should run attack.js on directories to see what's inside -- see if you can reveal the contents of an alternative version of the general/reports.txt!

### Project Goals

By the end of this assignment, you will be able to...

- [ ] Use bash scripting to launch an attack to access files located on an ftp server
- [ ] Gain more practice navigating the Vim editor.
- [ ] Analyze a .pcap file of Fairly Oddparents Corp. server traffic and identify which files the Directory Traversal attack was able to access without proper permissions.
- [ ] Resources


### Lab Resources

- [ ] [TryHackMe's Snort CheatSheet](https://assets.tryhackme.com/cheatsheets/Snort%20Cheatsheet%20-%20TryHackMe.pdf) Get started with Snort on CLI
- [ ] [pytbull-ng](https://github.com/netrunn3r/pytbull-ng)
- [ ] [Snort Rule Writing Guide](https://docs.snort.org/rules/)
- [ ] [Vim Cheat Sheet](https://devhints.io/vim) Most common vim editing commands on 1 page

### Project Resources

- [ ] FTP(https://www.hostinger.com/tutorials/what-is-ftp) What is ftp?
- [ ] Directory Traversal attack
- [ ] Vim Cheat Sheet Most common vim editing commands on 1 page
- [ ] Bash Cheat Sheet Most common bash editing commands on 1 page