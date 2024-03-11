**Definition:** 
 An intrusion detection system that monitors network traffic for suspicious activity.

An application that collects and monitors network traffic and network data
NIDS Rules/signatures consist of 3 components:
- Action: 
  - Determines the action to take if the rule criteria is met. 
  - Alert, pass, drop(also generates an alert but drops the traffic) or reject.
- Header: 
  - Source and destination IP addresses. 
  - Source and destination ports. 
  - Protocols. 
  - Traffic direction
![[Pasted image 20231224154926.png]]
- Rule options: 
  - Customise signatures with additional parameters.
  - E.G. match content of packet to detect [[malicious payload]]s
  - Contained in brackets & separated by semi-colons
   ![[Pasted image 20231224155224.png]]




![[Pasted image 20231224145901.png]]