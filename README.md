# 🛡️SOC Home Lab🛡️
HomeLab Setup with a Firewall, SIEM Solution, Exploitable machines and an Attacker.
The lab comprises 4 virtual machines running on VirtualBox, each configured to perform a distinct role within the security operations workflow. <br>

💻Hardware:<br>
Xeon E5-1620<br>
Logical Processors 	8<br>
Memory	40 GB DDR4<br>
Storage Space	2x 250 gb SSD

# Configuration
pfSense(Firewall/Router/VPN)<br>
Ubuntu(Monitoring, Logging, Compliance, Wazuh)<br>
Windows(User workstation simulation)<br>
Kali(Adversary simulation)

- <a href="https://www.pfsense.org/"><img src="https://img.shields.io/badge/pfSense-394B5A?logo=pfsense&logoColor=white" /></a> Router (**192.168.1.1**): Serves as the network gateway, routing traffic from the WAN port into VirtualBox’s internal network. It runs a firewall and IDS/IPS powered by Snort, and supports VPN management
- <a href="https://ubuntu.com/"><img src="https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white" /></a> Server (**192.168.1.25**): Runs Wazuh SIEM/XDR for centralized security operations management, serving as the primary system overseeing the Security Operations Center (SoC)
- <a href="https://www.microsoft.com/en-us/software-download/windows11"><img src="https://img.shields.io/badge/Windows%2011-0078D6?logo=windows&logoColor=white" /></a> Machine (**192.168.1.11**): Simulates an endpoint device, runs malware detection tools, and forwards security events to the SIEM for analysis.
- <a href="https://www.kali.org/"><img src="https://img.shields.io/badge/Kali_Linux-557C94?logo=linux&logoColor=white&style=for-the-badge" /></a> Machine (**192.168.1.8**): Adversary simulation system used to execute attack campaigns and evaluate detection capabilities.


🚨🔧🖥️🔌🌐💡📦🤖🖥️🧱🔍🎯
