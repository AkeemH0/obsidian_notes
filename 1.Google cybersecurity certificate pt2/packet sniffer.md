A tool designed to capture and analyse data traffic.
- Investigative tool used to monitor networks and identify suspicious activity
- Can be used maliciously to extract private information
- very loud on the network (easily detected)
How packet sniffers work:
- collected from the network via the [[Network interface card (NIC)]] which must be set to a mode that has access to all visible network data packets. In wireless interfaces this is often referred to as monitoring mode and in other systems it may be called [[promiscuous mode]].
- The packet sniffer must be positioned in an appropriate network segment to access all traffic between different hosts (start node is optimal to capture all incoming traffic (can also be configured to capture outgoing traffic))
- The packet sniffer then converts the raw binary format of the collected packet into a human-readable format.





Packet sniffers:
- SolarWinds NetFlow Traffic Analyzer
- ManageEngine OpManager
- Azure Network Watcher
- [[wireshark]]
- [[tcpdump]]
[[packet sniffing]]