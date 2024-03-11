**Definition:** 
 A communication protocol used to map an IP address to a physical [[MAC (Media Access Control) address]] on a local network.

A protocol used to translate an [[IP (Internet protocol)]] address to a physical [[MAC (Media Access Control) address]] . 
ARP is essential for communication between devices on the same local network segment such as Ethernet LAN as ARP helps with mapping the MAC address of the next or destination device.

*think of the ARP as the networks process for using a phonebook (ARP cache). When a device wants to call another device (send data), it needs the phone number (MAC address) corresponding to the name (IP address). ARP helps find and record these phone numbers so devices can communicate effectively.*
Steps:
1. [[ARP Request]] 
2. [[ARP Reply]]
3. [[ARP entry]] 
![[Pasted image 20240211174005.png|300]]


- Each device in a network stores MAC addresses of other devices in [[cache]]
- ARP operates at the [[2.Data Link Layer OSI]] of the [[Open Systems Interconnection (OSI)]] model & [[1.Network access Layer (TCP,IP)]]
- It is used to resolve the Layer 2 MAC address for a known Layer 3 IP address within the local network
- Each device on the network performs ARP and keep track of matching IP & MAC addresses in an ARP cache
- ARP messages are typically broadcasted within the local network to find the MAC address associated with a specific IP address
- ARP tables (also known as ARP caches) are maintained by devices to store recent mapping of IP addresses to MAC addresses which helps in reducing ARP broadcast traffic
- ARP spoofing or ARP poisoning is a security concern where malicious actors manipulate ARP to redirect network traffic to their own devices
- Mitigating ARP attacks: ARP inspection & dynamic ARP inspection are both methods to enhance network security 