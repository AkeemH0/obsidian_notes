**Definition:** 
 A method of key agreement in cryptography, ensuring that both parties contribute to the generation of a shared secret.

Mutual authentication
Shares session key hashes aren't shared across the network (are created on the end devices instead)
No more four-way handshakes, no hashes, no brute force attacks ([[WPA2]]s weakness)

A Diffie Hellman derived key exchange with an authentication component
Everyone uses a different session key, so even with the same PSK you won't be able to see any of the traffic from other users on the network
An IEEE standard - (often called the dragonfly handshake)