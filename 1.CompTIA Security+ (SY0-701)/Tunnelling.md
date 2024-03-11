A technique used in [[VPN (Virtual private network)]]s & networking to encapsulate/wrap data in a secure encrypted "tunnel" for private transmission across a public network.
The IP Header & data are encrypted & IPsec Headers/Trailers are added to show where the original packer starts and ends, then a new IP header is added to the packet which is used as a mask for the original IP.
The [[VPN Concentrator]] does the encrypting/decrypting
*Like hiding a transparent envelope in a non-transparent envelope with a different source address. The envelope is packed by the user when requesting data and unpacked by the user when receiving data.*
![[Pasted image 20240203193555.png]]