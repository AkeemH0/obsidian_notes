The process of managing a key throughout its lifecycle (includes: secure environment, storage, distribution and usage)
Keys are often managed using an automated system (cryptographic key system management) that oversees & secures the key management process.
Strong cryptographic algorithms can be compromised by poor key management resulting in a complete loss of confidentiality as the encrypted data will be compromised
A common practice to maintain security is the frequent regeneration of keys 
keys should be kept up to date to avoid cryptographic vulnerabilities and use the latest cryptographic algorithms
Old keys should be deactivates and deleted to remove the risk of accidental compromises in the future
Secure key management methods:
 1. 
    Encrypt private keys themselves & store them in a password-protected folder. Any attempted breach could be identified and eliminated with the help of [[IDS (Intrusion detection system)]].
 2. 
    Store the private key in hardware where possible (such as [[HSM (hardware security module)]])
     a. The keys are physically protected because they are stored on a locked-down appliance in a secure location with tightly controlled access.
     b. The keys are logically secure as they are typically password-protected or encrypted





[[TPM (Trusted platform module)]]
[[Cloud hardware security module (Cloud HSM)]]
Organizations & customers don't have direct access to the CSP but they can request audits and security reports by contacting the CSP.
Customers don't have access to the specific encryption keys that the CSP use to encrypt data however most CPSs allow customers to provide their own encryption keys, however this makes the customer responsible for their encryption keys and ensuring the key remains confidential & the CSP is limited in how they can help the customer if their key is compromised or destroyed.
