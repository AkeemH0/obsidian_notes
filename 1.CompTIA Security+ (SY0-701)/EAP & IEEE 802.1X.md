[[EAP (Extensible Authentication Protocol)]]
[[IEEE 802.1X]]
Happens automatically behind the scenes once you provide your password
Supplicant- client
Authenticator- Device that provides access (usually switch/access point)
Authentication server- Validates the client credentials (usually backend database with login credentials)
1. Supplicant requests access from authenticator
2. Authenticator sends [[EAP (Extensible Authentication Protocol)]] request for login credentials
3. Supplicant provides [[EAP (Extensible Authentication Protocol)]] response
4. Request passed form authenticator to authentication server
5. If authentication accepting logins it'll ask the authenticator for additional details/credentials from the supplicant
6. Authenticator sends a request to the supplicant for those details/credentials
7. Supplicant provides details/credentials
8. Authenticator sends details/credentials to authentication server
9. Authentication server verifies whether details/credentials are correct/incorrect
10. Authentication server tells authenticator to grant/decline the supplicant network access
![[Pasted image 20240124155007.png]]