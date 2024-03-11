**Definition:** 
A set of rules governing the format of data sent over the internet, essential for data routing between devices.

A fundamental set of rules and conventions that govern how data packets should be routed, addressed, transmitted and received across computer networks, including the global network known as the internet. IP is essential for functioning of the internet and most other networks as it provides a standardized method for devices to communicate with each other.
*is like a name*

- Two versions of IP are prevalent: 
  - [[IPv4 (Internet Protocol version 4)]]
  - [[IPv6 (Internet Protocol version 6)]]
  
- [[Public IP]] addresses are globally routable on the internet
- [[Private IP]] addresses are reserved for use within private networks
[[localhost (loopback address)]]
- [[Subnetting]]
- [[NAT (Network address Translation)]]
- [[CIDR (Classless Inter-Domain Routing)]]
- [[Routing (Internet Layer)]]
- IP relies on other protocols such as: [[ICMP (Internet Control Message protocol)]] for error reporting & [[ARP (address resolution protocol)]] for mapping IP addresses to MAC addresses in local networks.
- Security measures include: [[Encryption]], [[Firewall]],  [[IDS (Intrusion detection system)]] , [[IPS (Intrusion prevention system)]]
- [[IPsec (Internet Protocol Security)]]
IP address ranges uses
![[Pasted image 20240209121741.png]]


Finding out which network the device is connected to
![[Pasted image 20240209121956.png]]
E.G. 192.168.4.1 & 192.168.4.2
Since the first bit is 192<=192<=223 both the IP addresses belong to class C
Since both the IP addresses have 192.168.4 as the first 3 octets they are part of the same network
Since the IP addresses end with a different octet they are different hosts/devices 

[[subnet mask]] for class:
A 255.0.0.0
B 255.255.0.0
C 255.255.255.0