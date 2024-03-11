OpenSSL flaw that allowed people to access the private key of web servers.
This allows for:
- Decryption of HTTPS traffic using [[SSL, TLS  stripping]]
- Impersonation of the server by digitally signing their own certificates
- Inject malicious content into the communications (after [[SSL, TLS  stripping]])