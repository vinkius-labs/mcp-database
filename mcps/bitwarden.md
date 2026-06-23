# Bitwarden MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitwarden)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage Bitwarden organization resources—collections, events, groups, members, and policies—directly from your AI agent.

## Description
Connect your **Bitwarden** organization to any AI agent to audit security logs, manage collections, and oversee your team's access through natural conversation.

### What you can do

- **Collections Management** — List all organization collections to understand how vault items are organized and shared
- **Audit Trail & Events** — Retrieve detailed event logs to monitor administrative actions and security-related activities
- **Member Oversight** — List all members within your organization to verify access and seat utilization
- **Group Organization** — Query user groups to manage team-based permissions and access control
- **Policy Review** — Inspect active security and administrative policies to ensure compliance with organizational standards

### How it works

1. Subscribe to this server
2. Enter your Bitwarden Client ID and Client Secret
3. Start auditing your organization from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Administrators** — quickly audit event logs and verify policy compliance without navigating the web vault
- **IT Operations** — manage organization members and groups directly from automation workflows
- **Compliance Officers** — retrieve collections and access structures for security reporting


## Available Tools (5)
- **list_collections**: List organization collections
- **list_events**: List organization event logs
- **list_groups**: List organization groups
- **list_members**: List organization members
- **list_policies**: List organization policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitwarden** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all collections in my Bitwarden organization."

**🤖 AI Agent:**
> I've retrieved the collections for your organization. You have 4 active collections: 'Engineering-Shared', 'Marketing-Vault', 'Finance-Keys', and 'General-Access'. Would you like more details on any of these?

---

**👤 You:**
> "Show me the recent event logs for auditing."

**🤖 AI Agent:**
> Fetching the audit trail... I found the latest events. Recent actions include a policy update by 'admin@corp.com' and 3 new member invitations. Would you like me to list the specific details of the policy change?

---

**👤 You:**
> "Who are the current members of our Bitwarden organization?"

**🤖 AI Agent:**
> I've compiled the member list. There are currently 12 active members and 2 pending invitations. Notable users include 'Alice (Owner)', 'Bob (Admin)', and 'Charlie (User)'. Should I check their group assignments?


## ❓ FAQ

**Q: Can I use this to audit recent administrative changes in my Bitwarden organization?**
Yes! Use the `list_events` tool to retrieve the audit trail. It provides a detailed log of events, including who performed what action and when, helping you maintain security oversight.

**Q: How do I check which security policies are currently active?**
Simply ask the agent to run the `list_policies` action. This will return all administrative and security policies configured for your organization, such as Master Password requirements or Two-step Login rules.

**Q: Is it possible to see all the shared collections we have set up?**
Yes, the `list_collections` tool allows you to retrieve all collections available to the organization, helping you understand how shared secrets are categorized.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitwarden](https://vinkius.com/mcp/bitwarden)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bitwarden** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bitwarden` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bitwarden** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bitwarden": {
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
