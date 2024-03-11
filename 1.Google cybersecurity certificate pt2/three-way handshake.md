TCP establishes a connection throughout a [[three-way handshake]]
1. The device who wants to establish the connection sends a TCP segment set to the SYN (synchronize) flag to a server/recipient. 
2. Server responds with a TCP segment set to the SYN/ACK (synchronize-acknowledgement) flag to acknowledge receipt of the device's request. 
3. The sending device sends a TCP segment set to the ACK (acknowledgement) flag to the server/recipient, establishing the connection.
SYN & ACK flags are 1 bit areas within the TCP protocol Header
![[Pasted image 20240214064344.png|three-way handshake|400]]