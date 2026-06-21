# Tenable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tenable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage Tenable Vulnerability Management scans, inspect cloud assets, and triage CVEs natively via your AI agent.

## Description
Connect your **Tenable** (Tenable.io) environment to any AI agent and bring your enterprise vulnerability management directly into your IDE or chat via natural conversation.

### What you can do

- **Scans & Assessments** — List configured vulnerability scans, retrieve detailed run analytics, and even manually trigger immediate evaluations
- **Asset Intelligence** — Browse your entire host and cloud inventory, retrieving deep telemetry like OS fingerprints, IPs, and tags
- **Vulnerability Triage** — Pinpoint explicit security findings (Workbench) and CVEs affecting specific assets without navigating complex dashboards
- **Topology Oversight** — See how your network spaces overlap and track organizational logical folders
- **Scanner Health** — Check the operational status and plugin health of your internal enterprise scanning fleet

### How it works

1. Subscribe to this server
2. Enter your Tenable Access Key and Secret Key
3. Start investigating your risk exposure rapidly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts** — pull CVE details for a specific compromised server in a matter of seconds
- **DevSecOps Engineers** — manually trigger scans on newly deployed infrastructure zones right from their code editor
- **IT Administrators** — audit scanner health and check if host tags actually match the logical network topologies


## Available Tools
- **get_asset_details**: Retrieves detailed metadata, networking, and risk profile for a specific asset
- **get_asset_vulnerabilities**: Retrieves explicit security findings (Workbench) for a specific asset
- **get_scan_results**: Retrieves runtime analytics and vulnerability summaries for a specific scan
- **launch_scan**: Returns the newly created scan run ID.

Manually triggers an immediate execution of a configured scan
- **list_assets**: Lists host and cloud assets discovered in Tenable.io
- **list_scan_folders**: g. "My Scans", "PCI Quarters").

Lists operational scan folders
- **list_logical_networks**: Lists Tenable logical routing networks
- **list_scans**: Lists vulnerability assessment scans from Tenable.io
- **list_asset_tags**: g. "Critical", "Production", "External").

Lists organizational tags mapped to assets
- **list_scanners**: Lists Nessus scanners managed by Tenable.io


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tenable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the status and schedule of the 'Weekly PCI Scan'."

**🤖 AI Agent:**
> I've queried your configured scans. The 'Weekly PCI Scan' is currently 'enabled' and actively on schedule (UUID: eb92f03f-xxxx). It is mapped to the 'PCI Quarters' logical folder. Last execution was 4 days ago. Do you want me to list its historical results?

---

**👤 You:**
> "Retrieve all extreme vulnerabilities on asset ID 1383da-xxx."

**🤖 AI Agent:**
> I pulled the Workbench findings for asset 1383da-xxx. I found 3 critical severity issues detected via plugin 104743 (Windows OTD exploit) and plugin 51192 (OpenSSL RCE). It seems the host is missing 4 months of standard OS patches. Shall I provide the exact CVE payload?

---

**👤 You:**
> "Launch the scan with ID a981bf93 immediately."

**🤖 AI Agent:**
> Scan a981bf93 has been successfully commanded to start. The job run ID is c2f90a1-xxxxx. It has been pushed to the scanner queues and will evaluate all tied network zones independently. Let me know when you want to retrieve the results.


## ❓ FAQ

**Q: Can my AI agent trigger vulnerability scans directly?**
Yes! You can ask your agent to list all mapped scan profiles. Once you copy the ID for something like 'External Perimeter Quick Scan', you can tell the agent to seamlessly launch that specific scan ID out of standard bounds.

**Q: How easy is it to investigate an alert about a single compromised asset?**
Extremely fast. If an IP triggers an alert downstream, ask your agent to retrieve asset details tracking that IP, obtain its specific Asset ID, and immediately pull vulnerabilities. You will instantly get a markdown table of CVEs missing on the endpoint without complex GUI clicking.

**Q: Can the agent interact with scanner appliances (Nessus)?**
Yes. It can fetch your entire scanner inventory across Tenable.io. This includes the internal Nessus agents linked to the account, their connection status, license states, and underlying software versions so you know if your fleet is healthy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tenable](https://vinkius.com/mcp/tenable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tenable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tenable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tenable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tenable": {
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
