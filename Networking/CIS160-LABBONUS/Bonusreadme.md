# Lab: Network Routing

## Objectives
- Inspect the routing table.
- Use `ping` and `tracert` to test network connectivity.

## Part 1: Inspect the Routing Table

I used Windows Terminal and the `netstat -r` command to view the computer's routing table.

**Prelab – Private IPv4 Addresses**
- Class A: `10.0.0.0 – 10.255.255.255`
- Class B: `172.16.0.0 – 172.31.255.255`
- Class C: `192.168.0.0 – 192.168.255.255`
- Loopback: `127.0.0.0/8`

**Routing Table Results**
- Default gateway: `10.130.0.1`
- Default destination: `0.0.0.0`
- LAN subnet: `/21`
- IPv6 interfaces: `1` and `3`

## Part 2: Tracert Testing

I used `tracert` to examine the network paths to different destinations.

| Destination | Hops | Results |
|---|---:|---|
| `127.0.0.1` | 1 | Local loopback interface |
| `10.130.0.1` | 1 | Default gateway |
| `13.249.182.46` | 17 | Remote destination across multiple networks |
| `10.130.0.5` | 1 | On-link address within the LAN |

The remote destination took approximately 30 ms, compared with less than 1 ms for the gateway.

## Reflection

Ping tests connectivity between devices, while tracert shows the network path and intermediate hops packets take to reach a destination. Tracert helps administrators identify potential network problems, such as high latency, routing issues, and unresponsive devices.

## Conclusion

This lab helped me understand how to inspect routing tables and use network diagnostic tools to examine local and remote network connections. I also learned how tracert identifies the hops packets take across a network.