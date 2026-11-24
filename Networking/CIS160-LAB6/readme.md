# LAB 6: Packet Tracer – Use Ping and Traceroute to Test Network Connectivity

## Purpose

The purpose of this lab was to troubleshoot IPv4 and IPv6 connectivity issues using ping, traceroute, and router configuration commands.

## Part 1: Test and Restore IPv4 Connectivity

I used `ipconfig`, `ping`, and `tracert` to test connectivity between PC1 and PC3. The initial ping failed, and traceroute helped identify where communication stopped.

After inspecting the router configurations, I discovered that R2's Serial0/0/0 interface had an incorrect IP address. It was configured as `10.10.1.2` instead of `10.10.1.5`.

**Solution:** I accessed R2's CLI and corrected the interface configuration:

```
interface S0/0/0
ip address 10.10.1.5 255.255.255.252
```

After the change, I successfully pinged between PC1 and PC3, confirming that IPv4 connectivity was restored.

## Part 2: Test and Restore IPv6 Connectivity

I used `ipv6config`, `ping`, and `tracert` to investigate connectivity between PC2 and PC4. The initial ping failed. After inspecting R3's IPv6 interfaces, I discovered that PC4 had an incorrect default gateway.

PC4 was configured with `FE80::2`, but R3's directly connected GigabitEthernet0/0 interface used `FE80::3`. The address `FE80::2` belonged to R2.

**Solution:** I opened PC4's Desktop → IP Configuration and changed its IPv6 default gateway from `FE80::2` to `FE80::3`.

After making the correction, I successfully pinged between PC2 and PC4, confirming that IPv6 connectivity was restored.

## Conclusion

This lab helped me practice using ping and traceroute to identify network connectivity problems. I learned how incorrect router IP addresses and IPv6 default gateways can prevent devices from communicating. I also gained experience inspecting router interfaces and correcting network configurations to restore connectivity.
