- The practice of capturing analysing data packets across a network .
- Carried out by a [[packet sniffer]]
- Can be used to collect network statistics such as bandwidth or speed and troubleshoot network performance issues, like slowdowns.
- A malicious actor may place themselves between a connection between two devices [[MITM (man-in-the-middle) attack]] in order to packet sniff using a [[packet sniffer]] or hardware device to gain valuable information from the body of the packet such as SPII or PII
- malicious actors can make changes to the data such as altering the recipient of a transaction or inserting malicious code such as [[Spyware]]
Passive packet sniffing: 
- Packets are read in transit by the host
- *Like a postman reading letters he is delivering, he has the right to deliver the letters but not the right to read them*
Active packet sniffing:
- data packets are manipulated in transit
- e.g. injecting internet protocols to redirect the packets to an unintended port or changing the information the packet contains
- *Like a neighbour telling a postman they'll deliver the mail for them & then reading the mail or changing the letter before delivering it*

preventing packet sniffing:
- Using a [[VPN (Virtual private network)]] to encapsulate & encrypt data as is travels across a network
- Only accessing websites that utilise [[HTTPS (Hypertext Transfer Protocol Secure)]]
- Avoid using unprotected [[Wi-Fi (Wireless Fidelity)]] or low protection Wi-Fi such as [[WEP (Wired Equivalent Privacy)]], however if you have a VPN service already installed on the device avoids this security flaw