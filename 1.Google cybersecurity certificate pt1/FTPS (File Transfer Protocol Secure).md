**Definition:** 
 An extension of FTP that adds support for the Transport Layer Security (TLS) and Secure Sockets Layer (SSL) cryptographic protocols.
Port 989/990 TCP/UDP [[7.Application Layer OSI]]
A secure version of [[FTP (File Transfer Protocol)]] that enhances the security of traditional FTP by adding encryption. It's designed to protect the confidentiality and integrity of data transferred between a client and a server.
- FTP transmits data in plaintext making it vulnerable to interception and eavesdropping therefore FTPS employs encryption to secure data. 
- FTPS supports two encryption modes: 
- [[Implicit FTPS]]& [[Explicit FTPS]]: 
 both can be secured with [[SSL (Secure Sockets Layer)]]/[[TLS (Transport Layer Security)]]
- FTPS can use various authentication methods including username and password, client certificates, or a combination of both depending on the servers configuration.
-  In addition to encryption FTPS also ensures data integrity by detecting and preventing tampering during transfer 
- Used for transferring sensitive files between clients and servers, backup processes or updating website content securely.