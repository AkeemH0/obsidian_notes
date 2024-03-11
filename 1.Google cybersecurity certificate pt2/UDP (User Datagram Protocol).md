**Definition:**
 A connectionless communication protocol in the internet protocol suite, offering minimal overhead for data transmission.
 -one of the two main protocols of the [[IP (Internet protocol) suite]]

Provides connectionless (doesn't establish connection), unreliable (doesn't ensure delivery or order of packets) communication with minimal overhead. UDP is used when real-time or low-latency data transmission is more critical than reliability. Applications like VoIP, online gaming and streaming media often use UDP. Occurs at [[4.Transport Layer OSI]].

- Doesn't include features such as error checking, sequencing or flow control. This means data sent via UDP may not always arrive in the same order it was sent and there is no mechanism for ensuring that all data packets are received.
- Associated with the "best-effort approach", meaning it does its best to deliver data quickly but does not guarantee reliability or delivery confirmation. It is up to the application layer to handle error recovery if needed.
- Vulnerable to issues like data loss, duplication and [[amplifications attacks (using UDP)]]

**Header**
 ![[Pasted image 20240218082727.png]]
 **Checksum:** Optional field unlike in TCP (forced). Contains hexadecimal value used for checking whether integrity has been upheld (packet intact during transit).

**Key features:**
 - No connection setup before transmission
 - Fast transmission
 - Doesn't guarantee data transmission
 - Contains less data in the header structure
 - often used for real-time non-critical scenarios (gaming, video calling, streaming, IOT)
 - No error checking (can't check if data is missing or if packets are unordered)
 - No flow control

**Analogy**
 *Like mailing postcards without: confirmation of receipt & no order for the postcards. You can't be sure the postcards are received & that they are sent in the correct order but its fast.

![[Pasted image 20240218112733.png|UDP communication]]
![[Pasted image 20240218083303.png|UDP parameters (wireshark)]]