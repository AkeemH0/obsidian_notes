 - Ensures data integrity by generating fixed-size short [[hash]] values (message digest/digital fingerprint) based on the original data. 
- Even a minor change in the data results in a significantly different hash value.
- one-way cryptographic function meaning its impossible to decrypt/reverse and obtain the original text due to the irreversible algorithms used
Intention: To create a unique ID for every single piece of data 
Use:
- Used for data integrity checks e.g. verifies that data hasn't been altered during transit
- Used to achieve efficient & secure storage e.g. password storage
- [[digital signature]]
E.G. When a file is published on the internet, the author may choose to publish the hash value for that file so that others can download it, generate a hash and verify that it's the same as the original.
Hash vulnerabilities:
- [[pass the hash]]
- [[Birthday attack]]
Vulnerability Countermeasures:
- [[Key stretching]]
- [[Salting]]
- [[Nonce (number used once)]]
- Limiting failed login attempts
Hashing algorithms:
[[MD5 (Message Digest 5)]]
[[SHA (Secure Hashing Algorithm)]]
[[RIPEMD (RACE integrity primitives evaluation message digest)]]
[[HMAC (Hash based message authentication code)]]

![[Pasted image 20231123145051.png]]


