# Home SOC Lab -- Detection & Monitoring Environment

## Overview

This project documents the design and implementation of a **Home
Security Operations Center (SOC) Lab** used to simulate enterprise
security monitoring, threat detection, and incident response workflows.

The lab replicates a small enterprise network using virtual machines and
security tools to generate, monitor, and analyze malicious activity. It
provides hands-on experience with **SIEM platforms, IDS monitoring,
Active Directory environments, and attacker simulation**.

The goal of the lab is to practice real-world SOC operations such as log
collection, alert triage, threat detection, and incident investigation
in a controlled environment.

------------------------------------------------------------------------

## Architecture

The environment is built using **VMware virtualization** and multiple
virtual machines representing attackers, victims, and monitoring
infrastructure.

Core components in the lab include:

-   **pfSense** -- Firewall and network segmentation\
-   **Security Onion** -- IDS, network monitoring, and log analysis\
-   **Splunk Enterprise** -- SIEM platform for centralized log
    collection and analysis\
-   **Kali Linux** -- Attacker machine used to simulate cyber attacks\
-   **Windows Server 2019** -- Active Directory Domain Controller\
-   **Windows 10 Clients** -- Domain-joined victim machines\
-   **Ubuntu Server** -- Splunk SIEM server\
-   **Ubuntu Desktop** -- SOC analyst workstation

This architecture simulates a **corporate network with centralized
monitoring and security detection tools**.

------------------------------------------------------------------------

## Network Design

The network is segmented using **pfSense firewall rules** and multiple
virtual networks.

Traffic from victim machines flows through the firewall and is monitored
by Security Onion. Logs and security events are forwarded to Splunk for
centralized analysis and investigation.

Example workflow:

1.  Attack simulation is performed from Kali Linux.
2.  Network traffic flows through pfSense firewall.
3.  Security Onion captures packets and analyzes network activity.
4.  Alerts are generated using IDS tools such as Suricata and Zeek.
5.  Logs are forwarded to Splunk SIEM.
6.  SOC analysts investigate alerts and correlate events.

------------------------------------------------------------------------

## Technologies Used

### Virtualization

-   VMware Workstation

### Security Monitoring

-   Security Onion
-   Suricata IDS
-   Zeek Network Monitor

### SIEM

-   Splunk Enterprise
-   Splunk Universal Forwarder

### Operating Systems

-   Kali Linux
-   Windows Server 2019
-   Windows 10
-   Ubuntu Server
-   Ubuntu Desktop

### Network Security

-   pfSense Firewall
-   Network segmentation and monitoring

------------------------------------------------------------------------

## Key Capabilities

This lab enables experimentation with several SOC and detection
engineering workflows including:

-   Network intrusion detection
-   Log aggregation and correlation
-   Security event monitoring
-   Incident investigation
-   Threat hunting
-   Attack simulation and detection validation

Example detection scenarios include:

-   Port scanning detection
-   Suspicious login monitoring
-   Lateral movement detection
-   Malicious network activity analysis

------------------------------------------------------------------------

## Skills Demonstrated

This project demonstrates practical experience in:

-   Security Operations Center (SOC) workflows
-   SIEM configuration and log analysis
-   IDS monitoring and alert investigation
-   Network security architecture
-   Active Directory environments
-   Threat detection and incident response

------------------------------------------------------------------------

## Future Improvements

Planned improvements for this lab include:

-   SOAR automation for incident response
-   MITRE ATT&CK detection mapping
-   Threat intelligence integration
-   Endpoint monitoring with Sysmon
-   Automated attack simulations
