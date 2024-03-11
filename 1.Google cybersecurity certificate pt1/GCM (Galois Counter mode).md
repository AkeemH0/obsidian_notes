**Definition:** 
 A mode of operation for symmetric key cryptographic block ciphers, providing authenticated encryption and integrity.

[[Encryption]] with [[Authentication]]
- Authentication is part of the block mode
- Combines [[CTR (Counter)]] with Galois authentication 
Minimum latency (Minimum operation overhead)
- Very efficient encryption and authentication
Commonly used in packetized data
- [[Network]] traffic security ([[Wi-Fi (Wireless Fidelity)]], [[IPsec (Internet Protocol Security)]])
- [[SSH (Secure Shell)]], [[TLS (Transport Layer Security)]]

- Uses AES 
- [[Message Integrity]] check (MIC) using [[Galois message authentication code (GMAC)]]