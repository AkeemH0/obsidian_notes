Definition
 A data structure used by network devices to decide where to send data [[packet]]. Contains information on available routes/paths to reach specific destinations in a network.

*like a digital map that can only see adjacent places (nodes) & decides packets [[Next hop]] based on the closest place (longest sequence of similar characters in IP)) to destination ([[IP (Internet protocol)]]), once at the next hop a new digital map with the adjacent map is used.*


Components
 - Destination Network: Each entry in the routing tables specifies a destination network or [[subnet]]. This can be a specific [[IP (Internet protocol)]] address or a range of IP addresses represented as a network address and subnet mask [[CIDR (Classless Inter-Domain Routing)]]
 - [[Next hop]]: the IP address of the next router or network device that a packet should be forwarded to in order to reach the destination network. "Whoever carries out the last hop controls the network".
 - Interface: The physical or logical network interface through which the packet should be sent to reach the next hop. E.g. Ethernet interface, serial interface, virtual interface & etc. 
 - Metric or cost: Routing protocols use [[metric]]s or costs to determine the best path to a destination. Lower metrics indicate more efficient paths. metrics include hop count, [[Bandwidth]], delay and reliability

Routing Table entries (a route to a specific network): 
 - Static Routes: Manually configured set up by network administrators. Remain static unless modified by the administrator.
 - Dynamic Routes: Automatically update routing table based on network changes by utilising algorithms to calculate optimal paths e.g. [[OSPF (Open Shortest Path First)|OSPF (Open Shortest Path First)]] or Routing Information Protocol (RIP).

Routing table Decision Process:
 - When a network device ([[Router]]) receives a data packet it consults its routing table to determine the appropriate route for forwarding the packet.
 - The device matches the destination IP address of the packet with the entries in the routing table
 - It selects the entry with the most specific match (longest prefix match/string of characters match) or the lowest metric (if using dynamic routing)
 - The device then forwards the packet to the next hop specified in the selected routing table entry.

Security implications: 
 - Unauthorized changes to routing tables can lead to traffic interception or redirection e.g. [[MITM (man-in-the-middle) attack]]
 - Use [[ACL (Access control list)]] and authentication mechanisms to protect routing table modifications

- routing tables are used by routers and [[3.Network Layer OSI]] / [[1.Network access Layer (TCP,IP)]] switches to determine how to forward data packets.
- Routing table entries can contain both static and dynamic routes

