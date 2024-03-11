A connection-oriented byte streaming service with ordering, error-checking, flow-control & the ability to handle multiple connections to the same device.
 - Occurs in  [[4.Transport Layer OSI]].
 - Uses a [[three-way handshake]] to establish a connection (connection oriented)
 - Uses a [[Sliding window mechanism]] for flow control
 - Uses [[Sequence Number (TCP)]] for ordering & error checking
 - one of the two main [[communication protocol]]s of the [[IP (Internet protocol) suite]]
 - Uniquely identifies conversations using: Source & Destination Address, Source & destination [[port]]
**Byte streaming service**: 
 either device can send a stream of bytes without having to think how they're broken into individual packets (TCP automatically breaks byte stream into smaller segments each of which fits into an IP packet)
 Connection-oriented: establishes TCP connection before sending data

**TCP data flow and transmission reliability**
	- TCP segments sent are in the form of 32-bit (4-byte) data.
	- Each TCP segment sent/received is tracked with a mark ([[ISN (Initial Sequence Number)]] for first flag (SYN), [[Sequence Number (TCP)]] for subsequent flags).
	- TCP waits for the recipients response after marking and sending segments to fill the [[Sliding window mechanism]].
	- TCP only sends the next set of data after receiving a response with the correct [[Sequence Number (TCP)]]
	- If TCP receives the incorrect [[Sequence Number (TCP)]] or the timeout period is surpassed or there are other indications of segment loss it retransmits the previous TCP segment
	- ![[Pasted image 20240214072017.png|TCP ensuring reliable, ordered & error-checked transmission|350]]
	- ![[Pasted image 20240217064705.png]]

**TCP general**
 - Offers reliable, connection-oriented communication, ensuring data delivery with error checking, sequencing and flow control mechanisms.
 - Known for its reliability and is commonly used for applications and services that require guaranteed data delivery such as web browsing, email and file transfers
 - Operates on top of the [[IP (Internet protocol)]] and is responsible for breaking data into smaller packets, ensuring they reach their destination in the correct order, retransmitting lost packets and managing flow control to prevent congestion.
 - The protocol assigns a [[port]] number to each communication endpoint, allowing multiple services to run on the same device and facilitating the proper routing of data.
 - TCP also includes mechanisms for congestion control, such as slow start and congestion avoidance to prevent network congestion and optimize data transmission
 - possibility of TCP-based attacks such as [[SYN flood attacks (targeting TCP)]].
 - error-checking: Incorrect Sequence number (packet data missing), surpassed timeout period (packet loss/network congestion) & other mechanisms (packets out-of-order (if packets take different speed routes))
 - confirms whether each TCP segment has/hasn't been received: if ACK not received data can be retransmitted
 - tracks [[Sequence Number (TCP)]] of each packet (maintains order & allows for duplicate packets to be removed)
 - Can handle multiple conversations (e.g. multiple data transfers between the same/any devices overlappingly). These conversations can also be bidirectional (swaps source & destination for addresses and ports)
 - Checksum field (TCP provides its own checksum)

**TCP key Features**
	- Ensures ordered, error-checked & controlled data transmission between two applications/entities.
	- Allows for multiple connections to the same applications/entities.
	- There is no data transfer before the connection is established.
	- Priority and security definitions can be made for the data sent.
	- Provides [[flow control]] involving a [[Sliding window mechanism]].
	- Retransmissions

**TCP connection termination (two-sided)**:
 1. terminating device sends FIN flag (finish) to target device
 2. target device responds with ACK
 3. target device responds with FIN flag
 4. terminating device sends ACK flag to target device
 5. **connection is terminated**
 ![[Pasted image 20240217071505.png|TCP connection termination|500x500]]

**TCP connection termination (one-sided)**
 1.  terminating device sends RST flag (reset) to target device
 2. **Connection is terminated**

**TCP Header**
 Image:
 ![[Pasted image 20240217071844.png]]
 - **Source Port Number**
 - **Destination Port Number**
 - **Sequence Number**
	The number used to track the transmissions of TCP segments. 
	If  "**SYN**" flag this number is the "**Initial Sequence Number**" value.
 - **Acknowledgement Number**
	A value that indicates up to which byte the transmission of the sent segments is made.
 - **Header Length (HLEN)**
	“**Header Length**” is the field that holds the value of the TCP header length.
 - **Reserved**
	A field reserved for future use.
 - **Control Flags**
	The field where the values ​​of the flags are kept. Each flag is "1 bit" long. Setting a flag means that it takes the value "1" in binary. In total, this field is “9 bits” long.
  - **SYN**: It is the flag used to initiate TCP connections.
  - **ACK**: It is the confirmation flag that indicates that the packets are transmitted. It also indicates to confirm the connection setup.
  - **FIN:** It is the flag used to terminate the TCP connection in a controlled manner.
  - **RST**: It is the flag used to terminate the TCP connection unilaterally and abruptly.  It is used to reset the connection.
  - **PSH**: It is the flag set in the packets where the data is sent to the target application.
  - **URG**: It is the flag used to notify that there is urgent and priority data.
 - **Window Size**
	 Maximum data size of the recipient’s buffer capacity is defined (varies due to [[Sliding window mechanism]]). 
 - **Checksum**
	The field used to checks whether the integrity of the TCP segment is intact during the transmission. 
 - **Urgent Pointer**
	A value that indicates up to which data the urgent bytes are. In order to use this field, the "URG" flag must be set. 
 - **Options**
	The field created to use various TCP protocol additional features. 

[[netcat]]