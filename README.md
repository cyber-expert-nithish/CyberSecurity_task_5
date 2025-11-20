# Task 5 – Wireshark Packet Capture and Analysis

Student: R Nithish Ram  
Course: Cyber Security Internship  
Tool: Wireshark 4.6.1  
File: Task5 Wireshark.pcapng

Objective
To capture live network traffic, identify common protocols (DNS, TCP, TLS, ICMP), and analyze selected packets to understand how communication happens over the internet.

 Protocols Observed
- DNS: Domain name lookup (e.g., chatgpt.com, googleapis.com)
- TCP: Reliable communication with sequence/ACK flags
- TLSv1.2/TLSv1.3: Encrypted HTTPS traffic (Client Hello, Server Hello)
- ICMPv6: Ping echo request/echo reply
- QUIC: Modern encrypted transport protocol used by Google services



Filters Used

dns
tcp
tls
icmpv6


Packet Analysis (Summary)

 1. DNS Packet
- Source: 10.107.13.170  
- Destination: local DNS server  
- Query: chatgpt.com  
- Purpose: resolve domain to IP

 2. TCP Packet
- Source Port: 443  
- Destination Port: 51722  
- Flags: PSH, ACK  
- Purpose: carries encrypted HTTPS data

 3. TLS Packet
- Type: Client Hello / Server Hello  
- Purpose: negotiate encryption and establish secure session



 Files Included
- Task5 Wireshark.pcapng
- Task5_Report.pdf

## Conclusion
The capture successfully recorded DNS lookups, TCP flows, TLS handshakes, and ICMPv6 packets. This demonstrates real-time internet communication and the role of encryption in protecting data.
