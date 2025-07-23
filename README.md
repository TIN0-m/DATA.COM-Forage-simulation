# DATA.COM-Forage-simulation
In this simulation i was provided with two tasks. The **first task** was to produce a comprehensive investigation report of a cyberattack on a client and the **second task** was to conduct a comprehensive risk assessment
Before i get in to how i did this, id like to express that these resouces that you will get a glimpse of are provided by forage.

## TASK ONE:

**Scope:**         
One of our leading tech corporation clients has fallen prey to a sophisticated cyberattack by a notorious Advanced Persistent Threat (APT) group known as APT34. The attack, believed to be sponsored by a foreign government, has left the organisation's network compromised, and valuable customer data and intellectual property has been stolen.

## Objective 

My goal was to communicate my findings and recommendations effectively to the client's leadership team, providing actionable insights that can improve the corporation's security posture

## Thinking Process

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

## Common Tactics and Techniques (TTPs):

**Spear-phishing:** This is their most common initial access vector. They send highly customized emails (sometimes from compromised accounts) or messages, including via platforms like LinkedIn, often disguised as job offers or legitimate business communications.

**Malware:** They utilize a diverse portfolio of custom-built malware, including backdoors (e.g., Helminth, SaitamaAgent, AgentDrable, EarthquakeRAT, Tonedeaf, SideTwist, StealHook), downloaders (e.g., BondUpdater), credential stealers (e.g., ValueVault, Pickpocket, LaZagne), and web shells (e.g., TwoFace, IntrudingDivisor, HighShell, HyperShell).

**Exploitation:** They exploit known vulnerabilities (including zero-days), especially in public-facing applications like web servers and Microsoft Exchange.

**Privilege Escalation & Lateral Movement:** They use tools like Mimikatz for credential dumping, leverage valid accounts, RDP, VPN, and PowerShell scripts for moving stealthily through networks.

**Data Exfiltration:** Data is exfiltrated using various methods, including HTTP, DNS tunneling, FTP, and even via compromised email accounts.

**Defense Evasion:** They employ techniques like obfuscation, using signed malware, disabling system firewalls, and using anti-sandbox operations to evade detection.

To defend against APT34 and similar threats, a comprehensive cybersecurity strategy is essential. This includes:

**Preventing Initial Access:** Strong email security (anti-phishing, DMARC/SPF/DKIM), continuous security awareness training for employees, and robust web/browser security (WAFs, secure web gateways).

**Hardening Endpoints & Network:** Deploying EDR/XDR, next-gen antivirus, rigorous vulnerability management and patching (especially for public-facing systems), network segmentation, and implementing Zero Trust principles.

**Strong Access Controls:** Enforcing Multi-Factor Authentication (MFA) everywhere, applying the Principle of Least Privilege (PoLP), and using Privileged Access Management (PAM) solutions.

**Enhancing Detection & Response:** Centralized logging with SIEM, integrating up-to-date threat intelligence specific to APT34, proactive threat hunting, and having a well-tested incident response plan.

**Data Protection:** Encrypting sensitive data and maintaining regular, air-gapped, and immutable backups to ensure recovery from destructive attacks.

Essentially, it's about a layered defense, constant vigilance, and adapting your security measures as the threat evolves.

## Task Two

**Scope:**          
you will be documenting the client's risk position using the padlock analogy as an example. The client wants you to help them define the context, assess their risk matrix and identify potential risk scenarios

#Objective 

Conduct a comprehensive risk assessment

## Steps 
It is very important to note that i was provided with an empty template that i had to fill up with my own information.

The first thing i had to do was to fill up the Risk matrix, i decided the best way to scale this would be through a percentage scale ranging from 0 - 99 % spread upon 5 sections of Likelihood and Consequence to determine the risk level. The end result of that ended up looking something like this :
<img width="1294" height="423" alt="Screenshot 2025-07-11 100211" src="https://github.com/user-attachments/assets/0572c6f5-205e-4cfa-a7cd-1baf8f31287f" />

Once that was all sorted i went on to fill up the Risk Assessment, A cybersecurity company faces a unique set of risks due to the nature of its business – it's both a target for sophisticated attacks and responsible for protecting its clients. A comprehensive risk assessment would cover both internal and external threats, with a strong focus on data integrity, client trust, and intellectual property so i decided that the following would be the five assets i would cover:
- Human Error
- Insider Threat
- System Vulnerabilities
- Targeted Attacks
- Compliance Risk

I decided to go into further details covering each one of these 

## Human Error
- Accidental data exposure:    
 Employees inadvertently sharing sensitive client data, internal tools, or vulnerabilities through unsecured channels

- Social Engineering susceptibility:    
Employees falling victim to sophisticated phishing, smishing, or vishing attacks, leading to credential compromise or malware installation. This is particularly critical as they are often targeted.

- Weak password practices:   
Employees using easily guessable or reused passwords for internal systems or client accounts.

- Poor patch management:    
Delaying or failing to apply security patches to internal software, operating systems, and network devices, leaving known vulnerabilities exploitable.

- Bring Your Own Device (BYOD) risks:     
Employees using personal devices for work that may lack adequate security controls, introducing malware or data leakage risks.

## Insider threat
- Data theft:    
Former employees, or contractors intentionally stealing sensitive client data 

- Abuse of privileged access:      
Employees with elevated system privileges misusing their access for personal gain or to cause harm.

- Espionage:        
An insider working with external threat actors to facilitate attacks or data exfiltration.

- Shadow IT:
Employees using unauthorized software, cloud services, or devices without security oversight, creating unmonitored entry points.

## System vulnerabilities 

- Inadequate access controls:
Over-provisioning user permissions, giving employees access to systems or data they don't need for their role .

