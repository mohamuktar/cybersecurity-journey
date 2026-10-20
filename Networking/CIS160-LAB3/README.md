Writing

# Lab 3: Packet Tracer – Examine Addressing Tables

## Overview

This lab explores Address Resolution Protocol (ARP), switch MAC address tables, and how devices communicate within and across networks using Cisco Packet Tracer.

## Objectives

- Examine ARP requests and replies.
- Analyze switch MAC address tables.
- Understand ARP in remote network communications.
- Compare the functions of routers and switches.

## Key Concepts

- **ARP:** Resolves an IPv4 address to a MAC address on the local network.
- **MAC Address Table:** Maps MAC addresses to switch ports to forward Ethernet frames.
- **Default Gateway:** Allows devices to reach destinations outside their local subnet.
- **Simulation Mode:** Visualizes ARP and ICMP packets as they travel through the network.

## Lab Results

- Observed ARP broadcasts using `FFFF.FFFF.FFFF` as the destination MAC address.
- Examined how switches flood broadcast frames and learn MAC addresses.
- Verified ARP table entries using `arp -a`.
- Inspected switch MAC address tables using `show mac-address-table`.
- Examined router ARP entries using `show arp`.
- Observed that the first ping may time out while ARP resolution occurs.

## Useful Commands

```
arp -a
arp -d
ping 172.16.31.3
show mac-address-table
show arp
```

## Key Takeaways

Routers forward packets between different networks using IP addresses, while switches forward Ethernet frames within a LAN using MAC addresses. ARP enables devices to discover MAC addresses needed for local network communication, including communication with a default gateway.

## Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- ARP and ICMP troubleshooting commands