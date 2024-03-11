A pattern that is associated with malicious activity E.G. A sequence of binary numbers, bytes & IP address

Signature components:
 - Action: 
   - Determines the action to take if the rule criteria is met. 
   - Alert, pass, drop (also generates an alert but drops the traffic) or reject.
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
   - Have a specified ordering and changing their order would change the meaning of the rule
   ![[Pasted image 20231224155224.png]]
![[Pasted image 20240212172857.png|conficker worm signature example|450]]