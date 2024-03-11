A **random 32-bit number** set by TCP during connection establishment
- Used for **the first data transfer** on the TCP connection
- Then, new numbers are created by **adding the number of bytes** sent on this number creating the next [[Sequence Number (TCP)]]
- If the sequence number is incorrect or not received, data transfer would not continue and the previously sent TCP segment would be resent.