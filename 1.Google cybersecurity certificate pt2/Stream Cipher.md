Also known as [[bulk cipher]]
A method of [[symmetric encryption]] that encrypts data bit by bit using an [[XOR (Exclusive Or)]] function to create ciphertext, rather than waiting for a data block to form ([[block cipher]])
Applies an encryption algorithm to a [[pseudorandom]] [[cipher]] digit stream (keystream) using an XOR operation.
Each bit is encrypted one by one with the corresponding keystream digit to give a digit of the [[ciphertext]] stream.

Synchronous stream cipher : The keystream is generated independently of any previous plaintext or ciphertext. The sender and receiver must be synchronized in terms of key generation.

Asynchronous stream cipher :The keystream is generated from the previous ciphertext bits. The sender and receiver mustn't be perfectly synchronized in terms of key generation.

Key recycling: reusing portions of the keystream (introduces complexity and potential vulnerabilities so careful design and analysis are crucial)

[[PRNG (pseudorandom number generator)]]

- High speed
- Low processing power required
- Not commonly used with asymmetric encryption due to the overhead additional time it takes to be able to encrypt and decrypt with asymmetric encryption
- The key is often combined with an [[IV (initialization vector)]] to add some randomization to the encryption process (as you don't know what's coming later in the stream until you get to that particular byte meaning randomization of the data can be challenging if multiple bytes are input into the stream that are identical as you'd end up with identical bytes on the encrypted side (XOR  operation))
- If there's an error in one symbol it'll be less likely to affect the next due to the bit by bit approach.

![[Pasted image 20231127172918.png]]
Use:
 Utilized in applications where high speed is needed & data comes in quantities of unknowable length (real-time communication data streams: streaming audio, streaming video, gaming)
 - Secure wireless communication
 - Bluetooth & 4G [[Wi-Fi (Wireless Fidelity)]]
Vulnerabilities:
 - [[bit-flipping]]
 - [[key reuse attack]]