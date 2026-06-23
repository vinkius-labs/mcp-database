# Halo Security MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/halo-security)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Automate attack surface management via Halo Security — monitor assets, scans, and vulnerabilities directly from any AI agent.

## Description
Connect your **Halo Security** platform to any AI agent and take full control of your attack surface and vulnerability management through natural conversation.

### What you can do

- **Asset Monitoring** — List and add targets (domains, IPs, apps) to your security perimeter.
- **Vulnerability Oversight** — Access and inspect discovered security issues, severities, and remediation status.
- **Scan Management** — Review scan history and trigger new on-demand security assessments.
- **Infrastructure Discovery** — List open ports, SSL/TLS certificates, and detected technologies across your assets.
- **Security Trends** — Retrieve risk scores and security trends to monitor your posture over time.
- **DNS Insights** — Access DNS records discovered during the reconnaissance phase.

### How it works

1. Subscribe to this server
2. Enter your Halo Security API Key
3. Start managing your security posture from Claude, Cursor, or any MCP-compatible client

No more manual exporting of vulnerability reports. Your AI assistant acts as a dedicated Security Analyst or AppSec Specialist.

### Who is this for?

- **Security Engineers** — instantly retrieve asset lists and vulnerability details during triage.
- **DevSecOps Teams** — automate the triggering of scans and monitoring of security issues in real-time.
- **CISOs** — maintain a high-level overview of the organization's attack surface and risk scores.


## Available Tools (11)
- **add_target**: Add a new target for security monitoring
- **get_issue**: Get detailed information about a specific security issue
- **get_security_risk**: Get overall security risk scores and trends
- **list_certificates**: List SSL/TLS certificates and their status
- **list_dns_records**: List DNS records discovered for monitored targets
- **list_issues**: List all discovered security issues and vulnerabilities
- **list_open_ports**: List all discovered open ports across targets
- **list_scans**: List history of security scans
- **list_targets**: List all monitored targets (assets)
- **list_technologies**: List detected technologies and libraries on targets
- **trigger_scan**: Trigger a new security scan for a target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Halo Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all security issues with 'High' severity."

**🤖 AI Agent:**
> I've retrieved your issues. You currently have 3 High severity findings: 'Outdated jQuery Library' on example.com, 'Missing Security Headers', and 'SSL Certificate Expiring Soon'. Would you like the details for the SSL issue?

---

**👤 You:**
> "Trigger a security scan for target ID 5592."

**🤖 AI Agent:**
> Scan triggered! I've successfully requested a new security assessment for target 5592 (api.example.com). You can check the progress by listing scans in a few minutes.

---

**👤 You:**
> "Show me the risk score summary for our organization."

**🤖 AI Agent:**
> Accessing risk scores... Your organization's overall security score is 78/100. The score has improved by 5% since last month. Your primary risk drivers are outdated software on 2 targets. Would you like to see those targets?


## ❓ FAQ

**Q: How do I find my Halo Security API Key?**
Log in to your Halo Security account, navigate to **Account Settings** and then to the **API** section. You will be able to generate and copy your unique API key from there.

**Q: Can I trigger a new scan through this integration?**
Yes! Use the `trigger_scan` tool by providing the unique target ID of the asset you want to assess. Halo Security will initiate the scan immediately.

**Q: How are security issues categorized?**
Issues are categorized by their severity (e.g., Critical, High, Medium, Low) and type (e.g., Vulnerability, Information, SSL Issue). You can use `list_issues` to see all findings.

**Q: Is it possible to add new domains to monitor?**
Yes, the `add_target` tool allows you to add new domains or IP addresses to your security perimeter directly from the AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/halo-security](https://vinkius.com/mcp/halo-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Halo Security** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `halo-security` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Halo Security** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "halo-security": {
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
