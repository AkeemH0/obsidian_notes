**Definition:** 
 A hierarchical system translating human-readable domain names into numerical IP addresses used for computer communication on the internet.
Port 53 TCP/UDP [[7.Application Layer OSI]]
A decentralized hierarchical system for translating human-friendly domain name/[[URL (Uniform Resource Locator)]]s into [[IP (Internet protocol)]] addresses. When a client device wishes to access a website domain using a web browser a query is sent to a DNS server. The DNS server corresponds the domain name to an IP address & sends it back to the clients device.
- DNS operates at the Application Layer (Layer 7) of the OSI model
- DNS plays a fundamental role in internet communication by resolving domain names to IP addresses, making it easier for users to access websites and other resources using familiar domain names rather than numerical IP addresses.
- DNS servers [[DNS server]] are categorized into two main types: [[recursive DNS resolver]] and [[authoritative DNS server]]. Recursive resolvers are responsible for querying authoritative DNS servers to resolve domain names.
- decentralized: no single party is responsible for providing nameservers at each level (distributed databases/servers)
- Threats include [[DNS Spoofing attack]] 
- [[DNSSEC (DNS Security Extensions)]] prevents unauthorized changes to DNS records (counters [[DNS poisoning]] )
- Uses [[UDP (User Datagram Protocol)]] however if the reply to a request is too large (>65,535 bytes) it will switch to using [[Transmission control protocol (TCP)]] 
- emails are also domain names e.g. bob@gmail.com
- googles main dns servers have IP 8.8.8.8 & 4.4.4.4
[[DNS CMD commands]]
[[DNS request steps]]
[[DNS records]]
[[DNS hijacking]]
[[Hosts File manipulation]]
[[URL hijacking]]
**DNS Wireshark**
 ![[Pasted image 20240219071957.png|DNS query for letsdefend.io]]
 ![[Pasted image 20240219072053.png|DNS response for letsdefend.io]]

[[host file]]