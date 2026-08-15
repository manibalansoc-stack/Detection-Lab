# Enterprise SOC Detection & Threat Hunting Lab

## Overview
Designed and implemented a cloud-based Security Operations Center (SOC) lab using Microsoft Azure, Microsoft Sentinel, Microsoft Defender XDR, and Kusto Query Language (KQL). The lab was built to simulate real-world cybersecurity monitoring and incident response activities by collecting Windows security logs, detecting failed authentication attempts, generating security alerts, and investigating incidents through SIEM and XDR platforms.

The environment included an Azure-hosted Windows 11 virtual machine, Azure networking components, Log Analytics Workspace, Data Collection Rules, Microsoft Sentinel, and Microsoft Defender. Security events generated from the virtual machine were ingested into Sentinel, analyzed using KQL, and converted into actionable alerts and incidents for investigation.

## Objective

The primary objective of this project was to gain hands-on experience in:

- Security Operations Center (SOC) workflows
- Microsoft Sentinel SIEM administration
- Microsoft Defender XDR operations
- Threat hunting using KQL
- Alert triage and incident investigation
- Detection engineering
- Azure cloud security monitoring
- MITRE ATT&CK framework mapping
- Authentication attack detection and analysis

### Technologies Used

#### Cloud Platform
- Microsoft Azure
#### Security Tools
- Microsoft Sentinel
- Microsoft Defender XDR
- Microsoft Defender Portal
#### Monitoring Components
- Log Analytics Workspace
- Azure Monitor
- Azure Workbook
= Data Collection Rules (DCR)
#### Infrastructure
- Azure Virtual Machine (Windows 11)
- Azure Virtual Network (VNet)
- Azure Network Security Group (NSG)
- Azure Public IP
#### Security Framework
- MITRE ATT&CK
#### Query Language
- Kusto Query Language (KQL)


## Steps

### Microsoft Sentinel SIEM Implementation and Security Monitoring Lab

Implemented and configured Microsoft Sentinel as a cloud-native Security Information and Event Management (SIEM) platform for centralized log collection, threat detection, incident monitoring, and security analytics. Connected Azure and Microsoft security data sources, monitored incidents, reviewed security posture metrics, and explored User and Entity Behavior Analytics (UEBA) capabilities.

<img width="959" height="519" alt="SOC 1" src="https://github.com/user-attachments/assets/b0fe97d9-7a35-41f2-a49e-939721f43936" />

Observations from the Dashboard

SOC Optimization

Active Recommendations: 13
Completed Recommendations: 3
In Progress: 0

Data Connectors

Total Connectors: 1
Unhealthy Connectors: 0/1

Active Incidents

Total Active Incidents: 6
Multiple incidents related to Failed Logon Attempts
Severity shown: Low

Microsoft Secure Score

Secure Score: 89.29%
Achieved Points: 50/56



### Azure Network Security Group (NSG) Configuration for SOC Monitoring

Configured and managed Azure Network Security Groups (NSGs) to control inbound and outbound network traffic for a Windows 11 virtual machine deployed in an Azure-based SOC lab. The NSG was used to generate network activity, monitor security events, and support threat detection through Microsoft Sentinel.

<img width="1918" height="915" alt="image" src="https://github.com/user-attachments/assets/3bb641c2-2d61-41da-a9ec-f86f6f9b7209" />

Network Security Group
NSG Name: Itsec01admin-nsg
Resource Group: Virtual-SOC-Lab
Location: Australia East
Custom Security Rules
1 Custom Inbound Rule
0 Custom Outbound Rules
Associated Resources
1 Network Interface
0 Subnets

### Incident Monitoring & Investigation
<img width="1916" height="923" alt="image" src="https://github.com/user-attachments/assets/f3352da7-b64e-4f13-a755-093feaf0bfe8" />


Security Platform
Microsoft Defender Portal
Incident Management Dashboard
Incidents Observed
Total Incidents: 7
Incident Type: 4625 Failed Logon Attempt
Severity: Low
Category: Credential Access
Alert Description

Windows Event ID 4625 indicates:

"An account failed to log on."

### Advanced Threat Hunting Using Microsoft Defender and KQL

Performed proactive threat hunting within Microsoft Defender using Kusto Query Language (KQL) to identify failed authentication attempts against Azure-hosted Windows endpoints. Developed custom hunting queries to investigate Event ID 4625 logs, enrich source IP addresses with geolocation data, and identify suspicious login activity originating from external locations.

<img width="1918" height="911" alt="image" src="https://github.com/user-attachments/assets/906eb1ff-651a-45d1-a9c8-5d1e87993bcb" />


Detection Name

Failed Logon VM Detection

Workspace

vm-logs

Results
232 Events Found
Time Range: Last 30 Days
Target System

Itsec01admin

Authentication Event
4625 - An account failed to log on

Suspicious Source IP
194.165.16.166

### Alert Monitoring and Detection Management

The alerts were generated after a custom KQL detection rule identified repeated failed login attempts against the monitored Azure virtual machine.

<img width="1918" height="906" alt="image" src="https://github.com/user-attachments/assets/ec6a4dc5-3cff-481c-a0a0-36deb63abede" />

### Custom Detection Rule for Failed Logon Attempts

Designed and implemented a custom detection rule within Microsoft Defender XDR to identify Windows Event ID 4625 failed authentication attempts. Configured alerts to detect credential access techniques, mapped detections to the MITRE ATT&CK framework, and generated actionable alerts for incident investigation and SOC monitoring activities.

<img width="1918" height="918" alt="image" src="https://github.com/user-attachments/assets/fd552e70-1403-4640-93df-2b639bef8e80" />

### Azure Resource Group Architecture

the Virtual-SOC-Lab Resource Group, which contains all cloud resources required to build and operate the Microsoft Sentinel SOC environment.

The resource group serves as the centralized container for Azure infrastructure, security monitoring, log collection, networking, and threat detection components.

<img width="1914" height="921" alt="image" src="https://github.com/user-attachments/assets/870f7022-6f70-4dd4-b40e-d5ab320dff09" />

