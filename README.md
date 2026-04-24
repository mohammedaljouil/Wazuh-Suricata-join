# Wazuh-Suricata-Integration
A centralized security monitoring solution designed to provide real-time network intrusion detection (IDS) and security analytics for Windows Server 2022 environments. This project integrates Suricata for deep packet inspection and network traffic analysis with Wazuh (SIEM/XDR) for log aggregation and incident response.

About the Project
This project was developed to address the challenge of monitoring network activity on Windows Server 2022. By leveraging Suricata's powerful rule-based engine to detect potential threats and piping those alerts directly into the Wazuh manager, this solution provides a unified dashboard for security teams to visualize alerts, correlate logs, and respond to threats efficiently.

Core Objectives:

-Network Visibility: Gain granular insights into traffic flowing through the Windows Server.
-Centralized Alerting: Aggregate network intrusion alerts alongside system and security event logs.
-Threat Response: Enable rapid identification of malicious traffic patterns using customizable Suricata rulesets.

Architecture

The data flow follows this sequence:
Traffic Capture: Suricata monitors the network interface on the Windows Server.
Alert Generation: Suricata identifies malicious activity and logs it in JSON format.
Log Forwarding: The Wazuh agent (running on the Windows Server) collects these logs.
Correlation & Visualization: The Wazuh Manager processes the logs, triggers alerts, and displays them on the dashboard.

Key Features

-Real-time Detection: Immediate response to potential network intrusions.
-Unified Dashboard: Aggregated view of both system-level logs and network-level alerts.
-Scalable Architecture: Designed for easy integration with additional agents or network segments.
-Customizable Rules: Fully adaptable Suricata rules to match specific environment requirements.

Technologies Used

IDS/IPS:  https://suricata.io/download/
SIEM/XDR: https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html
OS: Windows Server 2022
Data Format: JSON / Event Logs

Author
©Mohammed Mahdi Aljouil ,Cybersecurity Student | Project Developer
