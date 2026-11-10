# Lab 5: Packet Tracer – TCP and UDP Communications

## Objectives
- Generate network traffic in Simulation Mode.
- Examine TCP and UDP functionality.
- Understand multiplexing and port numbers.

## Lab Summary

I used Cisco Packet Tracer Simulation Mode to generate HTTP, FTP, DNS, and email traffic between client devices and a server. I observed how PDUs travel through the network and examined their protocol headers, port numbers, sequence numbers, acknowledgment numbers, and TCP flags.

I also explored the TCP three-way handshake and how TCP establishes connections before application data is exchanged. For DNS, I observed how UDP uses port 53 to handle name resolution.

## Key Findings

- **TCP:** Connection-oriented and reliable; uses acknowledgments, sequence numbers, and retransmissions.
- **UDP:** Connectionless and does not guarantee delivery.
- **HTTP:** Uses TCP port 80.
- **FTP:** Uses TCP port 21 for control communication.
- **DNS:** Uses UDP port 53.
- **Email:** Uses SMTP (TCP port 25) and POP3 (TCP port 110).
- **TCP connection establishment:** Uses the SYN, SYN-ACK, and ACK three-way handshake.

## Conclusion

This lab helped me understand the differences between TCP and UDP, how port numbers identify network services, and how multiple protocols communicate across a network.