TCP communication mechanism
- [[flow control]]
- The window size determines the maximum amount of unacknowledged segments that can be in transit at any one time
- The receiver advertises its available buffer space through the window size field in the TCP header
- This helps avoid network congestion throughout dynamically adjusting the senders transmission rate in response to the receivers dynamically adjusting window size
- Allows a sender to transmit several segments simultaneously without waiting for an acknowledgement for each individual segment
- The receiver maintains a window of acceptable sequence numbers (provided by the sender initially & as the communication progresses), acknowledging all correctly received segments within that window & can request for retransmissions (if segments are lost or arrive out of order)
- requires correct Acknowledgement (ACK) of retrieval before sending the next group of segments