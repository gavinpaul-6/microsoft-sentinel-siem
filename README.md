![sentinel_poster](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/b3b9ba05-14c0-4e11-97c9-30f3dc7a0e31)
# Microsoft Sentinel SIEM & Honeynet

<h2>Summary</h2>
SIEM stands for Security Information and Event Management System. It is a solution that helps organizations detect, analyze, and respond to security threats before they harm business operations. It is a tool that collects event log data from a range of sources within a network such as Firewalls, IDS/IPS, Identity solutions, etc. This allows the security professionals to monitor, prioritize and remediate potential threats in real-time. A honeypot is a security mechanism that creates a virtual trap in a controlled and safe environment to lure attackers. An intentionally compromised computer system to study how attackers work, examine different types of threats and improve security policies. This lab's purpose is to understand how to collect honeypot attack log data, query it in a SIEM and display it in a manner that is easy to understand such data. In this case it will be displayed in a world map by event count and geolocation.

<h2>Diagram</h2>

![microsoft-sentinel-diagram](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/025762ef-314b-436d-9e58-007633086084)

<h2>Resources Used</h2>

- Virtual Network (VNet)
- Network Security Group (NSG)
- Virtual Machines (2 Windows host, 1 Linux host)
- Log Analytics Workspace
- Azure Key Vault
- Azure Storage Account
- Microsoft Sentinel

<h2>Attack Maps Before Hardening / Security Controls</h2>

![linux-ssh-auth-fail](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/48397af4-b2d2-44e9-9562-5b895592504f)

![windows-rdp-auth-fail](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/4d59440f-def0-4d5d-9700-2146d69a9777)

![nsg-malicious-allowed-in](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/ea55175c-bcc4-4fcb-8227-d36322d6974c)

![mssql-auth-fail](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/fb3752e5-d133-4d15-941e-b49d4717c158)

<h2>Metrics Before Hardening / Security Controls</h2>


| Metric  | Count |
| ------------- | ------------- |
| Security Event  | 10102  |
| Syslog  | 3486  |
| SecurityAlert  | 8  |
| SecurityIncident  | 173  |
| AzureNetworkAnalytics_CL  | 1628  |

<h2>Metrics After Hardening / Security Controls</h2>


| Metric  | Count |
| ------------- | ------------- |
| Security Event  | 7370  |
| Syslog  | 24  |
| SecurityAlert  | 0  |
| SecurityIncident  | 0  |
| AzureNetworkAnalytics_CL  | 0  |

<h2>Conclusion</h2>

In this project, a miniature honeynet was established within Microsoft Azure, and various log sources were seamlessly incorporated into a Log Analytics workspace. Microsoft Sentinel was deployed to initiate alerts and generate incidents based on the assimilated logs. Furthermore, we gauged metrics within the vulnerable environment before and after the implementation of security measures. Significantly, the deployment of these security controls resulted in a substantial reduction in the number of security events and incidents, underscoring their efficacy.

It's important to note that had the network's resources been heavily utilized by regular users, it's plausible that a higher volume of security events and alerts might have been generated in the 24 hours following the deployment of these security controls.



