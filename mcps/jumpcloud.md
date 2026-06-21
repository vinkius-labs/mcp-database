# JumpCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jumpcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage users, systems, and directories via JumpCloud API.

## Description
Empower your AI agents with JumpCloud's open directory platform. This MCP server allows you to list and retrieve users, manage user and system groups, track managed systems, and view directories and SSO applications directly through the JumpCloud API. Ideal for automating IT administration and directory management.


## Available Tools
- **get_user**: Returns account metadata, group memberships, and security settings. Use this for detailed user vetting or before making administrative changes.

Retrieves details for a specific user
- **list_applications**: Useful for auditing software access and identifying which SaaS apps are integrated.

Lists all configured SSO applications
- **list_commands**: Useful for auditing automation scripts.

Lists saved management commands
- **list_directories**: Useful for auditing identity source configurations.

Lists all configured directories (LDAP, AD, Google, etc)
- **list_networks**: Useful for auditing WiFi and VPN authentication settings.

Lists all RADIUS networks
- **list_policies**: g., Disk Encryption, Firewall) defined in JumpCloud. Essential for auditing security compliance across the fleet.

Lists all system security policies
- **list_system_groups**: g., "Production Servers", "Employee Laptops"). Useful for identifying device cohorts for policy application.

Lists all system groups
- **list_systems**: Returns hostnames, IDs, and OS versions. Use this to audit company hardware and device compliance.

Lists all systems managed by JumpCloud
- **list_user_groups**: g., Marketing, Developers) configured in JumpCloud. Useful for understanding the organizational structure and access control policies.

Lists all user groups
- **list_users**: Returns usernames, IDs, and account status. Use this as the primary entry point for user auditing and identity management.

Lists all users in JumpCloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JumpCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my JumpCloud directory."

**🤖 AI Agent:**
> I'll fetch the complete list of users from your JumpCloud account.

---

**👤 You:**
> "Show me the managed systems currently active."

**🤖 AI Agent:**
> I'll retrieve the list of systems managed by JumpCloud for you.

---

**👤 You:**
> "Check the user groups in my organization."

**🤖 AI Agent:**
> I'll look up the list of configured user groups in your account.


## ❓ FAQ

**Q: How do I get JumpCloud API credentials?**
Log in to your JumpCloud Admin Console, navigate to Settings > API Settings, and copy your API Key.

**Q: Which API versions are used?**
This MCP utilizes both JumpCloud API v1 and v2 endpoints to provide comprehensive coverage of users, groups, and systems.

**Q: Can I see managed systems?**
Yes, the list_systems tool allows you to retrieve a list of all devices currently managed by your JumpCloud account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jumpcloud](https://vinkius.com/mcp/jumpcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JumpCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jumpcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JumpCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jumpcloud": {
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
