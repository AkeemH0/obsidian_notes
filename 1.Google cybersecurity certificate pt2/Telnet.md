An older remote access protocol that allows access (with/without login)and control (using [[CMD]]) a remote server/device over a network similar to [[SSH (Secure Shell)]]  however, Telnet's less secure because it doesn't provide encryption (sends all information in clear text).
Mostly used for device management purposes
Telnet client isn't installed on windows by default so it must be installed and activated in order to make connections via telnet protocol
Port 23 TCP [[7.Application Layer OSI]]
- No authentication policies (no default enforcement of username and password, local admins can configure local authentication for Telnet)
- No encryption
**CMD line:** 
 - `telnet` (Ip address) e.g. `telnet 192.168.5.100`
**Images**:
 ![[Pasted image 20240219075618.png|enabling telnet client]]
 ![[Pasted image 20240219075606.png|enabling telnet client]]