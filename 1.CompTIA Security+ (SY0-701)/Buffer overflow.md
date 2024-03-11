Overwriting a [[buffer]] of memory so that it spills into other memory areas

- Time-expensive to exploit Application may crash often
- Its Complex to spill data into an area of memory with just the right information in order for the application to perform an advantageous function for the attacker
- A useful buffer overflow is repeatable
Countermeasures:
- Developers need to perform bounds checking to prevent excess data from being input
![[Pasted image 20240115210239.png]]![[Pasted image 20240115210248.png]]
Attacker input 9 characters for variable A, to overflow the last character into variable B thus changing it

[[Tail drop]]