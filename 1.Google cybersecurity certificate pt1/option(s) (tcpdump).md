also known as flags
Used to filter network traffic
Short options are abbreviated and represented by a single hyphen (-i)
Long options are spelled out & use a double hyphen (--interface)
Options are case sensitive
Short options can be written without a space between the option and its value e.g.
`sudo tcpdump -i any -c 3`   ==    `sudo tcpdump -iany -c3`

Options/Flags:
`-w` : write/save the sniffed network packets to a packet capture file instead of just printing it out in the terminal. Useful for later packet analysis e.g. for [[Digital Forensics]].
Example: `sudo tcpdump -i any -w packetcapture.pcap`
tcpdump is capturing network traffic from all network interfaces and writing it to a [[PCAP (Packet capture)]] file

`-r `: read a packet capture file by specifying the file name as a parameter.
Example: `sudo tcpdump -r packetcapture.pcap`
tcpdump will read the network traffic data stored in the P-cap file

`-v`: (verbose (meaning excessively wordy)), lets you control how much packet information you want tcpdump to print out. There are 3 levels of verbosity 
(`-v ` `-vv` `-vvv`) which increases with each v added. Useful if you're looking for packet information like details of a packet's IP header fields.
Example: `sudo tcpdump -r packetcapture.pcap -v`

`-c`: stand for count. Lets you control how many packets tcpdump will capture.
Example: `sudo tcpdump -i any -c 3` 
tcpdump will capture the first 3 packets it sniffs from any network interface

`-n`: Disables automatic name resolution (considered to be best practice when [[packet sniffing]]) `-n` will not resolve hostnames whereas `-nn` will not resolve both [[hostname]]s or[[ port]]s
By default tcpdump will automatically perform [[name resolution]].
Additionally, name resolution uses a [[reverse DNS lookup]]
Example: sudo tcpdump -r packetcapture.pcap -v -n
tcpdump reads the packetcapture.pcap file with verbosity and disables name resolution

**Note: you can combine options that don't accept parameters right after each other 
e.g. `-v` & `-n` can be combined to -`vn`**

`&`: This is an instruction to the Bash shell to run the command in the background.

