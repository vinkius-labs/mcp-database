# Kolide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kolide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Audit fleet security — list devices, track issues, and monitor people.

## Description
Connect your AI agent to **Kolide** to get full visibility into your organization's fleet security and device health.

### Key Features

- **Fleet Inventory** — List all managed devices and their high-level security status
- **Issue Tracking** — Monitor active security vulnerabilities and misconfigurations across your fleet
- **People & Ownership** — See which users are associated with which devices and their individual compliance state
- **Security Checks** — Audit available security checks and dive into specific failure conditions
- **Audit Logs** — Access a chronological history of administrative and security events

### How to setup

1. Subscribe to this server
2. Log in to Kolide, go to **Settings** > **API**, and generate a Bearer Token
3. Enter your token in the configuration
4. Start auditing your fleet via natural language


## Available Tools (10)
- **list_kolide_devices**: Use this to audit fleet security posture and identify individual device IDs.

List all devices in the fleet
- **get_device_details**: Get details for a specific device
- **list_kolide_issues**: List security issues across the fleet
- **get_issue_details**: Get details for a specific security issue
- **list_kolide_people**: List people/users managed in Kolide
- **get_person_details**: Get details for a specific person
- **list_kolide_checks**: List all available security checks
- **get_check_details**: Get details for a specific check
- **list_kolide_audit_logs**: List fleet audit logs
- **get_kolide_fleet_stats**: g., total devices, online status, issue count).

Get high-level fleet statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kolide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all devices currently online in Kolide"

**🤖 AI Agent:**
> Retrieving online devices… I've found 42 devices currently active. Most are MacBooks running macOS 14. Would you like to see if any of these have pending security issues?

---

**👤 You:**
> "What are the most common security issues in my fleet?"

**🤖 AI Agent:**
> The most frequent issues are 'Outdated OS' (12 devices) and 'Full Disk Encryption Disabled' (5 devices). I can provide the names of the affected users if you'd like.

---

**👤 You:**
> "Show fleet statistics for today"

**🤖 AI Agent:**
> Current fleet stats: 150 total devices, 92% compliance rate, 12 active issues, and 5 new devices enrolled this week. Overall health is 'Good'.


## ❓ FAQ

**Q: Where do I find my Kolide API Token?**
Log in to the Kolide dashboard, navigate to **Settings** in the bottom left, and select the **API** tab to generate a token.

**Q: Can I see hardware details of a device?**
Yes, the `get_device_details` tool returns hardware specifications along with security data.

**Q: Does this support multi-tenant accounts?**
The API key is typically scoped to a specific organization. Ensure you are using the token for the desired fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kolide](https://vinkius.com/mcp/kolide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kolide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kolide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kolide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kolide": {
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
