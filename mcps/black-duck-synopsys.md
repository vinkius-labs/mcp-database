# Black Duck (Synopsys) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/black-duck-synopsys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Secure your open source supply chain via Black Duck — list projects, versions, and vulnerabilities directly from any AI agent.

## Description
Connect your **Black Duck (Synopsys)** instance to any AI agent and orchestrate your open source security and license compliance workflows through natural conversation.

### What you can do

- **Project Oversight** — List and retrieve detailed metadata for all your software projects and their versions.
- **Vulnerability Tracking** — Query project versions for known vulnerabilities (CVEs) and retrieve severity levels.
- **BOM Monitoring** — Check the status of Bill of Materials (BOM) calculations to ensure up-to-date compliance data.
- **Policy Management** — List and audit security policy rules defined across your organization.
- **Scan Analysis** — Access code locations and scan histories to track security coverage.
- **User & Access Auditing** — Retrieve user profiles and manage access controls within the platform.

### How it works

1. Subscribe to this server
2. Enter your Black Duck Instance URL and API Token
3. Start securing your code from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — quickly audit vulnerabilities across multiple projects without manual dashboard exports.
- **Developers** — check the security status of their project dependencies straight from the code editor.
- **Compliance Officers** — retrieve policy rule summaries and BOM statuses for periodic reporting.


## Available Tools
- **get_bom_status**: Check BOM calculation status for a project version
- **get_project**: Get details of a specific project
- **list_vulnerabilities**: List vulnerabilities for a project version
- **get_vulnerability_details**: Get details of a specific CVE/Vulnerability
- **list_code_locations**: List all scan code locations
- **list_policy_rules**: List all security policy rules
- **list_project_versions**: List all versions for a specific project
- **list_projects**: List all Black Duck projects
- **list_users**: List all Black Duck users
- **search_projects**: Search projects by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Black Duck (Synopsys)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all versions for project 'Web-Portal'."

**🤖 AI Agent:**
> I've retrieved the versions for 'Web-Portal'. You have 3 versions: '1.0.0' (ID: v1), '1.1.0-beta' (ID: v2), and 'latest' (ID: v3).

---

**👤 You:**
> "Identify any critical vulnerabilities in the backend service repository."

**🤖 AI Agent:**
> Scanning project 'Backend Service'. Found 2 Critical CVEs linked to active OpenSSL dependencies (CVE-2023-xxxx). Actions recommended immediately.

---

**👤 You:**
> "Fetch the BOM status for project Alpha version 2.0."

**🤖 AI Agent:**
> The Bill of Materials (BOM) for Alpha v2.0 is perfectly 'UP_TO_DATE' and fully synchronized within the compliance policy guidelines.


## ❓ FAQ

**Q: Can I check for critical vulnerabilities in a specific project version?**
Yes! Use the `list_vulnerabilities` tool with the Project and Version IDs. Your agent will fetch the list of components with known security flaws and their severity levels.

**Q: How do I know if my Black Duck scan is finished?**
Simply ask the agent to `get_bom_status` for the specific project version. It will return the current calculation status, showing if the BOM is 'Up to date' or still processing.

**Q: What happens if I trigger API rate limits?**
Black Duck limits connections to 100 requests per 10 seconds or 10,000 per 30 minutes. If you exceed this sustained load protection, you will temporarily receive a HTTP 429 error code restricting your IP for 15 minutes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/black-duck-synopsys](https://vinkius.com/mcp/black-duck-synopsys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Black Duck (Synopsys)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `black-duck-synopsys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Black Duck (Synopsys)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "black-duck-synopsys": {
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
