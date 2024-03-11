a technique used to control network access by allowing or denying devices based on their MAC address
- MAC address filtering Operates at the Data Link Layer (Layer 2) of the [[Open Systems Interconnection (OSI)]] model
- To implement MAC address filtering the network administrator creates a list of MAC addresses for devices that are allowed to connect to the network. This list is often referred to as an allow list or [[whitelist]]
- When a device attempts to connect to the network, the network's access control system checks the device's MAC address against the list. If the MAC address is on the list, the device is granted access; otherwise, it is denied
- MAC address filtering can be used in conjunction with other security measures such as WPA/WPA2/WPA3 encryption for Wi-Fi networks, to add an extra layer of security
- While MAC address filtering provides a basic level of security, it is not fool proof because MAC addresses can be [[spoofed]] or cloned which is an important security consideration to understand
- Administrators should regularly review and update the MAC address list to maintain network security and ensure that only authorized devices are allowed to connect.