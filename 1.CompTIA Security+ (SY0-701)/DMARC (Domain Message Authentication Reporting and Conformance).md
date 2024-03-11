**Definition:** 
 An email authentication protocol that uses SPF (Sender Policy Framework) and DKIM (DomainKeys Identified Mail) to prevent email spoofing.
 - An extension of [[SPF (Sender Policy Framework)]] & [[DKIM (DomainKeys Identified Mail)]] that defines what to do with emails that don't properly validate (chosen by domain owner in [[DNS TXT record]](DMARC policy examples: ``none`` (no action, monitor only), ``quarantine`` (send to spam) or ``reject``)
 - `v=DMARC1; p=reject; rua=mailto:dmarc@example.com`
 - `v` version: specifies DMARC record version
 - `p` policy: specifies action to be taken after failed validation
 - `rua` aggregate report: specifies the email address to which aggregate (summary) reports are sent to
 - ![[Pasted image 20240213135715.png|setting DMARC policies in DNS TXT record |500]]
 - ![[Pasted image 20240213135846.png|DMARC aggregated reports|600]]

 