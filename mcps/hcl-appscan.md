# HCL AppScan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hcl-appscan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hcl-appscan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hcl-appscan-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **HCL AppScan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hcl-appscan](https://vinkius.com/mcp/hcl-appscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
