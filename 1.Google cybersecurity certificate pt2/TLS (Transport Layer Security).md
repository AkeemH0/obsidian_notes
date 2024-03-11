**Definition:** 
 A cryptographic protocol used to secure communication over a computer network, succeeding the obsolete SSL.

A [[cryptographic]] protocol used to secure communications over a network, typically the Internet. TLS provides encryption, data integrity and authentication mechanisms, ensuring that data transmitted between two parties remains confidential and tamper-proof.
- TLS is the successor to [[SSL (Secure Sockets Layer)]] and is often **referred to as** **SSL/TLS**. It is used to establish secure connections between a client (such as a web browser) and a server (such as a website) or between two servers.
- TLS encrypts data in transit, preventing eavesdroppers from intercepting and deciphering sensitive information exchanged between parties. This encryption is achieved through a combination of symmetric and asymmetric cryptography (asymmetric for sending symmetric key, symmetric for further communications).
- Data integrity is ensured by TLS through the use of hash functions and digital signatures. This prevents data from being tampered with during transmission
- TLS also provides authentication, verifying the identity of the server (and optionally the client) involved in the communication. This authentication helps prevent [[MITM (man-in-the-middle) attack]]
- TLS is commonly used to secure various Internet Services, including [[HTTPS (Hypertext Transfer Protocol Secure)]]] for secure web browsing, [[SMTP (Simple Mail Transfer Protocol)]] with [[STARTTLS]], [[SMTPS (Simple Mail Transfer Protocol Secure)]] for secure email transmission and [[IMAPS (Internet Message Access Protocol Secure)]] for secure email retrieval 
- TLS certificates issued by trusted Certificate Authorities (CAs) play a crucial role in the authentication process. Websites and servers use these certificates to prove their identity to client.
- TLS is essential for ensuring secure communications in various online transactions including online banking, e-commerce and data transfer.