**Definition:** 
 A file format used to store network packet data captured during network traffic analysis.

A file containing data packets intercepted from an interface or network.
Files can come in many formats depending on the packet capture library that's used:
- Libpcap - packet capture library designed to be used by Unix-like systems (Linux and MacOS). Tools like tcpdump use Libpcap as the default packet capture file format.
- WinPcap - an open-source packet capture library designed for devices running Windows OS. It's considered an older file format and isn't predominantly used.
- Npcap - is a packet capture library designed by the port scanning tool Nmap that is commonly used in Windows OS.
- PCAPng - is a modern file format that can simultaneously capture packets and store data. Its ability to do both explains the "ng" which stands for "next generation".
