[[On-path attack]] on the local IP subnet
[[ARP (address resolution protocol)]] has no security/encryption
involves spoofing IP address to pretend to be another device

In this instance the attacker uses ARP poisoning to conduct a MITM attack by changing the ARP cache of a device to make it so that the attacker is set as the default gateway so the victim device sends requests to the attacker device which it then forwards to the default gateway acting as a proxy.

Pretends to be default gateway (to sender) & sender (to default gateway)
pretends to be 192.168.1.9 to 192.168.1.1
pretends to be 192.168.1.1 to 192.168.1.9
![[Pasted image 20240118133155.png]]
  