A sequence of characters that forms a pattern 
e.g. all strings that start with a certain prefix or of a certain length (IP addresses, emails, device IDs)
requires the re module to be imported into python

`+` Represents one or more occurrences of a specific character e.g. a+ could be: "a","aa","aaa" etc.
`\w` Matches with any alphanumeric character but it doesn't match symbols e.g. "1","k" & "i"
`\w+` combines both of the above e.g. "192", "abc123", "security"
`.` all characters including symbols
`\d` all single digits
`\s` all single spaces
`\(symbol)` indicates that we are intending to use a symbol in the regex
`bw\a+b` e.g. bkaaab
`\w+@\w+\.\w+` regex for email addresses
`*` represents zero, one or more occurrences of a specific character
`re.findall((regex pattern),(string to search through))` Returns a list of matches to a regular expression
`{_}` indicates a specific number of repetitions to allow e.g. `re.findall("\d{2}","h32r317")#32,31`
`{_,_}` indicates a range of number of repetitions to allow e.g. `re.findall(\d{2,4},"h32r317)`


examples:
![[Pasted image 20231228174156.png]]

![[Pasted image 20231228174147.png]]