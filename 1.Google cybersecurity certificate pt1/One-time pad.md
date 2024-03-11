- An unbreakable [[cipher]] where the key length is equivalent to the encrypted message length
- The key (pad) is made up of random symbols and  i only used once and never again for any other message to be encrypted.
- Each bit or character from the plaintext is combined by modular addition with a bit or character from a secret random key (pad) of equal length, resulting in ciphertext.
One-time pad encryption methods
 - [[Vigenère cipher]]
 - [[Modulo 26 cipher]]
Rules for unbreakable one-time pad encryption
 - The key should consist of truly random symbols
 - Only two copies of the one-time pad should exist (one for the sender and one for the receiver)
 - The one-time pad should only be used once
 - Both copies of the one-time pad are destroyed immediately after use
Use
 - Situations where possession of a computer is illegal or incriminating or where trustworthy computers are not available
Difficulties
 - Transferring one-time pad whilst keeping it secret (are usually transferred in paper form)