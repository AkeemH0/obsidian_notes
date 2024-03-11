**Definition:** 
 An emulation of a computer system that operates in a software environment.

- Virtual instances of  that can run different [[OS (operating system)]]s or applications independently allowing for efficient resource utilization, isolation and flexibility.
- Additional layer of security as they run code in an isolated environment preventing malicious code from affecting the rest of the computer system. 
- VMs can also be deleted and replaced by a pristine image (clean and unaltered snapshot of a VM (back in its original untouched state)) after testing malware.
- Useful for investigating potentially infected machines or running malware in a constrained environment.
- There's still a small risk that a malicious program can escape [[virtualization]] and access the host machine
- May prevent damage to your system in the event its tools are used improperly. 
- VMs also give you the ability to revert to a previous state
- A VM inside of  VM is known as nested virtualization and is commonly used in testing to increase security in-case the malware escapes the initial VM.
- example of [[virtualization]]
- Increases efficiency as many security tasks can be performed simultaneously and switched between.
- [[hypervisor]] is software used to manage multiple Virtual machines and connect the virtual and physical hardware. 
- Some malware can tell if they're in a VM & may hide signs of malicious intent by disguising itself
- [[VM escape]]