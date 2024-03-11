A type of [[DoS (Denial of service)]]/[[DDoS (distributed denial of service attack)]] that specifically targets TCP

- In a SYN flood attack, the attacker sends repeated SYN packets to every port on the targeted server, often using a fake IP address. 
- The attack exploits the [[three-way handshake]] process that TCP uses to establish a connection between two devices.
- SYN (synchronize) packets are sent to create a new TCP connection
- The server responds with a SYN-ACK (synchronize-acknowledgement) packet & reserves resources for the source to connect (half open port)
- The client responds with an ACK (acknowledgement) packet thus establishing a connection between the client and server, allowing them to exchange data.
- Since in a flood attack the attacker sends repeated SYN packets the servers resources become consumed with maintaining these half-open connections which can lead to resource exhaustion by overwhelming TCP ports, memory or processing capacity meaning legitimate users' requests cannot be serviced because the server's resources are overwhelmed, leading to service unavailability and downtime, causing financial losses and reputation damage.
- If the number of SYN requests exceeds the number of available ports on the server the server will become overwhelmed and unable to function

**Mitigating SYN flood Attacks (TCP):**
- SYN cookies
- [[Rate Limiting]]
- [[Firewall]]
- [[IDS (Intrusion detection system)]]
- [[IPS (Intrusion prevention system)]]
- [[Load balancing]]



[[wireshark]]

