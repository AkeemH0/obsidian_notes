`echo -n (text) | md5sum` used to calculate the md5 hash of **text**
(hashing algorithm is Interchangeable)
`sha256sum`(file path) used to calculate the sha 256 hash of a **file**

`echo`"text" `| base64` used to encode text to base64/base32(change 64 to 32)
![[Pasted image 20240223084014.png|300]]
`echo `"text" `|base64` -d used to decode text from base64/base32(change 64 to 32)
![[Pasted image 20240223084024.png|300]]

`sudo echo $RANDOM` PRNG 0-32767
`od -An -N`(bytes) `-i /dev/random` PRNG with adjustable number of bytes

var/log service examples: access logs, error logs & firewall logs

`dpkg` is a package installer
using apt means whenever the system is updated the pieces of software are also updated whereas this is not the case when using dpkg
`apt` uses to add approved repositories
`add-apt-repository` used to add community repositories


cron process: scheduled tasks/actions for after the system has booted
`crontab`s: stores scheduled processes 
required values: (* can be used to provide no  value)
MIN HOUR DOM MON DOW CMD
MIN minute to execute at
HOUR hour to execute at
DOM day of month to execute at
MON month of year to execute at
DOW day of week to execute at
CMD command to execute
OR
@reboot 
`crontab -e` (used for editing cronlabs)
[Crontab Generator](https://crontab-generator.org/) can be used to check a cron commands execute times


`fg` used to foreground a process

ctrl + z used to background a process (instead of using & operator)

processes PIDs are based on the order they were launched in so PID 0 is the process that starts when the system boots (system's init **systemd**, sits between OS & user and manages user processes)

processes/services can be set to run on boot by admins.
`systemctl` (option) (PID) used to manage a process/services
options: 
`start`, `stop`: instance of process
`enable` , `disable`: start-up of process
e.g. `systemctl enable myservice`
Processes can run in 2 states: background or foreground

`kill SIGSTOP ` (PID) Stop/suspend a process
`kill SIGKILL` (PID) Kill the process - doesn't do any clean up after the fact
`kill SIGTERM ` (PID)  Kill the process, but allow it to do some clean-up tasks beforehand
`kill`(PID) used to end a specific process 
PID is interchangeable with process name for many commands
`top` shows a process display like task manager

`ps` shows running processes from our user's sessions
`ps aux `shows running processes from other users and processes that don't run from a session (system processes) (shows background & foreground processes)

![[Pasted image 20240220084930.png]]
![[Pasted image 20240220084907.png]]

- `python3 -m http.server` turns your computer into a http web server to host your own files in a specific directory e.g. webserver directory
- python 3 webserver runs in the terminal until you cancel it & then the webserver is down
- python3 webserver is port 8000
- flaw of python3 webserver is that its http and that u can't index therefore u must know the exact name and location of the file (updog (downloadable command)  has indexing & HTTPS)
- `scp` (local_file_name) **Source**(remote_user_name@remote_user_ip:file_path_and_file_name) **Dest**
- Source and destination can be swapped
- e.g.`scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt` (upload file to remote server)
- e.g. `scp ubuntu@192.168.1.30:/home/ubuntu/transferred.txt important.txt` (download file from remote server)
  secure copy (uses SSH, secure file transfer to and from remote system, (need to know the usernames and passwords for a user on your current system and a user on the remote system))
- `wget` used to download files from webservers (web get), (the downloaded file may be hidden due to file attributes and permissions set by the server)
- e.g. `wget https://assets.tryhackme.com/additional/linux-fundamentals/part3/myfile.txt
- e.g.`wget http://10.10.124.175:8000/myfile`

---
- `echo` - outputs the string of text entered by the user

- `pwd` - print working directory onto the screen (tells you which directory you're in)

- `ls` - list. Displays the names of files and directories in the current working directory or in the chosen directory e.g. ls /home/analyst/projects (from any directory), ls projects (if already in analyst directory)

ls -a lists all

- `cd` -  change directories. Can travel to any using absolute file path or subdirectories using relative file path. cd.. sends you to the parent directory

- `cat` - Displays the content of a file
- `head` - Displays the beginning of a file (10 lines by default but can be chosen by using "head -n *number* filename.txt''  )
- `tail` - displays the end of a file (10 lines by default but can be chosen by using "tail -n *number* filename.txt") can be used to read the most recent information in a log file
write command and then file name for cat & head

- `less`- returns the content of a file one page at a time. space bar : move forward one page. b: move back one page. down arrow : move forward one line. Up arrow: move back one line. q: quit and return to the previous window.

- `man hier` - tells you about the FHS and its standard directories

- `whoami` - returns your username

- `grep`- searches a specified file and returns all lines in the file containing a specified string . e.g. grep *string* filename.txt

- `|` ([[piping]]) : sends the standard output of one command as standard input to another command for further processing

e.g. ls /home/analyst/reports | grep users
piping takes the output of the ls command (files and subdirectories from reports) and searches for the word users using the grep command
e.g. if reports had files user.txt & example.txt then only user.txt would be returned as it contains the relevant string of characters

- `find` - searches for directories and files that meet specified criteria:
- specific string in name (-name (case sensitive) or -iname (case insensitive))
- certain file size
- last modified within a certain time frame (-mtime)
- find /home/analyst/projects - name "* example * ". is case sensitive
- find /home/analyst/projects - iname " * example * ". isn't case sensitive
    *  is a wildcard that represents 0 or more characters
- find /home/analyst/projects -mtime -3 returns all files and directories in the projects directory that have been modified within the past three days

-  `-mtime +1` indicates all files or directories last modified more than one day ago

-  `-mtime -1` indicates all files or directories last modified less than one day ago

-  `-mmin` can be used instead of -mtime if you want to base the search on minutes rather than days

-  `mkdir` - makes directory
e.g. `mkdir dir1 dir2` makes 2 directories simultaneously
-  `rmdir` - removes directory (can only remove if the dir is empty)
-  `touch` - creates new file
-  `rm` - removes file
- `file` (filename) - determines the type of a file e.g. `file note1` could return ASCII text
- `mv` - moves a file or directory to a new location (be in the directory of the file, indicate the file to be moved, indicate where to move it)
e.g. mv email_policy.txt /home/analyst/drafts
can also be used to rename files by passing the new name in as the second argument 
e.g. `mv permissions.txt perm.txt`
e.g. `mv note2 note3`
e.g. `mv note1` ..
e.g. `mv note2 note 3 noteholder ` (moves all previous files and directories into the last directory
)
`userdel `(user) 
`groups` lists all groups your account is part of
`whatis`
`su` (user) switch user  e.g. `su user2`
files move just how the user moves (cd)
You can have the same names file in two different directories (bad practice as if you move them in the same directory the one you moved into the directory will take precedence and delete the other
- `cp` - copies a file or directory into a new location
e.g. cp permissions.txt /home/analyst/logs
e.g. cp note1 note2

- `nano` - used to edit files e.g. nano newfile.txt opens the file so that it can be edited
can also be used to create a new file
ctrl + O to save in nano
ctrl + x to exit out of nano 
echo > overwrites an existing file 
echo >> adds content at the end of an existing file
rm & echo> should be used carefully because its not easy to recover deleted information
e.g. cd home/akeem/newdirectory
       echo "new message" >> newfile.txt 
       adds the string new message to the file
       echo "overwrite message" > newfile.txt 
       replaces the content of the file with the string overwrite message 
       > & >> will create a new file if one doesn't already exist with the specified name
- `ls -l` displays permissions to files and directories
- `ls -a` displays hidden files and directories
- `ls -la`/`ls -al` displays permissions of files and directories including hidden files and directories (options can be added in any order so ls-al also works)
hidden files appear with a . before their name

- `chmod` changes permissions on files and directories
![[Pasted image 20230928170332.png]]
u=user
g=group
o=other
so the group is gaining write permissions 
the other is losing read permissions

`chmod u+rwx,g+rwx,o+rwx login_sessions.txt` grants all permissions
`chmod u-rwx,g-rwx,o-rwx login_sessions.txt` removes all permissions

`chmod u=r,g=r,o=r login_sessions.txt` makes everyone have ONLY the specified permissions so everyone can only read as every other pre existing permission is removed

e.g. `chmod u=wx,g=wx,o=wx login_sessions.txt` makes everyone only have write and execute permissions

commas separate each owner type, there shouldn't be spaces in between the commas

[[sudo]] temporarily grants elevated permissions to specific users

- `useradd`: adds a user to the system e.g. `sudo useradd newuser3`

`-g` sets the users default group also known as their primary group
e.g.` sudo useradd -g security newuser3` 

`-G` adds the user to additional groups also called supplemental or secondary groups
e.g.  `sudo useradd -G admin,finance newuser3`

`userdel`: deletes a user from the system
can only be done with elevated privileges (root or sudo)
doesn't delete the files in the users home directory unless you use the -r option
e.g. `sudo userdel -r newuser3`
before deleting any user files you should ensure you have backups in case you need them later
Instead of deleting the user you could consider deactivating their account with user mod -L to prevent the user from logging in while still giving you access to their account and associated permissions. For example, if a user left an organization, this option would allow you to identify which files they have ownership over, so you could move this ownership to others.

`usermod` : modifies existing user accounts. The same `-g` & `-G` commands can be used
e.g. `sudo usermod -g executive newuser3` would change newuser3s' primary group the executive group
to add a supplemental group for a user you need to use the -G option proceeding with -a 
e.g. `sudo usermod -a -G marketing newuser3` would add newuser3 to the marketing group as a secondary group
can be used in conjunction with:
`-d`: Changes the user's home directory
`-l`: Changes the User's login name
`-L`: Locks the account so the user can't log in
e.g. `sudo usermod -d /home/newuserdirectory newuser3`

`chown`: changes ownership of a file or directory.
e.g. `sudo chown newuser3 access.txt` changes the user owner of access.txt to newuser3
e.g. `sudo chown :security access.txt` changes the group owner of access.txt to newuser3
The `:` indicates that the group owner is being changed whilst no `:` indicates that the user owner is being changed


when you create a new user in Linux a group with the same name as the user is automatically created and the user is the only member of that group. After removing users, it is good practice to clean up any such empty groups that may remain behind.
![[Pasted image 20231004183757.png]]
user researcher9 was removed however the group researcher9 wasn't removed therefore we had to remove it separately

`man` (command) : displays information on other commands and how they work
press Q to exit the manual page
(command)`-h`/(command)`--help`: displays possible options the command accepts
`whatis` : displays a description of a command on a single line
`apropos`: searches the manual page descriptions for a specified string 
e.g. `apropos password`
e.g. `apropos -a change password `
you use -a when you want to look up multiple strings

`sqlite3` enables SQLite commands ([[SQL (Structured Query Language)]])

`sha256sum` hashes the contents of a file

`curl` used to open websites (e.g. curl opensource.google.com)

encrypt AES-256
`openssl enc -aes-256-cbc -a -nosalt -in [input file] -out [output file]`

decrypt AES-256
`openssl enc -aes-256-cbc -d -nosalt -in [input file] -out [output file]`

Decrypt RSA private key

`openssl rsautl -decrypt -inkey [private key file] -in [input file] -out [output file]`

`jq` used for displaying JSON data in a more readable format (instead of using cat)

- `&` allows you to run commands in the terminal background (goes at the end of the command) (good for copying files since the command runs in the background so we can continue to use the terminal)
- `&&` allows you to combine multiple commands together in one line of your terminal 
- `\>` (redirector) takes the output of one command and creates it as a new file (overwrites pre-existing)
- `\>>` (redirector) takes the output of one command and adds it onto a file (adds onto pre-existing)
- `|` take the output of one command and use it as an input for another command
