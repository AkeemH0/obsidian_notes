a method to detect if a packet has been corrupted/modified in transit
comparing the senders checksum with the receivers calculated checksum
If senderChecksum!=receiverChecksum then packet has been altered or corrupted 
- Faster to compute than hashes 
- Higher likelihood of collisions than hashes
- Checksums are used for error-checking while hashes are used for integrity checking