- A network security device that monitors & manages traffic to & from your network. 
- Firewall security rules are configured by the organization & often reside between the secured & controlled internal/private network and the untrusted external/public network e.g. internet. 
- Firewall maintenance should be carried out regularly to stay ahead of potential threats
- Some firewalls can be used as [[VPN Concentrator]]s 
- Many firewalls operate like layer 3 devices ([[Router]]s). Therefore able to perform [[NAT (Network address Translation)]] & [[dynamic routing]]
- Often positioned at the entrance/exit of the network
- The firewall [[ACL (Access control list)]] has a logical path for following rules (usually top-to-bottom) (therefore more specific rules are usually at the top of the rule list). e.g. Allow/Disallow based on ([[Packet Filtering]])) source IP, Destination IP (IP filtering), port number ([[Port Filtering]] e.g. deny TCP/80), time of day, application, group (e.g. if any of the rules associated with a database injection are identified, block all traffic from the source IP ) etc.
- [[implicit deny]] at the bottom of the [[ACL (Access control list)]] (will deny packet if it doesn't follow any of the previous rules)(usually default configuration for firewall)
- [[4.Transport Layer OSI]]/[[3.Network Layer OSI]]
**Types of firewall**
  - **[[Hardware firewall]]** 
  - **[[Software firewall]]**
  - **[[Clouds based firewall]]**


  - [[NGFW (Next Generation Firewall)]]
  - [[Stateful firewall]]
  - [[Stateless firewall]]
stateful & stateless firewalls can only inspect a packets header whilst NGFW firewalls inspect a packets body as well.
[[screened subnet]]
![[Pasted image 20230908122424.png]]
can be used to protect against [[IP Address spoofing]] by configuring a firewall to reject all incoming traffic (from external/public network) that has the same IP address as the local network
![[Pasted image 20240212171332.png|firewall rule list example]]
8. ALL ANY ANY ANY DENY ([[implicit deny]])