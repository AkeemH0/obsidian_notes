Also known as recursive [[DNS server]]s or [[DNS resolver]]s.
Responsible for helping clients (e.g. computer or smartphone) resolve domain names into IP addresses by recursively querying authoritative DNS servers.
Usually provided by ISPs
- When a web address is inputted into a web browser the devices sends a DNS query to a recursive resolver to find the IP address associated with that domain
- The resolves traverses the DNS hierarchy. They first check their own cache for the requested domain-to-IP mapping. If it's not found or has expired, they start querying the DNS infrastructure from the root DNS servers, through the top-level domain (TLD) servers and down to the authoritative DNS server responsible for the specific domain
- Recursive resolvers are crucial for the overall functioning of the internet and DNS. They handle a large volume of DNS queries daily and play a role in improving DNS performance and reliability by caching DNS records for a certain period, reducing the need to repeatedly query authoritative servers.
- Recursive resolvers are potential targets for DNS-related attacks, such as [[DNS poisoning]] or [[DDoS (distributed denial of service attack)]]