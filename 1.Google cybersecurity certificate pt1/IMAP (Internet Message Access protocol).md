**Definition:** 
 An email retrieval protocol that allows messages to be kept on the mail server and accessed from various devices. (unencrypted) (two way communication)
Port 143 TCP [[7.Application Layer OSI]]
Another email protocol used by email clients to retrieve messages from a mail server.
- Unlike [[POP3 (Post Office Protocol version 3)]],  IMAP downloads the header of the content but leaves messages on the server allowing users to access their email from multiple devices and synchronizes the email client with the server.
- Allows users to partially read email before it is finished downloading
- allows syncing of emails
- slower than [[POP3 (Post Office Protocol version 3)]] 