Allows the certificate holder to get the OCSP record from the server at regular intervals
Alternative to [[OCSP (Online Certificate Status Protocol)]] 
The server includes a digitally signed (by the CA) OCSP response "stapled" with its SSL/TLS handshake which indicates the revocation status so the user doesn't need to check with the CA. 
Can use a 3rd party server to provide the status information instead of sending with SSL/TLS handshake
eliminates an extra connection needed for OCSP
Speeds up the tunnel creation process