A hypervisor abstracts the host's hardware from the operating software environment.
The software or firmware layer that manages and runs multiple [[VM (Virtual machine)]] on physical hardware (often referred to as a virtual machine monitor).
Enables the efficient and isolated execution of multiple virtual environments on the same hardware
- Help to allocate shared resources (RAM, Storage space & CPU availability )
2 types of hypervisors:
- Run on the hardware of the host computer e.g. VMware's EXSi. 
- Run on the software of the host computer e.g. VirtualBox


[[CSP (cloud service provider)]]s often use hypervisors that run on the hardware of the host computer
Vulnerabilities in hypervisors or misconfigurations can lead to virtual machine escapes ([[Virtual machine (VM) escape]]s).

- Multiple virtual servers can be created from a single physical server
- Virtual networks can also be created to more efficiently user the hardware of a physical network