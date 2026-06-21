# Acunetix 360 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acunetix-360)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automated web vulnerability scanning — manage scans, track issues, and audit security via AI.

## Description
Connect your **Acunetix 360** account to your AI agent to automate your web application security workflow. From launching new vulnerability scans to auditing identified security issues across your infrastructure, your agent manages application security through natural conversation.

### What you can do

- **Automated Scanning** — Launch new vulnerability scans for your web applications and APIs directly from chat
- **Issue Tracking** — List and retrieve detailed information on identified vulnerabilities, including severity levels and remediation tips
- **Scan Monitoring** — Track the progress and status of active security scans across your organization
- **Security Auditing** — Quickly retrieve a list of all identified issues to support compliance and risk management
- **CI/CD Integration Support** — Audit scan results from recent builds to ensure security is maintained throughout the development lifecycle

### How it works

1. Subscribe to this server
2. Enter your Acunetix 360 User ID and API Token
3. Start monitoring and managing your application security through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate vulnerability triage and monitor large-scale scanning operations
- **DevSecOps Teams** — integrate automated security checks intoCI/CD pipelines and audit results via AI
- **Web Developers** — quickly check for vulnerabilities in their applications during the development phase
- **Compliance Officers** — retrieve security reports and audit logs for risk assessment


## Available Tools
- **list_scans**: List vulnerability scans
- **launch_scan**: Start a new security scan
- **list_vulnerabilities**: List all identified security issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acunetix 360** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all high-severity vulnerabilities found in my last scan."

**🤖 AI Agent:**
> I've retrieved the identified issues. Your last scan found 3 high-severity vulnerabilities, including a SQL Injection and two Cross-Site Scripting (XSS) flaws. Would you like the remediation details for these?


## ❓ FAQ

**Q: How do I launch a new scan?**
Use the `launch_scan` tool and provide the target URL or Website ID. Your agent will initiate the vulnerability scan and provide a Scan ID for monitoring.

**Q: What is the API rate limit for Acunetix 360?**
Acunetix 360 APIs enforce server-side rate-limiting to ensure stability. Pagination limits are commonly applied to list endpoints, returning up to 100 objects per query.

**Q: Can I integrate scan results into issue trackers?**
Yes! Acunetix 360 results can be pushed to issue trackers like Jira, Azure Boards, and GitLab. The agent can summarize these vulnerability outputs for straightforward ticket creation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acunetix-360](https://vinkius.com/mcp/acunetix-360)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acunetix 360** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `acunetix-360` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acunetix 360** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acunetix-360": {
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
