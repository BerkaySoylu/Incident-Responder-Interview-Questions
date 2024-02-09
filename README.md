 ## Contribute

Let's make this repository full of interview questions!

This repository is maintained by [**LetsDefend**](https://letsdefend.io/). If you think any interview question is missing or incorrect, please feel free to **submit a pull request (PR)** to this repo. We will review the PR and merge if appropriate.

# Incident Responder Interview Questions

## Table of Contents

- What should you expect?
- Pre-preparing
- General Incident Response Interview Questions
- Network Related Incident Response Interview Questions
- Event Log Analysis Related Incident Response Interview Questions
- Digital Forensics & Incident Response (DFIR) Interview Questions
- References

## What should you expect?

Below is a list of the topics on which questions can be asked in the interview.

## Pre-preparing

 - First, fully understand what kind of role you are applying for. Like if you're applying Security Analyst (Tier 1 Analyst) job, then you should already know what Security Analysts do or what difficulties SOC Analysts are having.
 - Make sure that you know about the company you are applying for. Are you going to give support to multiple companies at the same time or they are looking for internal SOC?
 - If you have any friend who is working at the company you're applying for, make a phone call and ask what kind of difficulties your friend is having.
 - Do not tell your salary expectation during the interview. Answer like: "I think my salary expectations are within your scale. In case of positive progress, I am open to your suggestions at the proposal stage."
 - Make sure you know the salary scale of the job you're applying. You can ask on Reddit.


## General Incident Response Interview Questions:

### What is an incident?

The National Cyber Security Centre (NCSC) defines a cyber incident as a breach of a system's security policy in order to affect its integrity or availability and/or the unauthorized access or attempted access to a system or systems; in line with the Computer Misuse Act. 

In general, an incident is a violation of computer security policies, acceptable use policies, or standard computer security practices. (NIST)
Examples of incidents are:
 - An attacker commands a botnet to send high volumes of connection requests to one of an
organization’s web servers, causing it to crash.
 - Users are tricked into opening a “quarterly report” sent via email that is actually malware;
running the tool has infected their computers and established connections with an external
host.

### What is incident handling - incident response?

Incident handling is the process of detecting and analyzing incidents and limiting the incident’s effect. For example, if an attacker breaks into a system through the Internet, the incident handling process should detect the security breach. Incident handlers will then analyze the data and determine how serious the attack is. The incident will be prioritized, and the incident handlers will take action to ensure that the progress of the incident is halted and that the affected systems return to normal operation as soon as possible.

### Can you explain the Incident Response Life Cycle and its key phases?

The NIST incident response lifecycle breaks incident response down into four main phases: Preparation; Detection and Analysis; Containment, Eradication, and Recovery; and Post-Event Activity.

[Resim]

### How do you prioritize and classify incidents based on their severity and impact?

Incidents can be classified based on severity, impact, and likelihood of occurrence. Prioritization should consider factors such as potential damage, criticality of affected systems, and regulatory requirements.

### What are the common sources of incident alerts?

Common sources include intrusion detection systems (IDS), security information and event management (SIEM) solutions, antivirus software, firewalls, and user reports.

### What are the common indicators of a security incident?

Common indicators include unusual network traffic patterns, unauthorized access attempts, unexpected system behavior, and malware infections.

### What is the difference between an incident and an event in the context of cybersecurity?

An event is any observable occurrence in a system or network, while an incident is an event that has a negative impact on the confidentiality, integrity, or availability of information or IT services.

### Define the term "indicators of compromise" (IOCs) and explain how they are used in incident response.

Indicators of compromise (IOCs) are artifacts or behaviors that indicate the presence of a security incident or compromise. They can include IP addresses, domain names, file hashes, registry keys, and patterns of network traffic. IOCs are used to detect, investigate, and remediate security incidents.

### What are Indicators of Attack (IOAs) in incident response, and how do they differ from Indicators of Compromise (IOCs)?

Indicators of Attack (IOAs) are behavioral patterns or forensic artifacts observed within an organization's network or systems that suggest the presence of an active cyberattack. These indicators focus on detecting the tactics, techniques, and procedures (TTPs) used by attackers during different stages of an attack. Unlike Indicators of Compromise (IOCs), which are based on known patterns of malicious activity, IOAs provide insights into ongoing or potential attacks based on observed behaviors rather than predefined signatures or patterns. While IOCs are reactive and often indicate that a compromise has already occurred, IOAs enable proactive threat detection and response by identifying suspicious activities indicative of an attack in progress.

### What is the difference between an indicator of compromise (IOC) and a signature in the context of cybersecurity?

An indicator of compromise (IOC) is any observable evidence or artifact that may indicate an ongoing or past security incident, such as suspicious network traffic patterns, unauthorized file modifications, or unusual system behavior. A signature is a specific pattern or characteristic associated with a known threat or vulnerability that can be used to detect and block malicious activity, often implemented in intrusion detection and prevention systems (IDS/IPS).

### Explain the difference between proactive and reactive incident response strategies.

Proactive incident response involves implementing preventive measures and proactive monitoring to identify and mitigate security risks before they escalate into incidents. 
Reactive incident response, on the other hand, focuses on responding to security incidents after they have occurred, including detection, analysis, containment, eradication, and recovery activities.

### What Is Root Cause Analysis?

Root cause analysis, sometimes called RCA, is a formal effort to determine and document the root cause of an incident, then take preventative steps to ensure the same issue doesn’t happen again.


## Network Related Incident Response Interview Questions:

### Explain the concept of packet analysis and its role in network incident response. What tools do you commonly use for packet analysis?

Packet analysis involves examining network packets to understand communication patterns, identify anomalies, and detect malicious activity. Tools like Wireshark and tcpdump are commonly used for packet capture and analysis.

### Define the term "command-and-control (C2) server" and explain its significance in network incident response. How do you detect and block C2 communications during an incident?

A command-and-control (C2) server is a remote server used by attackers to send commands to compromised systems and exfiltrate stolen data. Detecting and blocking C2 communications is crucial for disrupting the attacker's control over compromised systems and preventing further data exfiltration or malicious activity. Techniques for detecting and blocking C2 communications include network traffic analysis, intrusion detection and prevention systems (IDPS), and endpoint security controls.

### Explain the concept of "intrusion detection" and its role in network incident response. How do intrusion detection systems (IDS) help identify and mitigate network threats?

Intrusion detection involves monitoring network traffic and system logs for signs of unauthorized access, malicious activities, or security policy violations. Intrusion detection systems (IDS) analyze network traffic patterns and behavior to identify potential security threats and alert security teams in real-time. IDS play a crucial role in early threat detection, incident triage, and response coordination.

### Define the term "honeypot" and discuss its use in network incident response. How can deploying honeypots help organizations detect and respond to network threats?

A honeypot is a decoy system or network designed to attract and deceive attackers, allowing security teams to observe and analyze their tactics, techniques, and procedures (TTPs). Deploying honeypots enables organizations to gather threat intelligence, identify emerging attack trends, and improve incident response capabilities. By luring attackers away from critical systems, honeypots help mitigate the risk of actual compromise and provide valuable insights for proactive threat mitigation.


## Event Log Analysis Related Incident Response Interview Questions:

### How is event log analysis conducted to detect and respond to security incidents?

Event log analysis involves establishing baseline behavior, identifying anomalies, and prioritizing alerts based on severity. Automated tools and correlation rules are utilized to streamline the analysis process. Once an incident is detected, further investigation, evidence gathering, and response actions are taken.

### What methods are used to identify anomalous activities in Windows event logs during incident response?
Methods for identifying anomalous activities in Windows event logs include focusing on critical events such as failed login attempts, account modifications, and privilege changes. Custom alerts and filters are created to quickly identify suspicious patterns indicative of security incidents, such as brute force attacks or data exfiltration attempts.

### Why is event log correlation significant in incident response, and how are logs correlated from different sources for comprehensive analysis?
Event log correlation is essential as it helps identify relationships and patterns across multiple data sources. By correlating logs from various sources such as servers, endpoints, firewalls, and IDS/IPS systems, a comprehensive view of security events is obtained. Correlation rules and SIEM platforms automate this process, facilitating real-time detection and response to security incidents.

### In the context of incident response, how are situations managed where logs may have been manipulated or altered by attackers?
When dealing with manipulated or altered logs, reliance on backup and archival systems to preserve original log data for forensic analysis is key. Tamper-evident logging mechanisms and log integrity monitoring using cryptographic hashes or digital signatures are implemented. Network-based logging and log forwarding to secure, off-site locations also mitigate the risk of tampering.

### Can you provide an example of a security incident where event log analysis played a critical role in identifying the root cause?
As an example; By analyzing firewall logs and correlating them with Windows event logs from affected servers, a compromised user account used for data exfiltration to an external IP address was identified. Unauthorized access attempts and suspicious file transfers revealed through event log analysis led to the discovery and remediation of the breach before significant data loss occurred.

## Digital Forensics & Incident Response (DFIR) Interview Questions:

### Explain the importance of creating a timeline during a digital forensics investigation. How does a timeline aid in understanding the sequence of events and identifying potential evidence?
A timeline created during a digital forensics investigation is crucial for incident response as it helps reconstruct the sequence of events leading up to and during a security incident. By correlating timestamps from various sources such as system logs, network traffic, and user activity, the timeline provides insights into the attacker's actions, the timeline of the incident, and the affected systems. This information is invaluable for understanding the scope of the incident, identifying potential evidence, and formulating an effective response strategy.

### Describe the process of conducting triage in digital forensics. What criteria do you use to prioritize evidence collection and analysis during triage?
Triage in digital forensics is akin to incident response's initial response phase, focusing on quickly identifying and prioritizing critical evidence while minimizing the impact of the incident. During triage, evidence is prioritized based on factors such as the severity of the incident, the potential impact on business operations, and the relevance to the investigation's objectives. The goal is to collect and preserve essential evidence promptly, allowing for immediate analysis and response actions to mitigate further damage and contain the incident.

### How do you acquire a forensic image of a digital device? Discuss the best practices and tools used for creating a forensically sound image while maintaining the integrity of the evidence.
Acquiring a forensic image of a digital device is a critical step in both digital forensics and incident response. Best practices involve using write-blocking hardware or software to prevent alterations to the original data and ensuring the integrity of the evidence. Tools such as EnCase, FTK Imager, and dd (Linux command) are commonly used for imaging. During incident response, rapid acquisition of forensic images allows for the preservation of volatile evidence and facilitates analysis to determine the scope and impact of the incident.

### What are some key Windows artifacts commonly analyzed during a digital forensics investigation? Provide examples of important artifacts and explain how they can contribute to the investigation process.
Windows artifacts such as event logs, registry hives, prefetch files, link files (LNK), and user activity logs are commonly analyzed during digital forensics investigations and incident response. Event logs provide a chronological record of system events, while registry hives contain configuration and user data critical for understanding system activity. Prefetch files store metadata about application execution, and link files provide insights into recently accessed files and applications. Analyzing these artifacts helps reconstruct the attacker's actions, identify compromised systems, and determine the extent of the intrusion.

### Explain the role of volatile data collection in digital forensics. What types of volatile data are typically collected from live systems, and how is this data used in an investigation?
Volatile data collection involves capturing live system information such as running processes, network connections, open files, and system memory. In incident response, volatile data collection provides real-time insights into ongoing attacks, malware behavior, and active network connections. Analysis of volatile data helps identify malicious processes, detect unauthorized access, and gather evidence of attacker activity. By collecting volatile data promptly during incident response, responders can capture critical evidence before it is lost due to system shutdowns or volatile memory clearing.

### Explain the concept of 'order of volatility' in digital forensics and incident response. How does it influence the collection and preservation of evidence during an investigation?
- The 'order of volatility' principle dictates the sequence in which digital artifacts or evidence should be collected and preserved during an investigation.
- It prioritizes the collection of volatile data, such as system memory and network connections, which is prone to loss or alteration.
- Volatile data is gathered first to capture real-time information about active processes and system state.
- Less volatile data, such as log files and registry entries, is collected subsequently.
- Following this principle ensures the preservation of critical evidence and enhances the effectiveness of the investigation.



















## References

 - https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-61r2.pdf
 - https://csrc.nist.gov/
 - https://www.cisa.gov/
 - https://www.sans.org/
