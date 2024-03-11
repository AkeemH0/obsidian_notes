**Definition:**
 A comprehensive approach to security management that combines SIM (Security Information Management) and SEM (Security Event Management) functions.

- An application that collects and analyses log data in real-time to monitor critical activities in an organization. 
- Real-time visibility, event monitoring & analysis and automated alerts in a centralised location. 
- Analyse log data sourced from [[IDS (Intrusion detection system)]], [[IPS (Intrusion prevention system)]], [[Firewall]]s [[VPN (Virtual private network)]]s, [[proxies]] & DNS logs 
- SIEM tools index and reduce the amount of logs that a security analyst would manually have to review and analyse thus increasing efficiency and saving time. 
- provides a list of network vulnerabilities along with the priority of each vulnerability (the higher the vulnerability the shorter the deadline for mitigation)
- SIEM tools collect security event data (authentication attempts, network activity etc.) so it all appears in one place for analysts to analyse, this is referred to as a "single pane of glass".
- can create automated reports
- SIEM tools only report on possible issues and don't take actions to stop or prevent suspicious events however AI & Machine learning SIEMs could solve this issue
- AI & machine learning are improving SIEM capabilities and will enhance security as actions could be performed automatically without waiting for human response & threats may be located more easily/quicker using AI & machine learning technologies.
- SIEM tools can act as a system for data retention.
- Used for data correlation
- Used for [[Digital Forensics]] as logs can be stored for a long time

Steps:
- Collect and aggregate data: SIEM tools collect data (using :[[Log ingestion]], [[agent]] or [[agentless]] software) from sources such as firewalls, servers and routers. Logs are aggregated into one centralized location eliminating the need for manual review as all data is accessible in one location (the SIEM). Parsing can occur at this stage (data is mapped according to their fields and corresponding values e.g. same host, same port number, same source Ip)
  
- Normalization: Collected data undergoes normalization, converting it into a standard structured format that is easily searchable 
  
- Analysis: SIEM tools analyse the collected, aggregated and normalized data using detection logic, including predefined rules, Correlation comparing multiple log events to identify patterns, is a crucial part of the analysis process.
  
[[SIEM dashboards]]
[[SOAR (Security orchestration, automation, and response)]]

SIEM Tool types:
- [[Self-hosted SIEM]]
- [[Cloud-hosted SIEM]] 
- [[Hybrid SIEM]]

SIEM applications:
[[Splunk enterprise]]
[[Splunk cloud]]
[[Chronicle]]

[[playbook]]

[[log analysis]]