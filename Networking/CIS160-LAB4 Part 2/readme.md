# LAB 4 – Part 2: Design and Implement a VLSM Addressing Scheme

## Objective
To design and implement a VLSM addressing scheme using the `10.1.1.0/24` network, configure routers, switches, and PCs, and verify connectivity in Cisco Packet Tracer.

## What I Did
I divided the network into four LAN subnets and one WAN subnet based on the required number of hosts. I configured the IP addresses and subnet masks on both routers, assigned management IP addresses and default gateways to the switches, and configured the PCs with their IP addresses and default gateways.

I used `no shutdown` to enable the router interfaces and configured the serial interfaces with `10.1.1.121/30` and `10.1.1.122/30`.

## Verification and Troubleshooting
I used `show ip interface brief` to check the router interface status and `ping` to test connectivity between devices. Initially, the serial connection remained down even after I entered `no shutdown`. I resolved this by enabling the serial interfaces on both routers. I was able to ping between LANs, although some requests timed out.

## Potential Problems
Possible issues include incorrect IP addresses or subnet masks, wrong default gateways, duplicate IP addresses, and forgetting to enable interfaces using `no shutdown`.

## Conclusion
I successfully implemented the VLSM addressing scheme and practiced configuring network devices and troubleshooting connectivity issues in Cisco Packet Tracer.