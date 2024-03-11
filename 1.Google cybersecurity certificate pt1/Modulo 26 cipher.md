 An encryption algorithm that utilizes [[One-time pad]]
 Table 
    - assign each letter a numerical value e.g. (A=0 B=1 C=2 ... Z=25)
      ![[Pasted image 20231127143355.png]]
 Encryption
   - Text and key values are added together & if the value is more than 25 we subtract 26 until the value is <=25
   - Then we convert the result back into letters
 Decryption
  - subtract the one-time pad key value from the cipher text value
  - If the result is <0 then we add 26