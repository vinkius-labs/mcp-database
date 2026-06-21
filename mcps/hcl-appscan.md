# HCL AppScan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hcl-appscan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage security scans and vulnerabilities with HCL AppScan — track issues and audit applications via AI.

## Description
The **HCL AppScan MCP Server** brings powerful application security testing capabilities directly to your AI agent. Seamlessly manage your security posture by monitoring vulnerabilities, tracking scan progress, and auditing your application inventory across HCL AppScan on Cloud (ASoC).

### Key Features

- **Inventory Management** — List and search for applications in your security inventory to find their unique IDs.
- **Vulnerability Tracking** — Retrieve detailed lists of security issues found during scans, including severity and status.
- **Scan Oversight** — Monitor all performed scans and check the real-time status of active security tests.
- **Dynamic Analysis (DAST)** — Start new DAST scans for your web applications directly from your chat interface.
- **Agent & Presence Monitoring** — List available Presences (local agents) used for scanning internal applications.
- **Real-time Insights** — Get instant summaries of your security findings and prioritize remediation efforts.

### Who is this for?

- **Security Engineers** — Quickly audit security findings across multiple applications without manual dashboard exports.
- **DevSecOps Teams** — Integrate security scan monitoring and initiation into your automated workflows.
- **Compliance Officers** — Monitor application security status and ensure all apps are regularly scanned.


## Available Tools (10)
- **get_account_check**: Verify AppScan account connection
- **get_account_info**: Retrieve authenticated user information
- **get_app**: Get details for a specific application
- **get_issue**: Get detailed information about a specific vulnerability
- **get_scan**: Get details and status for a specific scan
- **list_apps**: List all applications in your AppScan inventory
- **list_issues**: List vulnerabilities found for a specific application
- **list_presence**: List AppScan Presences (local agents)
- **list_scans**: List all scans performed in the account
- **start_dast_scan**: Start a new Dynamic Analysis (DAST) scan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HCL AppScan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications in my AppScan inventory."

**🤖 AI Agent:**
> I've retrieved your application inventory. You have 15 applications, including 'Customer Portal', 'Payment API', and 'Mobile Backend'.

---

**👤 You:**
> "Show me high severity issues for application 'Customer Portal'."

**🤖 AI Agent:**
> I've found 3 high severity issues for 'Customer Portal', including a 'SQL Injection' vulnerability and a 'Cross-Site Scripting' (XSS) issue.

---

**👤 You:**
> "Start a new DAST scan for appId '12345' with URL 'https://portal.example.com'."

**🤖 AI Agent:**
> A new DAST scan (ID: scan_998877) has been successfully started for 'Customer Portal' targeting 'https://portal.example.com'.


## ❓ FAQ

**Q: How do I get my AppScan API Key ID and Secret?**
Log in to the AppScan on Cloud console, go to your **User Profile** (top right), and select **API Keys**. You can generate a new Key ID and Key Secret there.

**Q: Does this server support the EU region?**
Yes, you can configure the `APPSCAN_REGION` environment variable to `eu` to connect to the European data center (`eu.cloud.appscan.com`).

**Q: Can I start a scan for an internal application?**
Yes, provided you have an AppScan Presence (local agent) configured. You can use the `list_presence` tool to check their availability before starting a scan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hcl-appscan](https://vinkius.com/mcp/hcl-appscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HCL AppScan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hcl-appscan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HCL AppScan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hcl-appscan": {
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
