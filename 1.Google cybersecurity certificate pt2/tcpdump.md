- A [[Command Line Interface (CLI)]] line network protocol analyser. 
- [[Lightweight ]]
- Uses open-source libpcap library meaning users can access the source code & make adjustments/configurations
- tcpdump is used to capture network traffic which can then be saved to a [[PCAP (Packet capture)]] (libpcap in this case)
- text based- all commands are executed in the terminal
- Can be installed on Unix-based OS such as macOS
- Preinstalled on many Linux distributions
- provides brief packet analysis and converts key information about network traffic into formats easily read by humans.
- Prints information about each packet directly into your terminal
- Displays time, source IP, Destination IP, source port & destination port numbers being used in the communications
- ![[Pasted image 20230919105402.png]]
- Can output sniffed packets to a log file after a command is executed in order to review packets later
- Timestamp: Hours, minutes, seconds, fractions of a second
- Source IP: 
- Source port: 
- Destination IP: 
- Destination Port:
Notes: 
- tcpdump attempts to resolve host addresses to hostnames
- tcpdump replaces port numbers with commonly associated services that use these ports  
  
Uses:
-  Troubleshooting network performance
- Establish a baseline for network traffic patterns and network utilization metrics
- Detect and identify malicious traffic
- Create customized alerts to send the right notifications when network issues or security threats arise
- Locate unauthorized instant messaging (IM), traffic or [[WAP (wireless access point)]]s
- Attackers can maliciously gain information about a network such as SPII & PII like account names and passwords
- Source IP address is always left of >
- Destination IP address is always right of >

Flags \[S] - Connection Start
Flags \[F] - Connection Finish
Flags \[P] - Data Push
Flags \[R] - Connection Reset
Flags \[.] - Acknowledgment e.g. Flags\[S.] = SYN-ACK packet
HTTP: GET / HTTP/1.1 is a get request


HTTP: GET / HTTP/1.1 shows the browser is sending a get request for yummyrecipesforme.com data which could be the download request for the malicious file


![[Screenshot 2023-11-18 071122.png]]
`sudo tcpdump [-i interface] [option(s)] [expression(s)]
- The option(s) provide you with the ability to alter the execution of the command 
  [[option(s) (tcpdump)]]
- The expression(s) are a way to further filter network traffic packets so that you can isolate network traffic
 [[expression(s) (tcpdump)]]
- you must identify which network interface you'll capture packets from  (using -D flag lists the network interfaces available on a system) unless you use `any`.
1. [[sudo]] [[tcpdump]] -i any -v -c 1
   sudo is used to elevate privileges so that tcpdump can be run
   -i ___ specifies which network interface we want sniff traffic on
   -i any sniffs traffic from all network interfaces on the system
   -v stands for verbose which displays detailed packet information
   -c stands for count which specifies how many [[packet]]s tcpdump will capture

2. tcpdump: listening on any, __ ,capture size 262144 bytes
   Indicates Tcpdump is listening on any available network interfaces & gives additional information such as capture size
   
3. 20:00:29.538395 
   Packet timestamp (indicates the time of beginning of travel). Helpful during incident investigation to determine timelines and correlate traffic.
   
4. [[IP (Internet protocol)]] 
   indicates the version field. Since its listed as IP it is IPv4 as that is the default internet protocol.
   
5. [[Type of Service (ToS)]] 0x10
   indicates if different packets should be treated with different care which is represented by a value in hexadecimal
   
6. [[Time to Live (TTL)]] 64
   indicates how long a packet can travel across a network before it gets dropped
   64 indicates the packet can traverse through 64 routers or networks before it is discarded
   
7. id 32645, offset 0, flags \[DF] 
   provided information relating to fragmentation
   contain instructions on how to reassemble packets in the correct order
   flags \[DF] stands for Don't Fragment
   
8. proto TCP (6)
   specifies the protocol in use along with the value that corresponds to the protocol

9. length 196
   Total Length of the packet including the IP header (196 bytes in this case (1568 bits))

10. 198.122.123.1.41012 > 198.111.123.1.61012
   The extension of the IP address indicates the port number or name  (41012 (source port in this case) & 61012 (destination port in this case))
   The direction of the arrow indicates the direction of the packet flow 

11. Flags [P.] 
   indicate TCP flags (The P is the data push flag and the period indicates it's an ACK flag)

12. cksum 0xa83f (correct)
 Corresponds to the [[Header Checksum]], which stores a value used to determine if any errors have occured in the header

`X` Displays the hexadecimal and [[ASCII]] output format packet data. Security analysts can analyse hexadecimal and ASCII output to detect patterns or anomalies during malware analysis or forensic analysis.