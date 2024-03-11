filter expressions
Can be used to specifically search for network traffic by protocol e.g. you can filter to find only IPv6 traffic using the filter expression ip6
You can utilize boolean operators like `and`, `or` & `not`.
E.G. `sudo tcpdump -r packetcapture.pcap -n 'ip and port 80'`
tcpdump reads the packetcapture.pcap with automatic name resolution disabled & filter expressions to display packets with IPv4 using [[port ]]80
Notes: 
- you can use single or double quotes to ensure that tcpdump executes all of the expressions.
- you can use parentheses to group and prioritize different expressions, which is helpful for complex or lengthy commands e.g. `ip and (port 80 or port 443)`
