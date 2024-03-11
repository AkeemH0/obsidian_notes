- A network device that connects multiple networks together.
- Has an integrated/Connects to a [[Modem]] (typically provided by ISP) for internet access
- Sit between networks and direct traffic,  based on the IP address of the destination network.
- IP address is contained in the IP header which is carried by the packet.
- Usually assigned 192.168.1.1 on a private home network
- Routers have several IP addresses (generally 1 public & 1 private)
- The router reads the header information and forwards the packet to the next router on the path to the destination updating the sender IP address to its own IP.
- This continues across many routers until the packet reaches the destination network.
- Routers often include [[Firewall]]s that allows or blocks incoming traffic based on information in the transmission which helps to stop malicious traffic from entering the private network and damaging the local area network.
- Used in LAN-to-WAN & LAN-to-LAN connections
- perform [[NAT (Network address Translation)]]
- [[3.Network Layer OSI]]
![[Pasted image 20240207202705.png]]


![[Pasted image 20240218150653.png]]

Here the private network has a router with private ip 192.0.2.1. 
This router is also known as the [[default gateway]] as it is the gate to internet access. 
The default gateway router will have a different public [[IP (Internet protocol)]] which will be used to communicate on the internet [[NAT (Network address Translation)]]