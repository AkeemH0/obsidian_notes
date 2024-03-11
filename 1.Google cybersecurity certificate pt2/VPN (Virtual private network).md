**Definition:**
 A secure network connection that allows remote users to access a private network over the internet.

- A network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you are using a public network like the internet.
- VPNs also encrypt ([[Encryption]]) your data as it travels across the internet to preserve confidentiality using algorithms such as [[AES (Advanced Encryption Standard)]] or Triple Digital Encryption Standard (3DES) for client-based (provide secure access for individual users) & [[IPsec (Internet Protocol Security)VPN]] for site-to-site (provide secure access between entire networks (act as if they are part of the same LAN))
- Encapsulation is a process performed by a VPN service that protects data in transit by wrapping sensitive data in other data packets allowing your data to be sent across the public network while remaining anonymous
- A VPN uses an encrypted tunnel between your device and the VPN server, the encryption is unhackable without a [[cryptographic]] key
- [[VPN Concentrator]] 
- Organizations often use a combination of VPN & [[SD-WAN (Software-defined Wide area networks)]] 
Use:
When you connect to the internet your internet service provider receives your networks request and forwards it to the correct destination server. If the traffic gets intercepted someone could connect your internet activity with your physical location and your personal information. Using a VPN can prevent this from happening.

Remote access VPN:
Individual users use remote access VPNs to establish a connection between a personal device and a VPN server. The connection between the user and the remote access VPN is established through the internet.

Site-to-site VPN:
Enterprises use site-to-site VPNs largely to extend their network to other networks and locations. This is useful for organizations that have many offices across the globe. IPSec is commonly used in site-to-site VPNs to create an encrypted tunnel between the primary network and remote network. One disadvantage is how complex they are to configure and manage compared to remote VPNs.

VPN protocols:
WireGuard and IPSec are two different VPN protocols used to encrypt traffic over a secure network tunnel. Factors between choosing a protocol includes: connection speeds, compatibility with existing network infrastructure and business or individual needs.
[[WireGuard VPN]]
[[IPsec (Internet Protocol Security)VPN]]