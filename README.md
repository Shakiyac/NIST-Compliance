Implementing Security Controls Towards NIST SP 800-53 R5 Compliance

<img width="1055" height="375" alt="image" src="https://github.com/user-attachments/assets/7b7ee99f-e535-4de0-9983-72b752a16d8a" />

Introduction

In this project, I remediate my mini honeynet I created in the previous project (Building a SOC + Honenet) to be up to par and compliant with NIST SP 800 53 R5 regulatory compliance standards. I resolved several non-compliant controls within the security metrics in Microsoft Azure to harden the environment and decrease/nullify attacks as well as keeping the environment up to compliant standards. The compliance metrics we will mitigate and audit are:

AC: Access Control

AU: Audit and Accountability

CP: Contingency Planning

IA: Identification and Authentication

IR: Incident Response

RA: Risk Assessment

SC: System and Communications Protection

SI: System and Information Integrity

Ratings Before Hardening/Security Controls

<img width="1690" height="486" alt="image" src="https://github.com/user-attachments/assets/7ef6b1dd-fcd0-4781-93bb-2aa798b8801b" />
<img width="1074" height="840" alt="image" src="https://github.com/user-attachments/assets/00c51e70-fc63-44c5-b739-2dbee9a40004" />

Metrics Before Hardening /Security Controls

Some of the more common compliance issues were the lack of encryption & having email notifications for security alerts. as well as Microsoft Defender configuration/

<img width="1592" height="588" alt="image" src="https://github.com/user-attachments/assets/37b293ac-24e9-4b62-a32f-b5beb0a2fa21" />

In addition to regular compliance issues there were “Quick Fixes”, such as Microsoft defender being enabled for different sources to match approved compliant status, with a HIGH severity.

<img width="1628" height="415" alt="image" src="https://github.com/user-attachments/assets/54558e31-7dbe-4334-b52e-4d926de1151d" />
<img width="1302" height="466" alt="image" src="https://github.com/user-attachments/assets/e971901b-ce9a-4514-ad70-fe3de50bd2ea" />

Each compliance tool had different freshness intervals as well from the lower end 30 minutes to 24 hours to verify compliance approval.

IMPLEMENTATION:

We started with the AC: Access control compliance controls with AC: 2 and ended with putting the SC: System and Communications Protection to compliance. Throughout I implemented both the Manual option options as well as Quick Fix & exemption tools when applicable.

<img width="2610" height="1584" alt="image" src="https://github.com/user-attachments/assets/7515a9fa-1da8-4fcf-afbb-86a2ee8a3f60" />
<img width="3526" height="1832" alt="image" src="https://github.com/user-attachments/assets/e702af44-8506-440a-94cc-931508e029e7" />

⭐ Some Of The Common Remediation Functions To Fix:


Firewall Creations for VMs (linux/Windows)

Email Notifications

Exemptions

Enabling of Microsoft defender for resource manager, DNS, etc.

Azure Backup for virtual machines

Purge Protection

Subnets associated with network security groups

⭐ Some Of The Common Techniques (categories) Fixed during remediation.

Defense Evasion (https://attack.mitre.org/tactics/TA0005/)

Privilege Escalation (https://attack.mitre.org/tactics/TA0004/)

Impact (https://attack.mitre.org/tactics/TA0040/)

Persistence (https://attack.mitre.org/tactics/TA0003/)

Exfiltration (https://attack.mitre.org/tactics/TA0011/)

Lateral Movement (https://attack.mitre.org/tactics/TA0008/)

Ratings AFTER Hardening/ Security Controls

The metrics shown below is after 24 hours of our last policy edit, showing increase in not only the NIST framework but also in the Microsoft Cloud security Benchmark controls as well.

<img width="1909" height="850" alt="image" src="https://github.com/user-attachments/assets/f9abc6b1-cd92-4b63-8412-674b432e2e48" />

Metrics AFTER Hardening/ Security Controls

As shown below majority of all compliance policies were mitigated

<img width="1923" height="881" alt="image" src="https://github.com/user-attachments/assets/7ec4bfd7-aa55-4b06-9903-9930ff1573ac" />

Conclusion

In this project, NIST SP 800 53 R5 policy changes were made within the Azure environment to become more compliant with regulations. Utilizing the tools available we were able to create firewalls for our virtual machines, create backups for virtual machines, create subnets with our NSGS, enable Microsoft Defender for several resources and more. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness as shown in previous Azure SOC + Honeynet lab

It is worth noting that remediating the environment to be more compliant with NIST SP 800 53 5 also increased our compliance with the Microsoft Cloud Security Benchmark (Azure default), increasing our overall score to a whopping 88% Secure Score!

<img width="1069" height="461" alt="image" src="https://github.com/user-attachments/assets/717ecd65-ac4b-432e-8ce4-ba74479b6baf" />
