Combine [[Adaptive identity]] with a predefined set of policies to determine authorization

- [[Policy administrator]]
- [[Policy Decision Point(PDP)]] 
- [[Policy engine]]
- [[Policy Enforcement Point (PEP)]]

![[Pasted image 20240102152101.png]]

**PEP intercepts access requests** & **asks PDP** whether to allow/disallow
If **PDP** needs additional info it will **communicate** with the **policy administrator**
Policy administrator provides necessary **information** on **access control policies**
**Policy engine processes information** & **makes decision** on whether traffic is allowed
Result is **passed down to policy administrator** 
Policy administrator **provides results to PEP**
PEP **allows/disallows access**



[[Access control]]