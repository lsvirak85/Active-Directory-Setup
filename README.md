# **Active Directory Home Lab**

## **Project Description**  
The **Active Directory Home Lab** is a cybersecurity-focused environment designed to simulate a real-world enterprise network. The project leverages **Active Directory (AD), Splunk, and Sysmon** to enable log collection, analysis, and security monitoring. This lab serves as a learning and testing ground for **identity access management, network security, and log analysis** using open-source and enterprise tools.

---

## **Key Features**  

- **Active Directory Implementation:**  
  - Configured **Windows Server 2022** with **Active Directory Domain Services (AD DS)** for user authentication and group policy management.  

- **Virtualized Environment Setup:**  
  - Deployed **Windows 10, Ubuntu Server, and Kali Linux** in VirtualBox to simulate enterprise infrastructure.  
  - Configured **NAT networking** to enable inter-machine communication.  

- **Security & Log Monitoring:**  
  - Installed **Splunk Enterprise** to collect and analyze system logs.  
  - Configured **Splunk Universal Forwarder** for real-time log forwarding from endpoint devices.  
  - Deployed **Sysmon** for enhanced security event logging on Windows endpoints.  

- **Network Configuration & Troubleshooting:**  
  - Set up **static IP addressing** to maintain a structured network environment.  
  - Verified connectivity using **ping, IP configuration, and Splunk search queries**.  

- **Automated Log Collection & Forwarding:**  
  - Developed an **inputs.conf** configuration to filter and forward logs related to **system security, applications, and Sysmon** events to Splunk.  
  - Enabled **Splunk auto-start** upon VM reboot for continuous monitoring.  

- **Log Analysis & Querying:**  
  - Used **Splunk Search Processing Language (SPL)** to create custom queries for analyzing security logs and identifying anomalies.  

- **Project Documentation & Learning Resource:**  
  - Documented **installation steps, configurations, and troubleshooting** for future reference and learning.  
  - Explored additional security tools like **Atomic Red Team** for testing security monitoring capabilities.  

---

## **Technical Specifications**  

- **Operating Systems:** Windows Server 2022, Windows 10, Ubuntu Server 22.04, Kali Linux  
- **Virtualization Platform:** VirtualBox  
- **Networking:** NAT Network (192.168.10.0/24) with static IP addressing  
- **Security Tools:**  
  - **Splunk Enterprise & Universal Forwarder** (log collection & analysis)  
  - **Sysmon** (enhanced Windows event logging)  
  - **Active Directory Domain Services (AD DS)** (user authentication & security policies)  
- **Programming/Querying Languages:** Splunk Search Processing Language (SPL), PowerShell (for configurations)  
- **Deployment Environment:** Local Virtual Machines (VMs)  

---

## **Development Roadmap**  

### **Phase 1: Virtual Machine Setup & AD Configuration**  
- **Milestone 1:** Install VirtualBox and set up NAT networking.  
- **Milestone 2:** Deploy **Windows Server 2022, Windows 10, Ubuntu Server, and Kali Linux** VMs.  
- **Milestone 3:** Configure **Active Directory Domain Services (AD DS)** and domain authentication.  

### **Phase 2: Security Monitoring & Log Collection**  
- **Milestone 4:** Install and configure **Splunk Enterprise** for log ingestion.  
- **Milestone 5:** Deploy **Splunk Universal Forwarder** on Windows machines to send logs.  
- **Milestone 6:** Install and configure **Sysmon** for advanced event logging.  

### **Phase 3: Log Analysis & Automation**  
- **Milestone 7:** Develop **custom queries in Splunk SPL** to detect suspicious activities.  
- **Milestone 8:** Automate **Splunk startup and log forwarding** processes.  
- **Milestone 9:** Test network security with **Atomic Red Team** simulations.  

### **Phase 4: Enhancements & Documentation**  
- **Milestone 10:** Document step-by-step installation and configurations.  
- **Milestone 11:** Explore additional security tools such as **EDR solutions, IDS, and firewalls**.  
- **Milestone 12:** Troubleshoot and optimize network and log collection settings.  

---

## **Important Considerations**  

- **Network Configuration & IP Management:**  
  - Ensuring each VM is assigned the correct **static IP** and connected to the **correct NAT network** to prevent conflicts.  

- **Splunk Indexing & Performance:**  
  - Logs must be properly categorized in **inputs.conf** and assigned to the **correct Splunk index** (e.g., "endpoint") to avoid data loss.  

- **Security Best Practices:**  
  - While this is a **lab environment**, similar setups in production should follow **least privilege principles**, **secure authentication methods**, and **log encryption**.  

- **Troubleshooting & Debugging:**  
  - Regularly check **Splunk logs, system event viewer, and network connectivity** for misconfigurations.  
  - Use **Splunk’s search and reporting tools** to validate data ingestion.  

---

## **Resources & Documentation**  

- **Splunk Enterprise Download:** [Splunk Official Website](https://www.splunk.com)  
- **Sysmon Configuration:** [Sysmon GitHub Repository](https://github.com/SwiftOnSecurity/sysmon-config)  
- **VirtualBox Installation:** [VirtualBox Official Website](https://www.virtualbox.org)  
- **Active Directory Fundamentals:** [Microsoft Learn - AD DS](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/)  
- **Networking Basics:** [Subnetting & IP Addressing](https://www.cisco.com/c/en/us/td/docs/switches/lan/catalyst2960/software/release/15-0_2_se/configuration/guide/scg_2960/subnet.pdf)  

---

### **Next Steps**  
- 🛠️ Setting up **Intrusion Detection Systems (IDS) and Endpoint Detection & Response (EDR)** solutions.  
- 📊 Developing **Splunk dashboards** for real-time security event monitoring.  
- 🔍 Exploring **threat hunting techniques** using logs collected in the lab.  
