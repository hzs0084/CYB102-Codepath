## WEEK 1

This unit, we will explore the role of the Blue Team in an organization's information security, their activities, required skills, and the Security Operations Center they typically work in. We will also explore the differences between a SOC and a Cyber Fusion Center, taking a look inside Target's Cyber Fusion Center!

Finally, we will dip our toe into the NIST Control, discussing the NIST Cybersecurity Framework and NIST System Monitoring. During our lab we will analyze a user's network traffic as well as two different log files to identify the rogue employee behind some bad actions at a company. In this week's project, we'll be analyzing email traffic in an attempt to identify legitimate from fraudulent emails.


### LAB 1 - Overview and Walkthrough

Scneario:\
You’ve been hired to the Security Operations Center of the company Boring Office to help track down the employee behind some nefarious activity. On April 19th, 2023 at 12:50PM an employee at Boring Office sent their deepest darkest secrets to everyone within the company. Or did they? This employee claims that someone else at the company is impersonating them, and your job is to hunt for who this rogue user is.

By the end of this lab you will be able to...

- [ ] Analyze a .pcap file to find a user's IP address
- [ ] Use DHCP logs to correlate an IP address to a host device
- [ ] Identify which user was logged in to a host device using account security logs

#### Resources:

- [SMTP](https://www.geeksforgeeks.org/computer-networks/-simple-mail-transfer-protocol-smtp/)\
- [IP Address](https://en.wikipedia.org/wiki/IP_address)\
- [Network Layer](https://www.cloudflare.com/en-gb/learning/network-layer/what-is-the-network-layer/)\
- [DHCP](https://learn.microsoft.com/en-us/windows-server/networking/technologies/dhcp/dhcp-top)


### LAB 1 PROJECT - Overview and Walkthrough

One of the most popular scams throughout industries is the Business Email Compromise (BEC). BECs are responsible for many notable real world scams, incurring $26 billion dollars of losses from 2016 to 2019 alone.

We'll be handling our own BEC situation, where a malicious actor (played by Leonardo DiCaprio) has sent phishing emails to many of our employees, trying to trick them into sending hundreds of thousands of dollars. To stop this, we'll be looking at some potentially malicious emails and inspecting .pcap files to determine which emails are legitimate and which ones are fraudulent.

By the end of this assignment you will be able to...

- [ ] Inspect .pcap files and extract their email content
- [ ] Identify legitimate vs. fraudulent emails
- [ ] Correctly identify the malicious actor

#### Resources

- [Reference guide](https://www.wireshark.org/docs/dfref/s/smtp.html) for SMTP display filter commands in Wireshark
- [Source](https://www.malware-traffic-analysis.net/) of the malicious .pcap file

#### Submission

- [Link to GoogleDoc](https://docs.google.com/document/d/1d4w_xsRF8qSTNdWRFq7aQTDnLfJqUdC5FBJYqs4X008/copy)

To receive full credit, you must submit ...

- [ ] The malicious actor's IP address
- [ ] The subject lines of three different phishing emails you identified\
    *Tip: only one of the `.pcap` files contains malicious emails*
- [ ] A detailed explanation of how you found the malicious actor using the provided `.pcap` files

#### Bonus Challenge

To receive bonus points, you can submit...

- [ ] Three different `.eml` files showing the content of the phishing emails you identified
