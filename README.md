# Azure Sentinel Honeypot – Live Cyber Attack Visualization

## Table of Contents
- [Project Overview](#overview)
- [Objectives](#objectives)
- [Skills Demonstrated](#skills-demonstrated)
- [Technologies Used](#technologies-used)
- [Screenshots & Documentation](#screenshots--documentation)
- [Future Enhancements](#future-enhancements)
- [Step 1: Setup](setup.md)
- [Step 2: Analyzing Security Logs in Event Viewer](logs_analysis.md)
- [Step 3: Geolocation Visualization in Microsoft Sentinel](geolocation_visualization.md)

---

## Overview
This project sets up a **vulnerable virtual machine (VM) in Microsoft Azure** as a honeypot to attract and log unauthorized **Remote Desktop Protocol (RDP) attacks**. Using **Azure Sentinel**, the project:

- Captures and analyzes **failed RDP login attempts**  
- Extracts **attacker IP addresses** from security logs  
- Retrieves **geolocation data** for each attacker using an API  
- **Visualizes attacks on a world map** in Azure Sentinel

### Project Architecture
The following diagram illustrates the high-level architecture of the honeypot setup:

![Azure Sentinel Honeypot Architecture](screenshots/readme1.png) 

## Objectives
- **Deploy Azure Resources**: Set up and configure essential Azure components, including Virtual Machines (VMs), Log Analytics Workspaces, and Azure Sentinel, to create a functional honeypot environment.
- **Implement a Honeypot**: Establish a decoy system designed to attract and monitor malicious activity, providing valuable insights into potential threats and attackers' tactics.
- **Integrate SIEM Solutions**: Utilize Azure Sentinel as a Security Information and Event Management (SIEM) tool to collect, analyze, and respond to security events in real-time.
- **Data Visualization**: Create interactive dashboards and visualizations, such as world maps, to display attack data and statistics effectively.

## Skills Demonstrated

- **Azure Resource Management**: Proficiently manage and deploy Azure services, including Virtual Machines, Log Analytics Workspaces, and Sentinel.
- **Security Monitoring**: Implement and monitor honeypot systems to detect and analyze unauthorized access attempts and potential security threats.
- **Log Analysis with KQL**: Utilize Kusto Query Language (KQL) to query and analyze logs within Azure Sentinel, extracting meaningful insights from collected data.
- **API Integration**: Integrate third-party APIs, such as ipgeolocation.io, to enrich log data with geolocation information, enhancing the context of security events.
- **PowerShell Scripting**: Develop and execute PowerShell scripts to automate tasks, such as exporting Windows Event Viewer logs and processing data for analysis.
- **Data Visualization**: Design and implement interactive workbooks and dashboards in Azure Sentinel to visualize attack data, including geolocation mapping of malicious IP addresses.


## Technologies Used
- **Microsoft Azure** – Cloud platform for VM deployment and monitoring  
- **Azure Sentinel** – SIEM (Security Information and Event Management) for threat detection  
- **PowerShell** – Scripting for log extraction and automation  
- **Log Analytics Workspace** – Centralized data collection for analysis  
- **ipgeolocation.io API** – Service for geolocation lookup based on IP addresses  

## Screenshots & Documentation
As you follow along, refer to the **setup.md** and other documentation files for screenshots and configuration steps. These will include:
- **VM creation and network configuration** in Azure.  
- **Firewall settings and Log Analytics configuration**.  
- **PowerShell script execution and log extraction results**.  
- **Azure Sentinel attack visualization on a world map**.  

## Future Enhancements
Potential improvements include:
- **Automated attack detection and alerts** using Azure Sentinel rules.
- **Extending the honeypot** to monitor additional attack vectors.
- **Integrating a dashboard** for real-time attack visualization.

## Disclaimer
This project is for **educational and research purposes only**. Deploying honeypots can attract real-world attacks, so ensure that your cloud security measures are in place.

---

[🔝 Back to Table of Contents](#table-of-contents)

[Step 1: Setup](setup.md)