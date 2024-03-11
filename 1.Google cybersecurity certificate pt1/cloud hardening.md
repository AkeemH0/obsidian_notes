- implement [[Principle of least privilege (POPL)]] to services & users
- implement [[EDR (Endpoint Detection and response)]] 
- Have [[backups (security architecture)]]

[[IAM (Identity and Access Management)]]
[[Cloud configuration]]
[[CSP (cloud service provider)]]s offer numerous applications and services however each application or service carries its own set of risks and vulnerabilities and may increase and organizations overall [[attack surface]] as there will be more entry points into an organizations network if the network isn't designed correctly.
an increased attack surface must be compensated for with increased security measures
entry points can be used to introduce malware onto the network and pose other security threats
[[CSP (cloud service provider)]]s often tend towards more secure options compared to a traditional on-premise network as they supply for various organizations and one security flaw would be far more catastrophic than a single on-premise network failing as every company using the CSP would have the same security flaw. 

CSPs are more likely to know about a [[zero-day]] attack occurring before a traditional IT organization does.
CSPs have ways of patching [[hypervisor]]s and migrating workloads to other virtual machines
These methods ensure the customers are not impacted by the attack.
There are also several tools available for patching at the operating system level that organizations can use.


**Visibility and tracking**
Network admins have access to every data packet crossing the network with both [[on-premise networks]] & [[Cloud network]]s meaning they can sniff and inspect data packets to learn about network performance or to check for possible threats and attacks.

This visibility is also offered in the cloud through flow logs and tools, such as packet monitoring.
CSPs take responsibility for securing the cloud but they do not allow organizations to monitor traffic on the CSPs servers which may be a concern for organizations that are accustomed to having full access to their network and operations.

CSPs offer strong security measures to protect their infrastructure .

CSPs pay for third-party audits to verify how secure a cloud network is and identify potential vulnerabilities.
This can help organizations identify whether any vulnerabilities originate from on-premise infrastructure or if there any compliance lapses from their CSP.

CSPs have to stay up-to-date with technology advancements meaning organization configurations may need to change often based on CSP updates for security reasons so that they align with the CSPs standards.

Adding services adds to the complexity of the security of the organization and can increase the [[attack surface]] if implemented incorrectly. Adding more services will also require more security personnel to monitor all of the cloud services

[[shared responsibility model]]

[[IAM (Identity and Access Management)]]

[[Cloud Baselining]]

[[cryptography]] : can be applied to secure data that is processed and stored in a cloud environment. Uses [[Encryption]] and secure [[key management]] systems to provide data  [[Integrity]] and [[Confidentiality]]. [[cryptographic]] encryption is one of the key ways to secure sensitive data and information in the cloud.
[[cryptographic erasure]]

