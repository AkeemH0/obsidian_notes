A packet is a small unit of data that carries information across a computer network.
[[data packet]]
Packets contain details such as source & destination IP, source & destination port number, Protocol identifier, Packet sequence Numbers, Header checksum, Time-to-Live (TTL), Payload, Header options, Fragmentation information, Flags and Control Bits, Quality of Service (QoS) Information.

Header contains 
 Destination & sender IP address, destination & sender MAC address ,Protocol Number , port number & packet size 

Body/payload contains  
 Contents of the packet (data)

Footer/trailer 
contains error-checking mechanisms like a checksum to ensure data integrity
 Signifies the end of a packet
 Most protocols (such as the [[IP (Internet protocol)]]) don't use footers
Ethernet protocol uses footers to provide error-checking information to determine if data has been corrupted. Ethernet network packets that are analysed might not display footer information due to network configurations.

- utilize [[routing table]]

[[IPv4 (Internet Protocol version 4)]] packet
![[Pasted image 20230917124708.png]]
The maximum size of an IPv4 packet is 65,535 bytes
Header
 - First 20 bytes (fixed): source & destination IP address, header length, total length of packet
 - Last 0 to 40 bytes (variable): options field
Body
  - 0-65,515 bytes 
  - Contains the message being transferred e.g. website information or email text
  
**The 13 fields of IPv4 packet header**
![[Pasted image 20230917125215.png]] 
Fields:
 - [[Version (VER)]]
 - [[IP Header Length (HLEN or IHL)]]
 - [[Type of Service (ToS)]]
 - [[Total Length]]
 - [[Identification (packets)]]
 - [[Flags]]
 - [[Fragmentation Offset]]
 - [[Time to Live (TTL)]]
 - [[Protocol]]: Tells the receiving device which protocol will be used for the data portion of the packet
 - [[Header Checksum]]
 - [[Source IP Address]]
 - [[Destination IP Address]]
 - [[Options]]
IPv4 vs IPv6 packet header
![[Pasted image 20230917192730.png]]
IPv6 offers more efficient routing and eliminates private address collisions that can occur on IPV4 when two devices on the same network are attempting to use the same address
Fields:
- [[Version (VER)]]
- [[Traffic Class]]
- [[Flow Label]]
- [[Payload Length]]
- [[Next Header]]
- [[Hop Limit]]
- [[Source IP Address]]
- [[Destination IP Address]]


[[PCAP (Packet capture)]]

[[packet sniffer]]s analyse [[packet]]s to find [[IoC (indicators of compromise)]]

[[network protocol analyser]]/[[packet sniffer]]

[[packet crafting]]

[[3.Network Layer OSI]],[[2.Internet Layer (TCP,IP)]] accepts & delivers packets for the network.