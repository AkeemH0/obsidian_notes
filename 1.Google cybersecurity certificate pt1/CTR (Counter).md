Uses an incremental counter to add randomization to the encryption process
Block cipher mode / acts like a stream cipher
 - Encrypts successive values of a counter
Plaintext can be any size, since it's part of the XOR
 - i.e. 8 bits at a time (streaming) instead of a 128-bit block (streaming refers to the data being processed in a continuous manner where the data isn't divided into fixed-size blocks but is instead operated on as a continuous flow).
![[Pasted image 20231123165352.png]]