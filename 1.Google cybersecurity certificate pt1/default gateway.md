A network device that serves as an entry point or exit point for traffic between a local network and external networks (typically home router)e.g. the internet. Usually has .1 or .254 as the final IP octet . Helps in routing data packets between different networks. The gateway determines the appropriate path for the data to reach its destination. The default gateways [[IP (Internet protocol)]] address is within the same [[subnet]] as the devices on the local network (serves as the [[Next hop]] for outgoing traffic).

like a router that can be used in all layers of the OSI model
connects networks throughout packet transfer

[[subnet mask]] identifies which part of the IP address represents the network,  which part represents the host & the default gateway. Devices use the subnet mask to determine if a destination IP address is on the same local network or if it needs to be sent to the default gateway for routing.

For devices on a [[LAN (Local Area Network)]] they need their default gateway set to the IP address of the router that connects the LAN to the internet 
[[3.Network Layer OSI]]

*like a traffic cop for a network that determines an appropriate path for packets (cars) to reach the right place*
![[Pasted image 20240207204029.png]]
[Default Gateway Explained (youtube.com)](https://www.youtube.com/watch?v=pCcJFdYNamc)