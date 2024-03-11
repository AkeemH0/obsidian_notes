**Definition:** 
 A block cipher mode of operation that enhances security by XORing the previous block's ciphertext with the current block's plaintext before encryption.

Popular mode of operation (easy to implement)
 - Adds additional randomization
 - Uses a seed generated [[IV (initialization vector)]] for the first block
 - Subsequent plaintext blocks use the previous ciphertext block as the initialization vector (Each plaintext block is XORed with the previous ciphertext block)
- Encryption:
![[Pasted image 20231127082826.png]]


- Decryption:
  ![[Pasted image 20231127082821.png]]