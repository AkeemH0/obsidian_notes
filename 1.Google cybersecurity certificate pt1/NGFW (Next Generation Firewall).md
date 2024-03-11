**Definition:** 
 A firewall that integrates additional features such as IPS, application control & URL filtering beyond traditional packet filtering.

- [[7.Application Layer OSI]] Analyses all packets throughout advanced decodes and performs security actions based on pre-set rules
- Not fully dependent on the port number as it looks at the application layer so it can block certain URLS
- Provides stateful inspection of incoming and outgoing traffic from applications
- Performs Deep packet inspection- a type of sniffing that examines data packets bodies and takes actions if threats exist
- Performs intrusion protection- detect security threats and notify firewall administrators
- Connect to cloud based threat intelligence services (so that they can quickly update to protect against emerging cyber threats)
- can inspect traffic at the [[4.Application Layer (TCP,IP)]] or [[7.Application Layer OSI]] and are typically application aware  (has the capability to understand and make decisions based on the specific applications or services that are using the network) therefore NGFWs can block or allow traffic based no the application rather than based on the IP address and ports like traditional firewalls do.
- Some NFGWs have additional features like Malware sandboxing, Network Anti-Virus and URL and DNS filtering
![[Pasted image 20240124172624.png|NGFW|400]]
![[Pasted image 20240212114405.png|NGFW]]