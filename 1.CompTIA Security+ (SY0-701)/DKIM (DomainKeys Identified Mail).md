**Definition:** 
 A method to validate the authenticity of email messages by attaching a digital signature in the message's headers.
 - Stored in DNS TXT record
- The sending email server digitally signs (DKIM signature) all outbound email headers using the domains private key
- Receiving email servers verify the DKIM signature using public key from the sending domains [[DKIM TXT record]]