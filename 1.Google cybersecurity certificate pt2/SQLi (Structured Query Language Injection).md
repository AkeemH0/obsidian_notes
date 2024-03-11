**Definition:** 
 A type of cyber attack where malicious SQL statements are used to manipulate a database.

An attack that executes unexpected queries on a database
Occurs due to a lack of sanitized input
Can be used to manipulate databases, steal sensitive data, take control of vulnerable applications & carry out a denial of service
injections take place in areas of the website that are designed to accept user input (input fields such as login forms, search bars or comment submission boxes.) e.g. the login form for a site which triggers a backend SQL statement. Web forms are designed to copy user input into the statement exactly as they're written. The statement then sends a request to the server which runs the query. Websites that are vulnerable to SQL injection insert the user's input exactly as its entered before running the code. An attacker might insert additional SQL code which could cause the server to run a harmful query of code that it wasn't expecting. Malicious hackers can target these attack vectors to obtain sensitive information, modify tables and gain administrative rights to the database.

` ' OR '1'='1'` is a common way to ask for everything in a database

The best way to defend against SQL injection is code that will sanitize the input. Developers can write code to search for specific SQL characters giving the [[server]] a clearer idea of what inputs to expect. This can be done throughout [[Prepared statement]]

Three categories of SQL injection:
- [[In-band SQL injection]]
- [[Out-of-band SQL injection]]
- [[Inferential SQL injection]]

SQL injection Prevention (a key to preventing SQL injection attacks is to [[escape user input]]):
- [[Prepared statement]]s
- [[Input sanitization]]
- [[Input validation]]
- [[WAF (Web Application Firewall)]]
A combination of these techniques can help prevent SQL injection attacks.









[[SQL (Structured Query Language)]]
[[Database]]