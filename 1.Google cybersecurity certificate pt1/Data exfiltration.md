The unauthorized transfer of data from a computer. E.G. IP, intellectual property, PII or trade secrets. Can be sold on the dark web, used for identity theft or leveraged for a competitive advantage.
Steps
 1. Attackers need initial access to a network & computer system. This can be achieved throughout [[social engineering]] attacks like [[phishing]].
 2. Ideally attackers aim to maintain access in the environment and avoid detection for as long as possible. This can be achieved throughout [[lateral movement]].
 3. Attackers then scope out the environment to identify valuable assets (e.g. proprietary code, SPII & PII) throughout searching through locations such as network file shares, [[Intranet]] sites & code repositories.
 4. Attackers must collect package and prepare the data for exfiltration outside of the organizations network. This can be achieved throughout reducing the data size (compression), which helps attackers to hide the stolen data and bypass security controls (e.g. abnormally large file transfers may be blocked by an organizations network configuration).

Defensive measures:
 - Prevent attacker access ([[MFA (Multi-factor authentication)]])
 - Monitor network activity ([[IoC (indicators of compromise)]])
 - Protect assets ([[Asset inventory]], [[Security Controls]], [[Asset Security]])
 - Detect and stop the exfiltration (Large internal file transfers, Large external uploads, unexpected file writes ([[SIEM (Security information and event management)]] tools can detect these activities). Block IP associated with attacker using firewall rules )
