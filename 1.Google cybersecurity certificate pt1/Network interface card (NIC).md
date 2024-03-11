Also known as a [[network adapter]] or [[network interface controller]].
A hardware component that enables a computer or other networked device to connect to and communicate over a computer network. The NIC serves as the interface between the computer's internal bus system and the network's communication medium, such as Ethernet cables or [[Wi-Fi (Wireless Fidelity)]] signals.
NICs receive and transmit network traffic but by default only listen to network traffic that's addressed to them.
- NICs can be integrated into a computers motherboard (integrated/Internal NIC) or installed as a separate expansion card (add-on/External NIC). They provide the physical and data link layer functions required to connect to a network.
- Operates at the [[2.Data Link Layer OSI]]. Responsible for framing data into packets, adding appropriate headers and trailers and managing the physical transmission and reception of data on the network medium
- Designed to work with specific network media types such as [[Ethernet]] or [[Wi-Fi (Wireless Fidelity)]]. Wired NICs use Ethernet Ports (e.g. RJ-45 connectors)
- Each NIC is assigned a unique [[MAC (Media Access Control) address]]which is a hardware address used for identifying the NIC on the network. MAC addresses are essential for addressing and routing data packets within the network.
- NICs require driver software to enable communication between the [[OS (operating system)]] and the hardware. These drivers facilitate the configuration and management of network settings
- NICs support various network speeds e.g. (10/100/1000 Mbps for Ethernet) and duplex modes (e.g. half duplex or full duplex). The choice of NIC and its settings affect network performance.
- NICs play a role in network security. They can be configured with security features such as [[MAC address filtering]] and [[VLAN (Virtual Local Area Network)]] support to control network access and enhance [[Network segmentation]]
- When troubleshooting network issues, problems with NICs such as driver conflicts or hardware failures are among the common areas to investigate.
- NICs can be set to [[promiscuous mode]] meaning that it accepts all traffic on the [[LAN (Local Area Network)]], even the packets that aren't addressed to the device

RJ-45 connector
![[Pasted image 20230916162318.png]]
![[Pasted image 20230916162418.png]
![[Pasted image 20230916162441.png]]