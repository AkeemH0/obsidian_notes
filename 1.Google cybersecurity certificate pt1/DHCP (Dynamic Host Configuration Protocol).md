**Definition:** 
 A network protocol that automatically assigns IP addresses and other network configuration information to devices on a network.
port 67/68 UDP [[7.Application Layer OSI]]
- DHCP Server listens on port 67 to receive DHCPDISCOVER & DHCPREQUEST from clients
- DHCP Client listens on port 68 to receive DHCPOFFER, DHCPACK, DHCPNAK from server
- Provides an [[IP (Internet protocol)]], [[subnet mask]], [[default gateway]] & [[DNS server]] for clients![[Pasted image 20240219114241.png]]

[[Router]] is usually used as DHCP server
Assigns a unique IP address & provides the addresses of the appropriate [[DNS server]] and [[default gateway]] for each device.
- IP addresses are temporarily assigned (unless an IP reservation is made) and must be renewed throughout a renewal request by the device (reduces the likelihood of the DHCP server  running out of IP addresses)
- IP reservations can be made by the network admin (using the DHCP Server management tool & devices mac address) and stored on the DHCP server (reserving IP addresses for certain devices makes it easier to trouble shoot and manage devices)
Steps:
1. DHCP Discover: When a device joins a network it sends out a request to see if there are any DHCP servers on the network
2. DHCP Offer: DHCP server replies back with IP address the device could use
3. DHCP Request: device sends a reply confirming it wants to use the IP address
Either:
4. 1. DHCP ACK: sends a reply acknowledging the assignment has been completed
4. 2. DHCP NAK: Negative acknowledgement - informs client that the requested IP address is not available.
![[Pasted image 20240211174452.png|350]]
![[Pasted image 20240218145340.png]]