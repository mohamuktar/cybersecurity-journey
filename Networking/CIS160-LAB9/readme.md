# LAB 9: Use Nmap to Test a Network 

## Overview
In this lab, I used Kali Linux running in VMware to explore Nmap and practice network scanning on my home network.

## Activities Completed
1. Explored Nmap commands and Zenmap profiles to understand different scanning options.
2. Practiced ping sweeps, TCP SYN scans, UDP scans, and scanning all ports.
3. Used `ip -4 addr` to identify my Kali VM's IP address (`192.168.1.176`) and subnet mask (`255.255.255.0`).
4. Ran a ping sweep using `sudo nmap -sn 192.168.1.0/24` to discover five active devices on my home network.
5. Scanned my default gateway (`192.168.1.254`) and identified three open TCP ports: 53 (DNS), 80 (HTTP), and 443 (HTTPS).
6. Identified the gateway manufacturer as Sagemcom Broadband SAS.
7. Performed identification scans on three additional devices: a Samsung Galaxy A71, an iPhone, and my computer.
8. Reviewed Nmap's capabilities and learned how it can help identify devices, open ports, running services, and potential security weaknesses.

## Conclusion
This lab helped me gain practical experience using Nmap from the Kali Linux terminal to discover network devices, examine open ports, identify services, and assess my home network.