(super user do)
temporarily grants elevated permissions to specific users
Will prompt you to enter the password for the user you're currently logged in as
Users must be granted access through a configuration file called the sudoers file
Still at risk in the event of an attack since elevated permissions can be accessed by intruders by using sudo on a sudoers account, therefore only users who need sudo to carry out their task should have sudo permissions.
sudo allows users to bypass the typical security controls that are in place to prevent elevated access to an attacker.

