**Definition:** 
 A framework that manages digital keys and certificates, enabling secure communication. A hierarchical system for the creation, management, storage, distribution and revocation of digital certificates.

Summary
 - An encryption framework that secures the exchange of information online by utilising digital certificates to authenticate using asymmetric encryption. PKI governs encryption keys by issuing and managing these digital certificates. Digital signing helps ensure that data comes from a legitimate source and hasn't been altered in transit. An entire system based on hardware, software, procedures and people that is based on [[asymmetric encryption]]. System that creates the asymmetrical key pairs that consist of those public and private keys that are used in the encryption and decryption process.
- **PKI authenticates you and your server**
   Allows site users' web browsers to authenticate your server before connecting to it, so is can verify that they're connecting to a legitimate server. You can also use client certificates to limit access to authenticated users, which gives greater control over your network and other IT systems.
- **PKI facilitates encryption and decryption**
   Uses digital certificates and key pairs to encrypt and decrypt data
- **PKI ensures the integrity of your data**
 - Protects against data tampering by facilitating digital signatures to confirm that it has come from a specific identity.
 - Uses a mathematical algorithm to generate two long keys (one public and one private)
 - Combines cryptographic technologies (digital signatures, asymmetric encryption, hash functions) and procedures ([[CA (Certificate Authority)]]) to secure data and authenticate entities
 - The hardware, software, policies, processes and procedures required to create, manage, distribute, use, store and revoke digital signatures and public keys.
 - Backbone of digital certificate systems that confirm the identity of people devices and applications
 1. Exchange of encrypted information ([[symmetric encryption]] &or [[asymmetric encryption]]). Can use either encryption or both in conjunction depending on whether speed or security is the priority
 2. Establish trust using a system of [[digital certificate]]s
 3. Used for [[digital signature]]s
[[Key escrow]]
[[CA (Certificate Authority)]] 
[[RA (registration Authority)]] 
[[Certificate store]] 
[[Validation Authority (VA)]]
[[public key cryptography]]
Uses:
 - [[Wi-Fi (Wireless Fidelity)]] authentication 
 - web - a padlock icon in your browser signifies that the site uses a [[TLS (Transport Layer Security)]] certificate based on PKI
 - email security
 - [[VPN (Virtual private network)]]s
Examples:
 Accessing a website
  1. Your web client connects to a web server & gets the servers certificate and public key
  2. your web client verifies whether that site's certificate originates from a trusted source by looking in your browsers/computers certificate store
  3. The client encrypts a piece of data using the certificates public key and sends it to the server. If the server can read it, it proves that the server has the correct private key and it's connecting to the right server.
 Ecommerce
   whenever a transaction is processed online the customer uses the applications public key to encrypt their sensitive information which is then decrypted by the server using the private key to protect the customers details from being read in the event of an interception
Setting up secure connection
 CA gives public key, you send asymmetrically encrypted (using public key) key for symmetric communications & it is decrypted by receivers private key. Receiver now has symmetric key for communications to setup an encrypted tunnel (HTTPS connection) using SSL or TLS encryption.
 ![[Pasted image 20240117143145.png]]
 ![[Pasted image 20240117143537.png]]
Components of the PKI ecosystem
  1. A user applies for a certificate with their public key at an RA
  2. The RA confirms the user's identity to the CA, which issues the certificate
  3. The certificate is then ready for use and the user can digitally sign a contract using their new certificate
  4. The identity is checked by the contracting party with a VA which again receives information about issues certificates by the CA
![[Pasted image 20231127160404.png]]