- sensitive network traffic should be encrypted
**Protocol selection:**
- unencrypted protocols: [[Telnet]], [[FTP (File Transfer Protocol)]], [[SMTP (Simple Mail Transfer Protocol)]], [[IMAP (Internet Message Access protocol)]] may be used for non-sensitive matters that require little overhead
- ![[Pasted image 20240213131255.png]]
**Port selection:**
- Port number doesn't guarantee security as multiple protocols can run on the same port & security features may not be enabled (manually verify that security features are enabled using [[packet sniffing]])
**Transport method:**
- Instead of relying on application for encryption, encrypt the transport method instead
- Configuring network devices to use secure transport methods e.g. [[WAP (wireless access point)]] to only use [[WPA3]]
- Using a [[VPN (Virtual private network)]] as an [[agent]] or through a [[VPN Concentrator]]

