
```
#if using a variable it will repeat through the whole list unless specified otherwise
for i in [1,2,3,4] 
print (i) # will print 1,2,3,4


for i in range (0,10) # inclusive first, exlusive second (so 0 to 9 inclusive)
# automatically start from 0 if we dont specify range (10)
# the variable i is created and only exists within the for loop
# its possible to loop through a string and return each character one by one e.g.
string = "security"
for character in string:
    print(character)
    #prints s e c u r i t y (each char on a diff line)  
```
![[Pasted image 20231226172624.png]]
