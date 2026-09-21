<img width="2000" height="1000" alt="image" src="https://github.com/user-attachments/assets/72a86e5d-b777-401c-856c-a6b0e8eb693a" />

## Project Description

In this project, I intentionally set up both a Windows and Linux virtual machine to be accessible on the internet. They were left in this state for 24 hours to create a honeynet which is an environment meant to attract and analyze potential malicious activities.

This intentional misconfiguration invited attackers from various locations globally to attempt unauthorized access, allowing me to observe and analyze their methods. This provided insights into the geographical origin of each attack, helping me understand potential threats.

Afterward, I strengthened the security of the environment and re-exposed the virtual machines to the internet. This phase allowed me to compare data and assess the impact of the security measures implemented.

## Attack Map Origins

![2024-01-06 01_19_24-linux-ssh-auth-fail - Microsoft Azure — Mozilla Firefox](https://github.com/paRaade/Global-Threat-Visualization-Azure-Honeynet-Mapping/assets/126734769/768802e4-2803-4d42-b9cc-616cd9fe9040)


![2024-01-06 01_09_16-mssql-auth-fail - Microsoft Azure — Mozilla Firefox](https://github.com/paRaade/Global-Threat-Visualization-Azure-Honeynet-Mapping/assets/126734769/309b126f-d963-4704-a864-1cf18944c3c3)


![2024-01-06 01_15_58-nsg-malicious-allowed-in - Microsoft Azure — Mozilla Firefox](https://github.com/paRaade/Global-Threat-Visualization-Azure-Honeynet-Mapping/assets/126734769/623b668b-bce2-4eb3-b571-f1e982b55efe)


![2024-01-06 01_22_35-windows-rdp-auth-fail - Microsoft Azure — Mozilla Firefox](https://github.com/paRaade/Global-Threat-Visualization-Azure-Honeynet-Mapping/assets/126734769/1c5fec52-3a32-48ad-873e-cf197a1e56c9)


## **Before Securing Environment**

The following is data collected in the insecure environment over the course of 24 hours:

2024-01-05T05:52:03.5049008Z to 2024-01-06T05:52:03.5049008Z
|Metrics| Count |
|--|--|
| Security Events (Windows VMs) |33486  |
|Syslog (Linux VMs) |2715|
| SecurityAlert (Microsoft Defender for Cloud) |3|
| SecurityIncident (Sentinel Incidents) |186|
| NSG Inbound Malicious Flows Allowed |2392|


## **After Securing Environment**

The following is data collected after hardening the environment over the next 24 hours:

2024-01-08T18:37:19.9634111Z to 2024-01-09T18:37:19.9634111Z
|Metrics| Count |
|--|--|
| Security Events (Windows VMs) |11548|
|Syslog (Linux VMs) |0|
| SecurityAlert (Microsoft Defender for Cloud) |0|
| SecurityIncident (Sentinel Incidents) |0|
| NSG Inbound Malicious Flows Allowed |0|









