**Definition:** 
 A secure file transfer protocol that provides encrypted communication over a network using SSH.
Port 22 TCP [[7.Application Layer OSI]]
A secure network protocol used for securely transferring files and managing file systems over a network. It is an extension of [[SSH (Secure Shell)]] which provides authentication and encrypted communication between clients and servers. SFTP is designed to ensure the confidentiality and integrity of data during file transfers. Occurs at the [[4.Application Layer (TCP,IP)]]. Often used with Cloud storage
- Often used as a secure alternative to traditional [[FTP (File Transfer Protocol)]] because it encrypts both authentication and data transfer making it resistant to [[eavesdropping]] and tampering.
- it operates on top of the SSH protocol and typically uses port 22 for communication
- SFTP provides strong authentication methods including username and password as well as key-based authentication using SSH key pairs
- Data transferred over SFTP is encrypted, ensuring that files and data remain confidential during transit
- Unlike [[FTPS (File Transfer Protocol Secure)]], SFTP uses a single port (usually port 22), simplifying firewall configuration.
- SFTP is commonly used for securely transferring files between a client and a remote server. It's frequently employed for tasks such as uploading and downloading files, remote backups and securely managing web server files
- SFTP clients and servers are available for various operating systems making it a widely supported and accessible protocol for secure file transfers
