- Improvement of [[WPA (Wi-Fi Protected Access)]] by:
- using the [[AES (Advanced Encryption Standard)]]. 
- using [[TKIP (Temporal Key Integrity Protocol)]]
- using the [[CCMP (Counter Mode Cipher Block Chain Message Authentication Code Protocol)]], which provides encapsulation and ensures message authentication and integrity.
- Still vulnerable to [[KRACK attack]]s thus [[WPA3]] was created
- The [[PSK (Pre-shared Key)]] hash can be captured during the handshake and [[brute force attack]]ed to find the original password & connect to the network.
- WPA2 Personal version is easy to implement, Initial setup takes less time for personal version than enterprise version since global passphrase for WPA2 personal version needs to be applied to each individual computer and access point in a network, making it ideal for home networks but unmanageable for organizations
- WPA2 Enterprise version works best for business applications as it provides the necessary security for wireless networks in business settings. Initial setup is more complicated than WPA2 personal mode, but enterprise mode offers individualized and centralized control over the [[Wi-Fi (Wireless Fidelity)]] access to a business network. This means that network administrators can grant or remove user access to a network at any time. Users never have access to encryption keys, this prevents potential attackers from recovering network keys on individual computers.