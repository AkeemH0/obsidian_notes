**Definition:**
 An approach to networking that uses software-based controllers or application programming interfaces (APIs) to direct traffic on the network.

Data/control/management planes coded as software
Data plane: process network frames and packets - forwarding, trunking, encryption, [[NAT (Network address Translation)]]
Control plane: manages the actions of the data plane - routing tables, session tables, NAT tables, dynamic routing updates
Management plane: Configure and manage the device - SSH, SNMP, Browser, API


A network architecture that separates the [[Control plane]] from the [[Data plane]]. It utilises a centralized controller to manage network policies, enabling dynamic and flexible network management. 
SDN enhances security by allowing real-time updates to security policies and configurations across the network. 
Just like CSPs provide virtual computers, many SDNs also provide virtual switches routers and firewalls. 
In the case of [[Cloud network]]ing SDN tools are hosted on servers located at the CSPs data centre.
SDNs enable dynamic, programmatically efficient network configurations to improve network performance and monitoring.

![[Pasted image 20240123201552.png]]
![[Pasted image 20240123201635.png]]