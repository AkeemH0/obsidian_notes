A registry file in Windows & Linux that contains URLs and corresponding IPs.
DNS resolutions check the host file contents first (takes precedence over local DNS cache ([[DNS request steps]]))
**Location:**
 - **Windows** C:\\Windows\\System32\\drivers\\etc\\hosts
 - **Linux** /etc/hosts

**Vulnerabilities:**
 - [[Hosts File manipulation]]

**Images:**
	**Windows Host file**
	![[Pasted image 20240219073352.png|Windows host file | Lines are commented out since its a sample and there are no domain name resolutions as they need to be added manually | Admins can add domain name resolutions|600]]
	**Linux CMD DNS query(dig)**
	![[Pasted image 20240219073900.png|dig | DNS query from Linux cmd line]]
	**Windows CMD DNS query (nslookup)**
	![[Pasted image 20240219074327.png|nslookup]]