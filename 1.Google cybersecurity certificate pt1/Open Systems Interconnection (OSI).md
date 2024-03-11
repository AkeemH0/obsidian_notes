A conceptual framework used to understand and standardize how different networking protocols and technologies interact in network communication, which is useful for communicating where disruptions or security threats occur in a network. It consists of seven distinct layers, each responsible for specific functions in the network communication process. (Bottom=Layer 1 , Top = Layer 7). Data is transmitted throughout each layer.
1. [[1.Physical Layer OSI]] Hubs, Fibre , WIFI, ethernet, fibre optic, [[Network interface card (NIC)]]  (bits)  (best represent physical topologies)
2. [[2.Data Link Layer OSI]] ARP, VLAN, Ethernet, Switch , MAC (physical addressing), (frames (+Mac address, trailer (for error checking), payload))) (LLC (Logical link control), flow control, error correction services, synchronization of transmissions (when the bits start and stop(isochronous: external device for clocking, asynchronous: use own internal clocks & start/stop bits, synchronous: Clocking is shared between sender and receiver over separate channel))  (best represent logical topologies) ([[ARP (address resolution protocol)]])
3. [[3.Network Layer OSI]] IP (logical addressing), ICMP, IPsec, Routers, firewall , (packets (+ IP address)) (packet switching (actively routing/forwarding packets across routers)) 
4. [[4.Transport Layer OSI]]  TCP, UDP, firewall, ([[segment]]s (manage end-to-end communication between two devices while packets are used for routing and transmitting data across networks) ([[flow control]]) ([[Windowing]] , [[Sliding window mechanism]], [[checksum]], error checking, [[buffer]]/[[buffering]] ) (establishes [[port]]numbers)
5. [[5.Session Layer OSI]] (Session management: establishing, maintaining and terminating sessions) (synchronization: ensuring data is delivered in the correct order and pace, especially important in scenarios where multiple conversations are happening concurrently)
6. [[6.Presentation Layer OSI]] (data formatting, syntax, encryption/decryption,  )
7. [[7.Application Layer OSI]] (Protocols, services/processes, service advertisement e.g. Bluetooth headphones, apple airdrop) DHCP
*Penguins dive near the south pole annually* 
physical data network transport session presentation application
*big fluffy penguin splash* 
bits (physical layer) frames (data layer) packets (network layer) segments (transport layer)
Physical, transmit raw bits of data
Data link, transforms raw bits into frames to ensure they reach the right destination
Network, Route data frames across different networks
Transport, handles end to end communication between two nodes
Session
presentation
application