# CrowdStrike Falcon MCP Server

Detect threats, manage endpoints, investigate incidents, and query telemetry from CrowdStrike Falcon — the #1 endpoint detection and response platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdstrike-falcon)

## Overview
**Category:** fort-knox
**Tools Count:** 8

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


## Installation & Usage

To install and use the **CrowdStrike Falcon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdstrike-falcon](https://vinkius.com/mcp/crowdstrike-falcon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
