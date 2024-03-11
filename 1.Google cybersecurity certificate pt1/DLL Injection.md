[[DLL (Dynamic Link Library)]] Injection
Inserting an external DLL file containing malicious code into the address space of a running DLL OR injecting malicious code into existing DLLs 
A rootkit either:
- Inject Malicious code into a runtime processes existing DLLs
- Replace the address space of an existing DLL for a runtime process with an external malicious DLL; done by changing [[shim]] code so that it intercepts communications between the windows OS and an existing [[DLL (Dynamic Link Library)]] and redirects to an external malicious DLL. 
so that the rootkit starts up each time you boot
![[Pasted image 20240115205641.png]]
