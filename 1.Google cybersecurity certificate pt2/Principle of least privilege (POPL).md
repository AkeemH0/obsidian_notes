similar to [[need to know basis]] but is about access restriction.
Restricts access and permissions to the minimum level necessary for users or systems to perform legitimate tasks. This minimizes the amount of potential vulnerabilities. Reduces the amount of damage a security breach could cause.
also known as [[Least privilege]]
supports the confidentiality, integrity and availability ([[CIA (Confidentiality, Integrity, Availability) triad]]) of information.
- Limits access to sensitive information
- Reduces the chances of accidental data modification, tampering or loss
- supports system monitoring and administration
Reduces the likelihood of a successful attack by connecting specific resources to specific users & limiting what they can do.
related to [[separation of duties]]

- who is the user? : every user should have their own account. Accounts are stored and managed within an organizations directory services. The most common types of user accounts:
   - Owner accounts
   - Group accounts
   - Other accounts
   - Guest accounts: are provided to external users who need to access an internal network like customers, clients, contractors or business partners
   - [[User accounts]]: are assigned to staff based on their job duties
   - Service accounts: are granted to applications of software that needs to interact with other software on the network
   - Administrator/root account
   - Privileged accounts: have elevated permissions or administrative access
   
- How much access do they need to a specific resource? each account should have a baseline access level determined before implementing least privilege. However, appropriate access level can change in different moments e.g. a customer support employee should only have access to your information while they are helping you. Your data should then become inaccessible when the support agent starts working with another customer and they are no longer actively assisting you. Least privilege can only reduce risk if user accounts are routinely and consistently monitored.

  Passwords play an important role when implementing the POPL as even is user accounts are assigned appropriately, an insecure password can compromise your systems.


Periodically auditing accounts helps keep company systems secure
Common approaches to auditing user accounts:

- Usage audits: review which resources each account is accessing and what the user is doing with the resource. Helps to determine whether users are acting in accordance with an organizations security policies. Can also help identify whether a user has permissions that can be revoked because they are no longer being used.

- Privilege audits: Users tend to accumulate more access privileged than they need over time (an issue known as [[privilege creep]]). This might occur if an employee receives a promotion or switches teams and their job duties change. Privilege audits assess whether a users role is in alignment with the resources they have access to.

- Account change audits: Account directory services keep records and logs associated with each user. Changes to an account are usually saved and can be used to audit the directory for suspicious activity, like multiple attempts to change an account password. Performing account change audits helps to ensure that all account changes are made by authorized users. Most directory services can be configured to automatically alert system administrators of suspicious activity.
  
