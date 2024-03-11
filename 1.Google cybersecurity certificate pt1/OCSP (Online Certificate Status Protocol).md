**Definition:** 
 A protocol used to check the validity of a digital certificate's status in real-time.

A protocol used to check the revocation status of digital certificates using their serial number
Alternative to [[CRL (Certificate Revocation List)]] as it operates more quickly and efficiently as it doesn't use encryption (makes it less secure) and only looks up one digital certificate at a time.
More efficient than downloading the whole [[CRL (Certificate Revocation List)]]
[[OCSP stapling]] is more efficient than OCSP

Most browsers support OCSP, not all do

