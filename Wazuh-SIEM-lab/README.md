# Wazuh SIEM Lab: Windows Agent + Ubuntu Manager

This lab demonstrates deploying a Wazuh SIEM manager on Ubuntu, installing a Windows endpoint agent, and validating log ingestion by generating authentication failures. The goal is to show the full pipeline: endpoint event → agent → manager → alert.

## Architecture

- **Host Machine:** Windows 11  
- **Virtualization:** VMware Workstation  
- **SIEM Manager:** Ubuntu VM running Wazuh Manager  
- **Endpoint:** Windows host running Wazuh Agent  
- **Network:** NAT (VMware)

Windows Agent → Wazuh Manager → Wazuh Dashboard

## Environment Setup

1. Installed Ubuntu 24.04 on VMware and configured networking.
2. Installed Wazuh Manager using the official quickstart script.
3. Added a new Windows agent in the Wazuh Manager console.
4. Installed the Wazuh Windows agent and inserted the agent key.
5. Verified agent connectivity in the Wazuh dashboard.

## Agent Registration

### Windows Agent Connected
These screenshot showcase the process for Windows endpoint successfully registering and being active in the Wazuh dashboard.

![Agent Added](Agent-added.png)
![Agent Key](agent-key.png)
![Wazuh Agent](wazuh-agent.png)
![Wazuh Dashboard](wazuh-dashboard-overview.png)

