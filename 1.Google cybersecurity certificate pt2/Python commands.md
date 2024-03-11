ctrl + z or ctrl + c to break an infinite loop
`//` (return a whole number from a calculation) e.g. print(1//4) = 0
`type ()` : Returns the data type of its input
`if` : Starts a conditional statement (If statements contain a header & body)
`elif` :precedes a condition that is only evaluated when previous conditions evaluate to false
`else` :precedes a code section that is only evaluated when all previous conditions evaluate to false 
`and` requires both conditions to evaluate to true
`or` requires either conditions  to evaluate to true
`not` opposes the conditions output, True<->false  1<->0
`in` checks to see whether a value is in a list e.g. `if username in user_list:`
`for` used to repeatedly execute a section of code a set number of times ([[for]]) (fixed loop),
`while` used to repeatedly execute  a section of code while a condition is met ([[while]]) (conditional loop)
`range( __ ,__ ,__ )`  start point inclusive, end point exclusive, increment ([[range]])
`break` exits a for or while loop if a condition is met ([[break]])
`continue` skips to the next iteration in the loop ([[continue]])
`def` Placed before a function name to define a function e.g. `def my_function():` ([[def]])
`return` Used to return information from a function
`print()` outputs a specified object to the screen
`type()` returns the data type of its input
`max()` Returns the largest numeric input passed into it
`min()` Returns the smallest numeric input passed into it
`sorted()` Sorts the components of a list
`import` searches for a module or library in a system and adds it to the local Python environment.
`from ____ import ___,___,___` to import specific function from a library ([[import]])
 
`str()` converts the input object into a string object
`len()` returns the number of elements in an object
`.upper` A string method that returns a copy of the string in all uppercase letters e.g. `print("Hello".upper())`
`.lower` A string method that returns a copy of the string in all lowercase letters e.g. ``print(name.lower())``
`.index()` Finds the first occurrence of the input in a string and returns its location

[[regular expression (regex)]]

`.insert(index,data)` Adds an element in a specific position inside a list without deleting other elements (shifts them)
`.remove()` Removes the first occurrence of a specific element in a list e.g. `my_list.remove("d")`
`.append()` adds input to the end of a list

`with` Handles errors and manages external resources (automatically release resources that would otherwise keep our system busy until the program finishes running (e.g. by closing file (if you don't use with you will have to close file (`close()`)))
`open()` Opens a file in python
`.read()` Converts files into strings
`.write()` adds text into a file (doesn't update unless the file is closed after writing)
`.split()` Converts a string into a list # separates a string based on a specified character or if no argument is passed, every time it encounters a whitespace
`.join()` converts a list into a string `characters_to_separate_each_element.join(listname)` e.g. `",".join(list) #can also use \n (newline character) to saperate each element by a newline

Examples
`print("Hello"[1]) #returns e`

`print("Hello"[1:4]) #returns ell (first num inclusive, second num exclusive)`

`my_list[1] = 7 #replaces the element at index 1 in my_list with 7`

`with open( "filepath"/"filename"(if in same directory as python file), "r"/"w"/"a") as variablename: #e.g. variable name can be ip_list_file, after the colon write the instructions on what to do with the file, r=read,w=write,a=append

`with open("newfile.txt", "w") as newfile: #"w" used to create a new file `

Tips
Files no longer in use should be closed ASAP to maintain code readability