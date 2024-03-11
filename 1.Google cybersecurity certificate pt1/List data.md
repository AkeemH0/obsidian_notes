A data structure that consists of a collection of data that can be changed in sequential form
Can contain multiple data types
mutable
Uses square brackets [ ]

```
#prints the first 2 elements of the list
username_list = ["elarson", "fgarcia", "tshah", "sgilmore"]
print(username_list[0:2]) 

#prints the element at index 2 from the list
print(["elarson", "fgarcia", "tshah", "sgilmore"][2])

#prints the element at index 2 from the list
username_list = ["elarson", "fgarcia", "tshah", "sgilmore"]
print(username_list[2])

#changes the element at index 1 of the list
username_list[1] = "bmoreno"

#removes the element "elarson" from the list
username_list.remove("elarson")

#adds the element "wjaffrey" to index 2 of the list (shifts the rest of the list up 1 index)
username_list.insert(2,"wjaffrey")

#adds the element to the end of the list
username_list.append("btang")

#add numbers iteratively to a list & print the output
numbers_list = []
for i in range(10):
    numbers_list.append(i)
print("After appending a sequence of numbers:", numbers_list)

# used to find the index of the element "tshah" in the list
username_index = username_list.index("tshah")
```