[[IDS (Intrusion detection system)]] & [[SIEM (Security information and event management)]] tools collect and analyse [[event]] data to identify potential unusual activity
If an incident is [[Detect]]ed (such as a malicious actor successfully gaining unauthorised access to an account) then an alert is sent out
During the [[Analysis (IR)]] process security analysts examine [[IoC (indicators of compromise)]] to determine whether an incident has occurred

Challenges:
- Its impossible to detect everything:
   Detection tools can only detect what security teams configure them to monitor, so if they aren't configured properly, they can fail to detect suspicious activity leaving systems vulnerable to attacks. Therefore it's important for security teams to use additional methods of detection to increase their coverage and accuracy ([[Defence in depth]]).
   (since some incidents are unavoidable [[IRP (incident response plan)]]s are crucial)
- High volumes of alerts (often caused by misconfigured alert settings (e.g. alert rules that are too broad and not tuned to an organizations environment create false positives) or malicious actors taking advantage of a newly discovered vulnerability)

Detection methods:
[[Threat hunting]]
[[Threat intelligence]] 
[[Cyber deception]]