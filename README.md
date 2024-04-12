# Running Insecure Environment for 24 Hours and Capture Analytics

In the course of this Azure lab project, my primary focus revolved around fortifying the digital infrastructure while simultaneously exploring potential vulnerabilities. Initially, I initiated the process by establishing the lab account and subscription, followed by the deployment of virtual machines (VMs) encompassing both Windows and Linux operating systems. These foundational steps laid the groundwork for our subsequent security measures.

To mimic a honeypot environment, I intentionally reduced the network's security measures, allowing for a more permissive stance towards inbound traffic. This adjustment was made with the specific goal of creating a scenario conducive to gathering information and creating maps within Microsoft Sentinel. By loosening the restrictions on network security groups, I aimed to entice potential attackers and capture valuable insights into their tactics and techniques. This approach facilitated the generation of comprehensive maps within Microsoft Sentinel, providing a visual representation of the network's interactions and potential vulnerabilities. Transitioning into what I term "attacker mode," I orchestrated simulated breach attempts by fabricating failed authentication logs and executing brute force attacks on the VMs. This practical exercise offered invaluable insights into the intricacies of threat detection and response strategies, thereby augmenting the overall security posture.

Furthermore, I undertook the responsibility of managing user access within Azure Active Directory, coupled with the establishment of log analytics workspaces. The integration of Microsoft Defender for Cloud significantly bolstered our capabilities in terms of real-time threat monitoring and response, thereby enhancing resilience against potential security breaches.

Within the realm of Azure Sentinel, I crafted workbooks, leveraging pre-built JSON maps to visualize and delineate malicious traffic patterns. This proactive approach not only facilitated a clearer understanding of potential threats but also enabled us to take preemptive measures to mitigate them effectively.

Moreover, I established analytics rules within Azure Sentinel to systematically identify potential security breaches. These rules underwent rigorous testing via simulated attacks, ensuring their efficacy in identifying and mitigating security incidents promptly.

Throughout this project, the underlying emphasis was consistently placed on the pivotal role of comprehensive logging and monitoring. This robust framework serves as the cornerstone of our cybersecurity strategy, enabling us to promptly detect and respond to potential threats in a proactive manner. As a result of these concerted efforts, we stand better equipped to safeguard digital assets and combat evolving cyber threats effectively.


## BEFORE SECURING ENVIRONMENT:
	
Start Time	2024-04-11T00:42:16.7427788Z
Stop Time	2024-04-12T00:42:16.7427788Z

Security Events (Windows VMs):	121420
![image](https://github.com/Savier5/Running-Insecure-Environment-for-24-Hours-and-Capture-Analytics/assets/55478673/5f1efa75-bc08-42bc-8c6a-24113216e574)

![image](https://github.com/Savier5/Running-Insecure-Environment-for-24-Hours-and-Capture-Analytics/assets/55478673/333d9746-aea9-44fa-a18b-8f730963fbca)

Syslog (Linux VMs):	3407
![image](https://github.com/Savier5/Running-Insecure-Environment-for-24-Hours-and-Capture-Analytics/assets/55478673/ed35d8e7-8acb-4785-a304-7407b1b0ce0b)

SecurityAlert (Microsoft Defender for Cloud):	6

SecurityIncident (Sentinel Incidents):	241

NSG Inbound Malicious Flows Allowed:	1898
![image](https://github.com/Savier5/Running-Insecure-Environment-for-24-Hours-and-Capture-Analytics/assets/55478673/65117322-abdb-4cf4-a618-e6a1076b3be3)


