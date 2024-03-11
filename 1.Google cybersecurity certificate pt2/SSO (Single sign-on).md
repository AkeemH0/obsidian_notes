**Definition:** 
 A session/user authentication process that enables a user to access multiple applications with a single set of login credentials.
- A technology that combines several different logins into one preventing users from having to authenticate repeatedly
- Establishes a users identity once allowing them to access resources faster
- improves user experience by reducing the number of usernames and passwords people have to remember
- lowers company costs by streamlining how they manage connected services
- Improves overall security by reducing the number of access points attackers can target (reduces [[attack surface]])
- introduced to combat [[password fatigue]]
- SSO automates how trust is established between a user and a service provider by using trusted third-parties to prove that a user is who they claim to be throughout the exchange of encrypted access tokens between the identity provider and the service provider. These access tokens are exchanged using LDAP and SAML protocols.
- Usually on a timer/condition (reverify identity after x hours or after system logoff)
[[LDAP (Lightweight Directory Access Protocol)]] is used to transmit information on-premises
[[SAML (Security Assertion Markup Language)]]  is used to transmit information off-premises (e.g. the cloud)
LDAP & SAML are often used in conjunction
[[OpenID]] often used for SSO
[[OAUTH (Open Authorization)]] often used for SSO
[[Identity federation]]
![[Pasted image 20231013153846.png]]
  limitation of SSO: a lost or stolen password could expose information across multiple services (MFA prevents this)
  *magic key that temporarily opens everything once you provide valid identification*
