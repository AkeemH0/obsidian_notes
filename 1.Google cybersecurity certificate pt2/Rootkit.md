[[malware]] that provides persistent remote, [[administrative (root) access]] to a computer without being detected. Rootkits try to increase privilege level.
Wont be seen in task manager

Rootkits try to elevate privileges by moving themselves from [[privilege level]] 3 (user) to privilege level 0 (kernel) so that it can hide from your OS & antivirus to avoid detection.
This can be done throughout [[DLL Injection]]

can be spread by a [[dropper]] and a [[loader]]

Attackers use rootkits to open a backdoor to systems allowing them to install other forms of malware or to conduct network security attacks ((e.g. by opening vulnerable ports)).

Countermeasures:
- External system scan to find rootkit
- Secure boot with [[UEFI (Unified Extensible Firmware Interface)]]

