Application checks the value/data needed for a process
Another process causes the checked value/data to change in-between the time of check and time of use, unbeknownst to the applications current process
Application uses the value/data prior to the change for a process instead of the updated value
![[Pasted image 20240115211350.png]]
In this instance: Deposits instant, Withdrawals not instant
Since U1 & U2 deposits are instant there is no race condition (otherwise would be $150 instead of $200)
Since U1 & U2 withdrawals are not instant there is a race condition; although both users withdraw $50 from a $100 account the final balance is $50 instead of $0