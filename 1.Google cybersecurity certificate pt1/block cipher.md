- Encrypt fixed-lengths groups of [[bit]]s (plaintext bits -> ciphertext bits)
- Often 64-bit or 128-bit blocks
- Pad added to short blocks (to reach 64 or 128 bits)
- Padding shouldn't be added to the same section each time (vary between end/start of each plain-text block), or the security of the block cipher reduces since it becomes predictable
- Each block is encrypted or decrypted independently
- used in [[symmetric encryption]] algorithms (to encrypt as quickly as possible with a minimum of overhead)
- Some modes utilize [[IV (initialization vector)]]
- Easier to setup and implement and less susceptible to security problems than [[Stream Cipher]]
- Modes of operation (different ways to encrypt a block of information):
  Avoid patterns in the encryption
  Many different modes to choose from
  Different modes use different methods of encryption
  - [[ECB (Electronic code book)]]
  - [[CBC (Cipher Block Chaining)]]
  - [[CTR (Counter)]]
  - [[GCM (Galois Counter mode)]]

Triple Digital Encryption Standard (3DES) & [[AES (Advanced Encryption Standard)]] use block ciphers

  ![[Pasted image 20231127080937.png]]
  ![[Pasted image 20231127081208.png]]