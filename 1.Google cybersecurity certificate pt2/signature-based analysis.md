- A detection method used to find events of interest

- A [[signature]] specifies a set of rules that an IDS refers to when it monitors activity, If the activity matches the rules in the signature the IDS logs it and sends out an alert E.G. A signature can be made to generate an alert if a failed login occurs X amount of times on the same account.

- [[Pyramid of Pain]] can be useful for creating targeted signatures to detect and block attacks based on [[IoC (indicators of compromise)]]

Signature Advantages:
  - Low rate of false positives: very efficient at detecting known threats because it's simply comparing activity to signatures, leading to fewer [[False positive]]s. 
Signature Disadvantages:
- Can be evaded: attackers can slightly modify malware code to alter its signature and avoid detection.
- Require regular updates: Each time a new exploit or attack is discovered new signatures must be created and added to the signature database
- Inability to detect unknown threats: New malware families ([[malware family]]) & [[zero-day]] attacks cannot be detected.

Signature components:
 - Action: 
   - Determines the action to take if the rule criteria is met. 
   - Alert, pass or reject.
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
