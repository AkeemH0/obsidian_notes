Involves the attacker sending a small request to an intermediary server or service, typically over UDP and manipulating the source IP address to appear as the victim's IP address. The intermediary server or service then responds with a larger response, thus amplifying the amount of traffic sent to the victim.
- UDP is a connectionless protocol meaning it doesn't establish a connection before transmitting data which makes it vulnerable to amplification attacks because it doesn't require a handshake like TCP
- UDP services that can be used for amplification typically include [[DNS (Domain Name System)]], [[NTP (Network Time protocol)]] , [[SNMP (Simple Network Management Protocol)]] and Memcached
- [[spoofed]] source IP, The attacker spoofs (fakes) the source IP address of the request packets to appear as the victim's IP address. this ensures that the amplified reponses are directed to the victim.
- amplification factor represents the ratio between the size of the request and the size of the response. E.G. in a DNS amplification attack, a small DNS query can trigger a much larger DNS response. This amplification factor magnifies the attack's impact.
- The victim is inundated (overwhelmed/overloaded/flooded) with amplified traffic from multiple intermediary servers or services, causing a network or service disruption in order to achieve network congestion and downtime which could lead to reputational or financial losses.


**Mitigating Amplification Attacks (UDP):**
- [[Packet Filtering]]
- [[Rate Limiting]]
- Application Layer Filtering
- [[Network Traffic Monitoring]]
- [[DNS Response Rate Limiting (DNS RRL)]]
- [[DDoS mitigation services]]