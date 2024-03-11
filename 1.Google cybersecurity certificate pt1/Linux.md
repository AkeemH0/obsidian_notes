An [[open-source]] [[OS (operating system)]] that utilises a command-line interface to tailor the OS.
uses:
Looking at an error log when investigating an issue
verify access and authorization in an identity and access management system
You may use a Linux distribution with a forensic tool to investigate what happened in an event alert
You may use a Linux [[distribution]] for pen testing in offensive security to look for vulnerabilities in the system
Multi-user system, multiple users can use the systems resources at the same time
Order of task completion:
  - [[User]] - initiates tasks or commands that the OS is going to execute.
  - [[Application]]s - a [[package manager]] to install applications
  - [[Shell]]
  - [[Filesystem Hierarchy Standard (FHS)]]
  - [[Kernel]]
  - [[hardware]]


[[echo]] - A Linux command that outputs a specified string of text inputted by the user (a command)
[[String data]] - Data consisting of an ordered sequence of characters
Standard error - Error messages returned by the OS through the shell
expr command carries out arithmetic
[[Linux Commands]]

[[Authorization]]
[[permissions]] in Linux: 
- Read:
   on a file , file contents can be read
   on a directory , all files in that directory can be read
- Write:
   on a file , allows modification of contents of the file
   on a directory , allows creation of new files in that directory
- Execute: 
   on a file , allows execution of executable files
   on a directory , allows a user to enter a directory and access its files
Owners in Linux:
- User - The owner of the file (when you create a file you become the owner of the file but the ownership can be changed)
- Group - consists of several users. Helps manage a multi-user environment
- Other - anyone else with access to the system

File permissions are represented by a 10 character string 
drwxrwxrwx 
d indicates it is a directory 
\ - indicates a regular file 
r indicates the user has read permissions
w indicates the user has write permissions
x indicates the user has execute permissions
if one of the permissions were missing there would be a \- instead
the 2nd to 4th characters are for the user
the 5th to 7th characters are for the group
the 8th to 10th characters are for other
(pairs of three for each owner)

Options modify the behaviour of the command

ls -l displays permissions to files and directories
ls -a displays hidden files and directories
ls -la displays permissions of files and directories including hidden files and directories (options can be added in any order so ls-al also works)
hidden files appear with a . before their name

chmod changes permissions on files and directories




