- A service that allows anyone to analyse suspicious files, domains, URLs & IP addresses for cybersecurity threats such as malware.
- Users can submit and check artifacts (e.g. file hashes or IP addresses) to get reports on whether an [[IoC (indicators of compromise)]] is considered malicious or not & how that IOC is connected to other IOCs in the dataset.![[Pasted image 20231223080035.png]]
1. Detection: 
   A list of third-party security vendors and their detection verdicts on an IoC e.g. vendors can list their verdict as malicious, suspicious, unsafe etc.
2. Details: 
   Provides additional information extracted from a static analysis of the IOC such as different hashes, file types, file sizes, headers, creation time & first and last submission.
3. Relations: 
   Related IOCs that are somehow connected to an artifact, such as contacted URLs, domains, IP addresses and dropped files if the artifact is an executable.
4. Behaviour: 
   Contains information related to the observed activity and behaviour of an artifact after executing it in a controlled or sandboxed environment. Includes: tactics & techniques detected, network communications, registry and file system actions & processes.
5. Community: 
   Where security professionals or researchers leave comments and insights about the IOC
6. Vendors' ratio and community score: 
 -  Vendors' ratio shows how many security vendors have flagged the IOC as malicious. 
 - Community score is based on the inputs of the VirusTotal community. 
 - The more detections a file has and the higher its community score is, the more likely that the file is malicious.
   
   Note: data uploaded to VirusTotal will be publicly shared with the entire VirusTotal community therefore do not upload personal/private information.