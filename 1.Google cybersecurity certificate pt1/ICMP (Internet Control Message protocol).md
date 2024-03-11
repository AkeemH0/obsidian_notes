**Definition:** 
 A network layer protocol used to send error messages and operational information about network conditions.

Utilized by devices to tell each other about data transmission errors across the network. used by a receiving device to send a report to a sending device about the data transmission. Used as a quick way to troubleshoot network connectivity and latency by issuing the "ping" command on a Linux operating system. Operates at the [[2.Internet Layer (TCP,IP)]]/[[3.Network Layer OSI]]

A network-layer protocol within the [[IP (Internet protocol) suite]]. ICMP is primarily used for sending error messages (for UDP & TCP e.g. destination unreachable or Time exceeded ([[Time to Live (TTL)]] surpassed)) and operational information about network conditions. It plays a crucial role in network diagnostics, error reporting, and providing feedback on the status of network devices.
- ICMP is commonly associated with utilities like "ping" and "traceroute" used for network troubleshooting. "ping" sends ICMP echo requests to test network connectivity, while traceroute uses ICMP time-exceeded messages to trace the path of packets across a network.
- ICMP includes various messages types, including echo requests and replies, destination unreachable messages, time-exceeded messages and redirection messages.
- "Ping flood" is a type of ICMP-based attack where attackers send an excessive number of ICMP echo requests to overwhelm a target system or network.
- ICMP can also be used for network scanning and reconnaissance (surveying to locate enemies), as attackers may send ICMP messages to discover live hosts or gather information about a network
- [[ping(ICMP)]]
- 