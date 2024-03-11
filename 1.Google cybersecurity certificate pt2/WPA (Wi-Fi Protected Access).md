**Definition:** 
 A security protocol designed to secure wireless computer networks.

A wireless security protocol for devices to connect to the internet.
- WPA addressed [[WEP (Wired Equivalent Privacy)]]s weak encryption by using [[TKIP (Temporal Key Integrity Protocol)]] which uses larger secret keys than WEPs making it more difficult to guess the key by trial and error
- Includes a message integrity check that includes a message authentication tag with each transmission so that if a malicious actor attempts to alter the transmission or resend at another time, WPA's message integrity check will identify the attack and reject the transmission
- Malicious actors can use a  [[KRACK attack]]to decrypt transmissions using WPA. Attackers can insert themselves in the WPA authentication handshake process and insert a new encryption key instead of the dynamic one assigned by WPA. If they set the new key to all zeros, it is as if the transmission is not encrypted at all, therefore WPA was replaced with WPA2
- Evolved into [[WPA2]] & [[WPA3]] which include further security improvements like more advanced encryption