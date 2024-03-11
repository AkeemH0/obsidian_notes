Allows an HTTPS website to resist impersonation attacks from users who are trying to present fraudulent certificates
Pins public keys to the users web browser as part of HTTP header
If web browser gets different public key from CA then it knows the website was compromised 
*Matches public key provided by browser to public key provided by CA*