# Tool Introduction
Suricata is an open-source, high-performance network threat detection engine developed by the Open Information Security Foundation (OISF). It is designed to provide deep visibility into network traffic and to detect, prevent, and respond to modern cyber threats in real time.  <br><br>

Unlike traditional Intrusion Detection Systems (IDS), Suricata goes beyond simple pattern matching by combining IDS, IPS (Intrusion Prevention System), and Network Security Monitoring (NSM) capabilities into a single, versatile tool. With its powerful multi-threaded architecture, Suricata can analyze traffic at gigabit speeds, making it suitable for enterprise and high-traffic environments.  <br><br>

✨ Key Features
  * **Intrusion Detection & Prevention (IDS/IPS)**: Detects malicious activity using signature-based and anomaly-based methods, and can actively block threats when deployed in IPS mode.
  * **Deep Packet Inspection (DPI)**: Provides detailed insights by parsing application-layer protocols such as HTTP, TLS, DNS, FTP, and SMB.
  * **File Extraction & Logging**: Identifies and extracts files from network streams for further analysis, and supports JSON logging for SIEM/SOC integration.
  * **Threat Intelligence Integration**: Supports rule sets like Emerging Threats (ET) and custom signatures for tailored detection.
  * **Scalability**: Multi-threaded performance ensures high throughput on modern multi-core systems.
  * **Versatility**: Works as an IDS, IPS, or as a packet capture tool for traffic analysis.
<br>

🚀 Use Cases
  * Monitoring and analyzing suspicious network traffic.
  * Blocking intrusions at the gateway in IPS mode.
  * Collecting logs for SIEM integration (e.g., Wazuh, ELK, Splunk).
  * Forensics and incident response through packet capture and file extraction.
  * Research and lab environments to study malicious traffic behavior.

# Lab Description
This lab is designed to demonstrate the installation, configuration, and usage of Suricata as a network threat detection tool. The goal is to provide hands-on experience with deploying Suricata in a controlled environment and exploring its capabilities for Intrusion Detection, Intrusion Prevention, and Network Security Monitoring (NSM).

This lab focuses on installing and configuring Suricata, an open-source network threat detection engine, in a controlled environment. Students will deploy Suricata in IDS mode, apply community rule sets, and generate test traffic to observe alerts. The exercise provides hands-on experience with monitoring network traffic, analyzing Suricata logs, and understanding how IDS tools support real-world security operations.

# Prerequisites
1. Ubuntu Machine
2. Access to Internet

# Initial Setup
```
sudo apt update -y
```
```
sudo apt upgrade -y
```
```
sudo apt install build-essential curl dkms dnsutils tree vim vim-gtk3 -y
```
# Step 1
To begin installing Suricata, first add the Open Information Security Foundation (OISF) software repository to your Ubuntu system.
```
sudo add-apt-repository ppa:oisf/suricata-stable
```

![](1.png)
As shown in Figure 1, press **ENTER** when prompted to confirm the addition of the repository. After the repository is added, the system automatically updates the list of available packages.
