- Division of an [[IP (Internet protocol)]] address into network and host portions. 
- Helps determine which parts of an IP address identifies the start of the **network** and which part identifies individual **hosts** within that network. 
- Helps indicate the size of the host network
e.g /24
192.146.53.101
192.146.53.102
For example these two IPs are of the same network but have different hosts (devices) therefore the subnet mask for these would look like this:
255.255.255.0 
since the first 3 sections are for the network and the last section is for the host
which is 11111111.11111111.11111111.00000000 in binary
- 1s represent the network section
- 0s represent the host section

- Subnet masks allow for the larger division of larger IP addresses into smaller more manageable subnets helping an organization to manage traffic and security
- [[default gateway]] device usually ends in (4th octet) .1 or .254 
- Routers use subnet masks to determine how to forward data packets; by knowing the network portion of an IP address, routers can make decisions about where to send data within a network.
