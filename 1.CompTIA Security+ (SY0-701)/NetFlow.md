A standard for monitoring traffic flows & traffic statistics (all shared communication between devices)
- Has a NetFlow probe to compile data. 
- Probe watches network communication and sends summary to the collector. 
- May be built into the software of a networking device or connected as an external hardware device. 
- Connect probe via monitoring port (e.g. [[SPAN (Switch Port Analyser)]]) or a physical [[tap]].
- Copy of compiled metrics is sent to NetFlow collector
- NetFlow collector uses metrics/data to create reports & details
![[Pasted image 20240212112347.png|logical network topology including probe and collector|400]]
![[Pasted image 20240212112509.png|NetFlow collector summary (NetFlow Traffic Analyzer)|800]]