📝 Mini SOC Lab – Notes

📌 Project Overview

This SOC lab is a small-scale virtual environment designed to simulate real-world Security Operations Center (SOC) activities. It focuses on log monitoring, threat detection, vulnerability scanning, and incident response in a controlled setup.

The lab follows industry frameworks such as:

NIST SP 800-61 (Incident Response Lifecycle)
MITRE ATT&CK Framework (Threat Mapping)

🏗️ Lab Architecture

The environment includes:

Attacker System: Kali Linux, Metasploitable2 (used for scanning and exploitation)
Target Systems: Windows VM, Ubuntu Linux (with logging enabled)
SIEM Tools: Elastic SIEM (ELK Stack), IBM QRadar (for log analysis and alerts)

🛠️ Tools Used
Elastic SIEM (Kibana): Log monitoring, visualization, alerting
IBM QRadar: Event correlation and security monitoring
Snort: Network intrusion detection system
Nessus Essentials: Vulnerability scanning
Wireshark: Packet analysis
Osquery: Endpoint monitoring
🛡️ Attack Scenarios Practiced

1. Brute Force Attack Detection
Simulated repeated failed login attempts on Windows system
Captured Event ID 4625 (Failed Login Attempts)
Logs analyzed in SIEM for detection
Mapped to MITRE ATT&CK: T1110 (Brute Force)
Response: Source IP blocked and system access restricted

2. Network Intrusion Detection (Snort)
Configured Snort rules to detect suspicious HTTP traffic
Example rule used:
alert tcp any any -> any 80 (msg:"Malicious Domain Access Detected"; content:"malicious.com"; http_uri; sid:1000001;)

🔍 Skills Gained
SIEM monitoring and alert analysis
Incident detection and response
Threat intelligence mapping (MITRE ATT&CK)
Network traffic analysis
Vulnerability assessment
Log correlation and investigation
🧠 Frameworks Applied
MITRE ATT&CK
NIST SP 800-61
CVSS Scoring Model
SOC Incident Response Lifecycle

🎯 Objective

To gain hands-on SOC experience by simulating real-world cyber-attacks, detecting them through monitoring tools, and performing structured incident response.

⚠️ Disclaimer

This lab is strictly for educational and training purposes only. All activities are performed in isolated virtual environments.
