# DATA.COM-Forage-simulation
In this simulation i was provided with two tasks. The first task was to produce a comprehensive investigation report of a cyberattack on a client and the second one was to conduct a comprehensive risk assessment
Before i get in to how i did this, id like to express that these resouces that you will get a glimpse of are provided by forage.

# TASK ONE:

Scope: One of our leading tech corporation clients has fallen prey to a sophisticated cyberattack by a notorious Advanced Persistent Threat (APT) group known as APT34. The attack, believed to be sponsored by a foreign government, has left the organisation's network compromised, and valuable customer data and intellectual property has been stolen.

# Objective 

My goal was to communicate my findings and recommendations effectively to the client's leadership team, providing actionable insights that can improve the corporation's security posture

# Thinking Process

to create a an investigation report on an APT i decided to draft a list of questions to be give me a proper understanding of the threat and their motives, here is a list of some of the questions :

- What is their history?
- Which nation/state are they associated with?
- Do they target specific industries?
- What are their motives?
- What are the TTPs they use to conduct their attacks?
- What security measures could the client implement to defend against cyberattacks conducted by this APT?

Once i had these questions it was a matter of research to get clear answers and start drafting the report, i had to make sure that the report met industry standards so i used the MITRE ATT&CK Framework to help guide me. Below will be a list of the websites that i used to conduct my research :

- [https://attack.mitre.org/](https://attack.mitre.org/groups/G0049/)
- https://cyberscoop.com/booz-allen-hamilton-dark-labs-apt34/
- https://www.darkreading.com/cyberattacks-data-breaches/irans-mois-linked-apt34-spies-allies-iraq-yemen
- https://cloud.google.com/blog/topics/threat-intelligence/targeted-attack-in-middle-east-by-apt34/
- https://unit42.paloaltonetworks.com/unit42-oilrig-targets-technology-service-provider-government-agency-quadagent/

With the information gathered from these resouces i managed to create the following report :

APT34 is a suspected Iranian threat group that has targeted Middle Eastern and international victims since at least 2014. The group has targeted a variety of sectors, including financial, government, energy, chemical, and telecommunications. It appears the group carries out supply chain attacks, leveraging the trust relationship between organizations to attack their primary targets. The group works on behalf of the Iranian government based on infrastructure details that contain references to Iran, use of Iranian infrastructure, and targeting that aligns with nation-state interests.

Common Tactics and Techniques (TTPs):

Spear-phishing: This is their most common initial access vector. They send highly customized emails (sometimes from compromised accounts) or messages, including via platforms like LinkedIn, often disguised as job offers or legitimate business communications.

Malware: They utilize a diverse portfolio of custom-built malware, including backdoors (e.g., Helminth, SaitamaAgent, AgentDrable, EarthquakeRAT, Tonedeaf, SideTwist, StealHook), downloaders (e.g., BondUpdater), credential stealers (e.g., ValueVault, Pickpocket, LaZagne), and web shells (e.g., TwoFace, IntrudingDivisor, HighShell, HyperShell).

Exploitation: They exploit known vulnerabilities (including zero-days), especially in public-facing applications like web servers and Microsoft Exchange.

Privilege Escalation & Lateral Movement: They use tools like Mimikatz for credential dumping, leverage valid accounts, RDP, VPN, and PowerShell scripts for moving stealthily through networks.

Data Exfiltration: Data is exfiltrated using various methods, including HTTP, DNS tunneling, FTP, and even via compromised email accounts.

Defense Evasion: They employ techniques like obfuscation, using signed malware, disabling system firewalls, and using anti-sandbox operations to evade detection.

To defend against APT34 and similar threats, a comprehensive cybersecurity strategy is essential. This includes:

Preventing Initial Access: Strong email security (anti-phishing, DMARC/SPF/DKIM), continuous security awareness training for employees, and robust web/browser security (WAFs, secure web gateways).

Hardening Endpoints & Network: Deploying EDR/XDR, next-gen antivirus, rigorous vulnerability management and patching (especially for public-facing systems), network segmentation, and implementing Zero Trust principles.

Strong Access Controls: Enforcing Multi-Factor Authentication (MFA) everywhere, applying the Principle of Least Privilege (PoLP), and using Privileged Access Management (PAM) solutions.

Enhancing Detection & Response: Centralized logging with SIEM, integrating up-to-date threat intelligence specific to APT34, proactive threat hunting, and having a well-tested incident response plan.

Data Protection: Encrypting sensitive data and maintaining regular, air-gapped, and immutable backups to ensure recovery from destructive attacks.

Essentially, it's about a layered defense, constant vigilance, and adapting your security measures as the threat evolves.
