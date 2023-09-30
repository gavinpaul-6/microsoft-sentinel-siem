![sentinel_poster](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/b3b9ba05-14c0-4e11-97c9-30f3dc7a0e31)
# Microsoft Sentinel SIEM & Honeynet

<h2>Summary</h2>
SIEM stands for Security Information and Event Management System. It is a solution that helps organizations detect, analyze, and respond to security threats before they harm business operations. It is a tool that collects event log data from a range of sources within a network such as Firewalls, IDS/IPS, Identity solutions, etc. This allows the security professionals to monitor, prioritize and remediate potential threats in real-time. A honeypot is a security mechanism that creates a virtual trap in a controlled and safe environment to lure attackers. An intentionally compromised computer system to study how attackers work, examine different types of threats and improve security policies. This lab's purpose is to understand how to collect honeypot attack log data, query it in a SIEM and display it in a manner that is easy to understand such data. In this case it will be displayed in a world map by event count and geolocation.

<h2>Diagram</h2>

![microsoft-sentinel-diagram](https://github.com/gavinpaul-6/microsoft-sentinel-siem/assets/98987388/025762ef-314b-436d-9e58-007633086084)

<h2>Resources Used</h2>

- Microsoft Azure Subscription
- Microsoft Sentinel
- Microsoft Defender for Cloud
- Kusto Query Language (KQL - Used to build world map)
- Network Security Groups (Layer 4/3 Firewall in Azure)
- Remote Desktop Protocol (RDP)
- 3rd Party API: [ipgeolocation.io](https://ipgeolocation.io/)
