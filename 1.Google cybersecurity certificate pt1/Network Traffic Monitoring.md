Continuously monitor network traffic patterns to detect and respond to amplification attacks in real-time. Intrusion detection systems (IDS) and intrusion prevention systems (IPS) can be valuable in this regard.

Identify deviations from the [[baseline]]e.g. large and unusual data transfers .
Network components that can be monitored to detect malicious activity:
- Flow analysis:
  Monitoring the movement of network communications including packets, protocols and ports.
  Malicious actors can use non-standard ports for communication a technique known as [[command and control (C2)]] to maintain connections with compromised systems. Organizations must use port filtering and watch out for any mismatches between ports and their associated protocols in order to prevent C2.
- Packet payload information: packets contain details like source and destination IP address and the packet payload information. This data is encrypted and requires decryption for it to be readable. Organizations can monitor the payload information of packets to uncover unusual activity such as sensitive data transmitting outside the network which could indicate a possible data exfiltration attack.
- Temporal patterns: Network packets include time-related data, allowing analysis of temporal (time related) patterns. Normal network activity follows specific time patterns e.g. 9am to 5pm .Therefore sudden deviations from the [[baseline]], such as high traffic volumes outside normal operating hours, signify off-baseline activity and warrant investigation.
- [[network operations centre (NOC)]]
- [[SOC (Security operations centre)]]
- SPAN (switch port analyser mode) copies all VLAN traffic to one switch port