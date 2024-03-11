A user with elevated privileges to modify the system
Can create modify or delete any file and run any program (no limitations)
only root users can add new users
Running commands as the root user is bad practice when using Linux:
- Security risk as malicious actors will try to breach the account (logins should be disabled on the root account)
- Irreversible mistakes are more likely to occur e.g. permanently deleting a directory
- Accountability: if a user is running as route there is no way to track who exactly ran a command
[[sudo]] solves the accountability problem ([[Linux Commands]])