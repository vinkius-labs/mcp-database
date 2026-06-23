# Socket.dev (Dependency Security) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/socketdev-dependency-security)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Protect your software supply chain by scanning dependencies, checking package security scores, and monitoring threat feeds directly from your AI agent.

## Description
Connect **Socket.dev** to your AI agent to proactively defend against supply chain attacks. This MCP server allows you to analyze open-source packages, scan manifest files, and monitor for malicious dependencies without leaving your development environment.

### What you can do

- **Package Analysis** — Get deep security scores and identify issues for specific packages using PURLs (e.g., npm, PyPI, Go).
- **Dependency Scanning** — Upload manifest files like `package.json` or `requirements.txt` to create comprehensive security scans.
- **Report Management** — List and retrieve detailed security reports, including policy compliance and alert data.
- **Threat Intelligence** — Access a real-time feed of malicious packages detected by Socket's analysis engine.
- **Organization Oversight** — Manage scans across different organizations and monitor your API usage quotas.

### How it works

1. Subscribe to this server
2. Enter your Socket.dev API Token
3. Start auditing your dependencies directly from Claude, Cursor, or any MCP-compatible client

Stop guessing if a package is safe. Let your AI agent use Socket's industry-leading telemetry to catch typosquatting, backdoors, and telemetry before they enter your codebase.

### Who is this for?

- **Security Engineers** — Automate the review of new dependencies and monitor organizational security posture.
- **Developers** — Check package safety scores instantly before running `npm install` or `pip install`.
- **DevOps Teams** — Integrate dependency scanning into the conversation to quickly triage security reports.


## Available Tools (10)
- **create_scan**: Provide manifest files data (e.g., package.json, requirements.txt).

Create a new scan by uploading manifest files
- **delete_scan**: Delete a scan
- **get_package_issues**: g., pkg:npm/babel).

Get issues/alerts for a specific package
- **get_package_score**: g., pkg:npm/babel).

Get the security score for a specific package
- **get_quota**: Check remaining API quota
- **get_report**: Get detailed report data
- **get_scan**: Get scan metadata and status
- **get_threat_feed**: Access the real-time threat feed
- **list_organizations**: List organizations the token has access to
- **list_reports**: List reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Socket.dev (Dependency Security)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the security score for the npm package 'axios'."

**🤖 AI Agent:**
> I've checked the security score for `pkg:npm/axios`. It currently has a high security score of 98/100, with no critical issues detected in the latest version.

---

**👤 You:**
> "List all security reports for my organization."

**🤖 AI Agent:**
> I've retrieved the reports. You have 3 recent scans available. Would you like me to get the details for the most recent report (ID: rep_12345)?

---

**👤 You:**
> "Show me the real-time threat feed from Socket."

**🤖 AI Agent:**
> Fetching the threat feed... I found several recently flagged malicious packages, including 'discord-selfbot-v14' which was flagged for containing malware. Be cautious if these appear in your dependencies.


## ❓ FAQ

**Q: How can I check if a specific npm package is safe to use?**
You can use the `get_package_score` tool by providing the Package URL (PURL), such as `pkg:npm/lodash`. The agent will return a security score and risk assessment.

**Q: Can I scan my entire project's dependencies at once?**
Yes! Use the `create_scan` tool and provide the content of your manifest files (like `package.json`). Socket will analyze all dependencies and generate a report.

**Q: How do I see the specific security issues found in a package?**
Use the `get_package_issues` tool with the package's PURL. It will list all alerts, such as telemetry, install scripts, or known vulnerabilities associated with that package.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/socketdev-dependency-security](https://vinkius.com/mcp/socketdev-dependency-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Socket.dev (Dependency Security)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `socketdev-dependency-security` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Socket.dev (Dependency Security)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "socketdev-dependency-security": {
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
