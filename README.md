# Home SOC Lab with Wazuh SIEM

## Overview
This project documents the creation of a Home Security Operations Center (SOC) Lab using Wazuh SIEM, VirtualBox, Ubuntu, and Kali Linux.

The purpose of this lab was to gain hands-on experience with security monitoring, log collection, attack detection, and SIEM operations in a controlled environment.

---

## Lab Environment
The lab consists of three virtual machines:

- **Wazuh Server** (Manager, Indexer, and Dashboard)
- **Ubuntu Target Machine** (with Wazuh Agent installed)
- **Kali Linux Attacker Machine**

All systems were connected through an isolated VirtualBox NAT Network.

---

## Tools & Technologies

| Tool         | Purpose                                  |
|--------------|------------------------------------------|
| Wazuh SIEM   | Security monitoring and threat detection |
| VirtualBox   | Virtualization platform                  |
| Ubuntu 22.04 | Target endpoint                          |
| Kali Linux   | Attack simulation                        |
| Nmap         | Network reconnaissance                   |

---

## Key Activities

### 1. Wazuh Deployment
- Installed and configured the Wazuh server (Manager, Indexer, Dashboard)
- Verified all services were operational
- Deployed Wazuh Agent on Ubuntu endpoint for log collection and monitoring

### 2. Attack Simulation & Detection
- Performed network reconnaissance using Nmap from Kali Linux against Ubuntu target
- Monitored and analyzed generated security events in Wazuh Dashboard
- Successfully detected and logged all attack activities

### 3. Custom Detection Rules
- Created custom detection rules in `rules.xml`
- Enhanced threat detection capabilities with custom rule logic
- Verified rule effectiveness through attack simulation

---

## Technical Insights

**Memory Optimization:**
The original guide allocated 4 GB RAM to the Wazuh server. Due to deploying a newer Wazuh version, I increased the server memory to 6 GB for improved stability and performance.

---

## Skills Developed

- SIEM deployment and configuration
- Security monitoring and log analysis
- Threat detection and incident response
- Custom rule creation and management
- Linux administration
- Virtualization and network segmentation
- Cloud security operations

---

## About the Author

**Obaidur Rahman**  
Diploma in Computer Engineering  
Jamia Millia Islamia (JMI), New Delhi