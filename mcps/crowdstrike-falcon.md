# CrowdStrike Falcon MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdstrike-falcon)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crowdstrike-falcon-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crowdstrike-falcon-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Detect threats, manage endpoints, investigate incidents, and query telemetry from CrowdStrike Falcon — the #1 endpoint detection and response platform.

## Description
Connect your **CrowdStrike Falcon** tenant to any AI agent and operate security at machine speed through natural conversation.

### What you can do

- **Detections** — Query, triage, and update detection alerts across your fleet
- **Hosts** — Search and inspect endpoint details, OS info, and sensor versions
- **Incidents** — List, investigate, and manage security incidents
- **IOCs** — Create, list, and manage Indicators of Compromise
- **Real-Time Response** — Query active sessions and retrieve device status
- **Vulnerabilities** — Spotlight vulnerability data across managed endpoints

### Who is this for?

- **SOC Analysts** — triage detections and incidents 10x faster through chat
- **Security Engineers** — automate IOC management and threat hunting
- **CISOs** — get real-time fleet health and threat posture summaries
- **IT Operations** — monitor endpoint compliance and sensor coverage


## Available Tools
- **list_detections**: Use FQL filter syntax for precision: severity, technique, hostname, etc. Returns detection details with MITRE ATT&CK mapping.

Query detection alerts
- **update_detection**: Optionally add a triage comment.

Update detection status
- **search_hosts**: Returns full device inventory details.

Search endpoints
- **list_incidents**: Filter by state, severity, assigned_to, or date range using FQL syntax.

Query security incidents
- **list_iocs**: Includes type, value, action, and metadata.

List custom IOCs
- **create_ioc**: Types: sha256, md5, domain, ipv4, ipv6. 

Create a custom IOC indicator.. Actions: default
- **list_vulnerabilities**: Filter by CVE, severity, host, or remediation status.

Query Spotlight vulnerabilities
- **contain_device**: Contain or lift containment on a device.. Actions: default


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrowdStrike Falcon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all critical detections from the last 24 hours."

**🤖 AI Agent:**
> Found 3 critical detections in the last 24h: 1. 'CobaltStrike Beacon' on WIN-SERVER-05 (Critical, T1059.001 PowerShell). 2. 'Credential Dumping - LSASS' on DC-PROD-01 (Critical, T1003.001). 3. 'Lateral Movement - PsExec' on WS-FIN-12 (Critical, T1021.002). Recommend immediate containment of DC-PROD-01.

---

**👤 You:**
> "How many endpoints are running outdated sensors?"

**🤖 AI Agent:**
> Fleet Health: 2,847 total endpoints. 2,691 (94.5%) on latest sensor v7.18. 127 (4.5%) on v7.16 (1 version behind). 29 (1.0%) on v7.14 or older - URGENT update needed. Top affected: Finance dept (12), Remote workers (9), Lab servers (8).

---

**👤 You:**
> "List all IOCs related to ransomware campaigns added this month."

**🤖 AI Agent:**
> 18 ransomware IOCs added this month: 8 SHA256 hashes (LockBit 3.0 variants), 5 domains (C2 infrastructure), 3 IPs (data exfiltration endpoints), 2 mutex names. Sources: CrowdStrike Intelligence (12), Custom (6). All set to 'Detect' action.


## Installation & Usage

To install and use the **CrowdStrike Falcon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdstrike-falcon](https://vinkius.com/mcp/crowdstrike-falcon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
