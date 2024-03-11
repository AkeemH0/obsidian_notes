Users trying to access the legitimate website are redirected to the fraudulent site
Can be done by:
- Manipulating a DNS server's cache to associate a legitimate domain name with a malicious IP address. difficult to do as they are usually secured and configured properly
*Injecting false DNS records into a DNS cache*
- Modifying the client host files that take precedence over DNS queries (like a cache of IPs and URLs so that the computer resolves without having to query a DNS server)
- Sending a fake response to a valid DNS request, real-time redirection of the original request or resulting response ([[On-path attack]])
- ![[Pasted image 20240118130900.png]]