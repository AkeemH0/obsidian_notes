Detailed Summary
 - Verifies the authenticity and integrity of data by associating it with a unique digital signature generated using the sender's private key.
 - The mathematical algorithm creates data matching the signed document called a hash & encrypts that data with the result being the digital signature.
 - The hash generated is unique to the document & changing any part of the document will completely change the hash
 - The recipient generates their hash of the document and decrypts the signer's digital signature using the signer's public key (which can be found and verified in a [[key repository]]) to retrieve the original hash.
 - If the recipients hash matches the decrypted signatures hash the document has not been modified and the sender is authenticated otherwise the document has been changed after signing and the digital signature is invalid

Process:
  Signer:
   1. creates a [[hash]] of the data they wish to send
   2. encrypts hash using their private key (digital signature)
   3. sends the original data (doesn't need to be encrypted) along with the digital signature
  Recipient: 
   1. receives the original data and the digital signature
   2. generates a hash of the original data
   3. decrypts the digital signature using the signer's public key to retrieve the hash the signer originally generated.
   4. compares the original hash to the one they have generated. If the hashes match the document hasn't been modified and the sender is authenticated.
Digital signatures provide the following assurances:
 - [[authenticity]] : the proclaimed signer is confirmed as the real signer
 - [[Integrity]] : The content has not been altered since signing
 - [[Non-repudiation]] : Proves the origin of the singed document to all parties
Uses:
 - Financial transactions
 - Contract management software
 - Email service providers
 - Cases where it is important to detect tampering
Other
 "electronic fingerprint"
 used to associate a signer with a document to provide proof of ID & to verify a file hasn't been modified since signing
 uses [[PKI (public key infrastructure)]] to provide the highest level of security and universal acceptance.
![[Pasted image 20231127085810.png]]

[[DSA (Digital signature algorithm)]]
[[RSA (Rivest, Shamir, & Adleman)]]
[[ECC (Elliptic Curve Cryptography)]]