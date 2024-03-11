**Definition:** 
 A security tool that monitors network or system activities for malicious behaviour or policy violations.

- an application that continuously monitors system activity and produces alerts on possible intrusions.
- An IDS alerts administrators based on the signature of malicious traffic.
- IDSs are configured to detect known attacks.
- Usually integrated into [[NGFW (Next Generation Firewall)]]
- IDSs often monitor [[endpoint]]s
- IDSs sniff data packets as they move across the network and analyse them for the characteristics of known attacks
- some IDS systems review not only for signatures of known attacks but also for anomalies that could be a sign of malicious activity
- When the IDS discovers an anomaly it sends an alert to the network administrator who can then investigate further
- IDS can only scan for known attacks or obvious anomalies so new and sophisticated attacks might not be caught
- IDS doesn't stop/prevent incoming traffic if it detects something wrong so its up to the network administrator to catch the malicious activity before it damages the network
- IDS is placed in front of the LAN and behind the Router allowing IDS to analyse data packets that have already been filtered by the firewall to reduce the number of false positives.
- ![[Pasted image 20230920073943.png]]
- True positive: correctly detects the presence of an attack
- True negative: a state where there is no detection of malicious activity since malicious activity doesn't exist so no alert is triggered.
- False positive: Incorrectly detects the presence of a threat. When an IDS identifies an activity as malicious but it isn't. False positives are an inconvenience because they spend time and resources investigating an illegitimate alert
- False negative: A state where the presence of a threat is not detected even though there is malicious activity. Security teams are left unaware of legitimate attacks that they can be vulnerable to.
- Many IDS tools can also operate as an IPS e.g. Suricata, Sagan, Snort
- IDS logs
Types of detection methods:
- [[signature-based analysis]]
- [[Anomaly-based analysis]]
- Signature-based analysis & Anomaly-based analysis are often used in unison as they are complementary to one another
  
Types of IDS:
 - [[HIDS (Host-based intrusion detection system)]]
 - [[NIDS (Network-based intrusion detection system)]]
 - NIDS & HIDS are often used together to provide a multi-layered approach to intrusion detection and response & provide a comprehensive view of the activity happening in an environment.