- Insufficient logging and monitoring:
 Lack of comprehensive logging or ineffective monitoring of internal systems, making it difficult to detect and respond to breaches quickly.

- Poor incident response planning:     
An underdeveloped or untested incident response plan for internal security incidents, leading to slower recovery and increased damage.

- Configuration errors:      
Misconfigurations in internal servers, firewalls, or applications creating security gaps.

- Legacy systems:      
Continued use of outdated or unsupported hardware and software for internal operations, which may have unpatched vulnerabilities.

- Lack of data backup and recovery:             
Insufficient or untested backup and recovery procedures for critical internal data, risking data loss in case of an attack.

## Targeted Attacks
- Advanced Persistent Threats (APTs):   
Highly sophisticated, long-term attacks by state-sponsored groups or well-resourced criminal organizations aiming to steal intellectual property, client data, or disrupt services.

- Ransomware:      
Attackers encrypting the company's internal systems or client data and demanding a ransom. This is a severe threat for a cybersecurity company as it undermines their core value proposition.

- Supply Chain Attacks:      
Attackers compromising a third-party vendor  that the cybersecurity company relies on, to gain access to their systems or client data.

- Distributed Denial of Service (DDoS) Attacks:     
Flooding the company's public-facing services to disrupt operations and make them unavailable to clients.

- Brand Impersonation/Reputational Damage:       
Threat actors creating fake websites, social media accounts, or phishing campaigns impersonating the cybersecurity company to trick clients or damage its reputation.

## Compliance 
- Data privacy regulations (GDPR, POPIA, CCPA, etc.):   
Non-compliance with data protection laws if client data or personal information is mishandled or breached, leading to significant fines and reputational damage.

- Industry-specific regulations:      
Failure to adhere to specific security standards required by industries they serve (e.g., financial services, healthcare).

- Contractual obligations:     
Breaching service level agreements (SLAs) or security clauses in contracts with clients due to a security incident.

Once i had this information all sorted i then filled up the first section of the Risk Assessment as follows:

When choosing the Liklihood and Consequence i was leaning more towards the strict end of things, Setting the baseline high allowed me to feel confident in the risk that could occur
<img width="1196" height="358" alt="Screenshot 2025-07-11 101729" src="https://github.com/user-attachments/assets/8be09445-3157-40c2-a8a3-8f789c5c31d0" />
<img width="1196" height="262" alt="Screenshot 2025-07-11 101809" src="https://github.com/user-attachments/assets/78fcacf7-bee2-4d7d-84f0-f7c2f5188136" />

Once that was all done i moved on to the second section this was about implemting control measures (I also had to decided on if these controls were Excellent,Good,Moderate or Weak) and any additional layers of security( Just like the primary control measures i had to decide if they were Excellent.......I had to decide how to treat the risk if it had additonal controls with these categories Aceept, Treat, Avoid and Trasnfer ). So starting from the top i came up with the following controls. 

## Human Error
- Awareness Training Programs
- Password Policy
- Patch Update Cycle
- Mobile Device Managemt

**Additional Control measures:**                 
Creating Alerts and staying up to date with the latest threats and making sure Employees are aware of these with regualar training events

# Insider Threat 
- Background Checks 
- Implementing Least priviledge
- Application allow list

**Additional Control measure:**            
Having an external source do a bag ground check of employees to ensure the one conducted internally is 100% or making sure nothing was missed on

# System Vulnerabilities
- A Backup System
- Table top exercises
- SIEM and EDR
- Compensating Controlls

**Additional Control measures:**              
Intergrating a cloud service provider to add an additonal layer of security

# Targeted Attacks 
- Load Balacers
- Anti-Malware Software
- Firewalls
- Logging and Monitoring
- Incident Response Plan

**Additonal Control measures:**            
Regular training to ensure security team is up to date with the latest trends

# Complaince 
- Complying with laws regulations
- Creating a baseline
- Meeting the Agreements of SLA

**Additional Control measures:**            
Getting a Legal team to deal with Everything, public Relations Consultations and directly Communicating with the Public

Once i had this down i then proceeded to fill up the remainder of the Risk Assessment as follows: 

<img width="1326" height="356" alt="Screenshot 2025-07-11 101912" src="https://github.com/user-attachments/assets/9ad8aabd-38b1-462b-8fba-ee22df39ced6" />
<img width="1327" height="258" alt="Screenshot 2025-07-11 101940" src="https://github.com/user-attachments/assets/f4e35feb-6d36-4402-85dd-b7506a6b5a06" />

Below i have provided the Excel sheet and an image of the entire Risk Assessment        
[Risk Assessment.xlsx](https://github.com/user-attachments/files/21180255/Risk.Assessment.xlsx)

<img width="1797" height="610" alt="Screenshot 2025-07-11 100916" src="https://github.com/user-attachments/assets/869727e6-d98d-4e66-a6e7-d069676dd09a" />

# Conclusion 
This brings the job simulation to an end, upon this i was provided with a certification of completion and can confidently say that i am compitent in the following:

- I can investigate a cyberattack and produced a comprehensive report documenting findings and outlining key recommendations to improve a client's cybersecurity posture
- I can conduct a comprehensive risk assessment

</a>
  <a href="https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/gCW7Xki5Y3vNpBmnn/yTszJTvkHFBH6zAn3_gCW7Xki5Y3vNpBmnn_mvw8oKQbrDajKM8Sh_1751918583932_completion_certificate.pdf" target="_blank">
  <img src="https://img.shields.io/badge/-DATA.COM-4285F4?&style=for-the-badge" alt="DATA.COM Project Certificate" />
</a>
