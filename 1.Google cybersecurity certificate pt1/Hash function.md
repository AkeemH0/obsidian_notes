- A mathematically irreversible algorithm that produces un-decryptable cipher known as a hash value
- hash functions are crucial for [[Non-repudiation]] & authentication
-  A good hash function should have a low chance of collision, be quick to compute and produce an output smaller than the input for improved search speeds
![[Pasted image 20231013144054.png]]


![[Pasted image 20231013143553.png]]
can be used to verify if a programs code has been altered

Virus Total is a common security tool that uses a database containing known online viruses, it hashes the input file and compares it to the database


[[hash table]] :A data structure used to store and reference hash values
![[Pasted image 20231013144920.png]]
[[MD5 (Message Digest 5)]]: 
A hashing algorithm that converts data into a 128-bit value which is represented as a string of 32 characters in a hash table
prone to collisions as it was only 128-bits 

generally, the longer the hash value the less prone to hash collisions it is
[[hash collision]]

[[SHA (Secure Hashing Algorithm)]]

Hashing is used for secure password storage:
- passwords are typically stored in a data base where they are mapped to a username
- This system is insecure in the scenario that an attacker gains access to the user database & the passwords are stored in plaintext
- Therefore passwords are hashed and stored as their hashed values 
- When logging in the users inputted password is hashed and checked against the hash value (of the accounts password) in the database

[[rainbow table]]

[[Salting]]


