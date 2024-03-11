**Definition:** 
 A security tool that not only detects but also actively blocks or mitigates potential security threats.

- An application that monitors system activity for intrusive activity and takes action to stop the activity.
- It offers even more protection than an IDS because it actively stops anomalies when they are detected, unlike the IDS that simply reports the anomaly to a network administrator.
- Usually integrated into [[NGFW (Next Generation Firewall)]]
- An IPS reports the anomaly to security analysts and blocks a specific sender or drops network packets that seem suspect
- IPS rules are similar to [[Firewall]] with the addition of using [[signature]]s of known malware/attack patterns & data anomalies (unusual traffic patterns) to identify malicious traffic. 
- IPS [[ACL (Access control list)]] has a logical path for following rules (usually top-to-bottom) (therefore more specific rules are usually at the top of the rule list). e.g. Allow/Disallow based on ([[Packet Filtering]])) source IP, Destination IP (IP filtering), port number ([[Port Filtering]] e.g. deny TCP/80), time of day, application, group (e.g. if any of the rules associated with a database injection are identified, block all traffic from the source IP ) etc.
- Sits between the internal and external network 
- Can be either: [[HIDS (Host-based intrusion detection system)]] ([[agent]]) or [[NIPS (Network-based Intrusion Prevention System)]] ([[agentless]])
- Since its in-line if the IPS breaks the connection between the private network and the public network breaks
- false positives can result in legitimate traffic getting dropped
![[Pasted image 20230920073954.png|IPS in Network Topology]]
![[Pasted image 20240212172958.png|signature example (conficker worm)|400]]
![[Pasted image 20240212174619.png|IPS filter list|600]]