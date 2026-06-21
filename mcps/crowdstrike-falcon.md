# CrowdStrike Falcon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdstrike-falcon)
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


## Available Tools (8)
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


## ❓ FAQ

**Q: What authentication does CrowdStrike use?**
CrowdStrike uses OAuth 2.0 Client Credentials. You create an API Client in the Falcon Console under Support > API Clients and Keys. The server automatically obtains and caches Bearer tokens using your Client ID and Secret.

**Q: Which cloud regions are supported?**
All CrowdStrike commercial clouds: US-1 (api.crowdstrike.com), US-2 (api.us-2.crowdstrike.com), EU-1 (api.eu-1.crowdstrike.com), and US-GOV-1. Configure the Base URL credential to match your tenant region.

**Q: Can it triage detections automatically?**
Yes. The list_detections tool returns severity, tactic, technique, and device context. An AI agent can use this to auto-triage low/medium detections and escalate critical ones, reducing SOC analyst workload by 60-80%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdstrike-falcon](https://vinkius.com/mcp/crowdstrike-falcon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrowdStrike Falcon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crowdstrike-falcon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrowdStrike Falcon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crowdstrike-falcon": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
