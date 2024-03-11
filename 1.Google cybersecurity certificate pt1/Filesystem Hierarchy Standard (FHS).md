The component of the Linux OS that organizes data
Specifies the location where data is stored in the [[OS (operating system)]]

The FHS defines how directories , [[directory]] contents and other storage is organizes so the operating system knows where to find specific data.

[[Root directory]] is the highest-level directory in Linux identified by a /
![[Pasted image 20230928125533.png]]
File path e.g. /home/analyst/logs

/home:  every user has their own home directory

/bin:  stands for binary, contains binary files and other executables. Executables are files that contain a series of commands a computer needs to follow to run programs and perform other functions

/etc: stores the systems configuration files

/tmp : stores temporary files. Commonly used by attackers because anyone in the system can modify data in these files

/mnt: stands for mount, stores media such as USB drives and hard drives.

users home directory can be represented as ~    
(home/akeem) is represented as ~
you can navigate to specific subdirectories using their absolute or relative file paths.
absolute file path is the full file path starting from the route
relative file path is the file path that starts from a users current directory

relative file paths can use a dot (.) to represent the current directory
relative file paths can use two dots (..) to represent the parent of the current directory