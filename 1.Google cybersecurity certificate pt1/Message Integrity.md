Assures that the transported message hasn't been altered.
A message has integrity when the payload sent is the same as the payload received
[[Encryption]] doesn't guarantee integrity as alterations can still take place

Passive message integrity threat:
 - Occur due to noise in communication channel or data corruption 
Active message integrity threat:
 - When an attacker manipulates the message maliciously
 - Protected against by security mechanisms such as hash functions
   

[[digital signature]] preserves integrity

message and digest pair ("electronic fingerprint") preserves integrity.
 - A message is passed through an algorithm called a cryptographic hash function to preserve integrity.
 - The hash function creates a compressed message value that can be used as an electronic fingerprint
 - ![[Pasted image 20231127134852.png]]
 - The message and message digest are mathematically linked
 - The message and message digest can be unlinked separately but the message digest must be kept safe from change
 - The message digest is created at the sender site and is sent with the message to the receiver
 - To check the integrity of a message or document the receiver creates the hash function again and compares the new message digest with the original message
 - If both are the same, the receiver is sure that the original message has not been changed
 - ![[Pasted image 20231127135209.png]]


Message integrity is important as it ensures the message digest hasn't been altered during transit. Recipients cross-reference the hashes (original digest & received message) to check that they are identical