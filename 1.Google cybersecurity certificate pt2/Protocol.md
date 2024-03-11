A set of rules used by several devices on a network to determine the order of the delivery and the structure of the data.
Instructions in the data [[packet]] header that tell the receiving device what to do with the data.
- Protocols are like common language that allows all devices to communicate and understand each other
- Some protocols have [[vulnerabilities]] that can be exploited e.g. Use [[DNS (Domain Name System)]] to divert traffic to a malicious website.
- Three Types of protocols:
  - Communication protocols: 
    Govern exchange of information ;dictate how data is transmitted between devices & the timing of the communication. Also have methods to recover data lost in transit.
     - [[Transmission control protocol (TCP)]]
     - [[UDP (User Datagram Protocol)]]
     - [[HTTP (Hypertext Transfer Protocol)]]
     - [[DNS (Domain Name System)]]
     - [[Telnet]]
  - Management protocols:
    Monitor & manage network activity. Involve error reporting & performance optimization.
     - [[SNMP (Simple Network Management Protocol)]]
     - [[ICMP (Internet Control Message protocol)]]
     - [[DHCP (Dynamic Host Configuration Protocol)]]
     - [[POP3 (Post Office Protocol version 3)]]
  - Security protocols:
    Ensure secure sending & retrieval of data by utilising encryption algorithms to protect data in transit. Don't conceal the source or destination IP address thus interceptors can still learn basic information about traffic.
     - [[HTTPS (Hypertext Transfer Protocol Secure)]]
     - [[SFTP (SSH File Transfer Protocol)]]
     - [[FTPS (File Transfer Protocol Secure)]]
     - [[SMTPS (Simple Mail Transfer Protocol Secure)]]
     - [[SSH (Secure Shell)]]