# Cyberimpact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cyberimpact-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Email marketing automation with Cyberimpact.

## Description
The Cyberimpact MCP server allows your AI agent to manage members, groups, and mailings. Create campaigns, add subscribers, and track results directly from your chat.


## Available Tools
- **add_member_to_group**: Add an existing member to a group
- **create_group**: Create a new group
- **create_mailing**: Create a new mailing
- **create_member**: Create a new member (contact)
- **delete_member**: Delete a member from the account
- **get_me**: Check API connectivity and get account context
- **list_groups**: List all groups
- **list_mailings**: List all mailings (campaigns)
- **list_members**: List all members (contacts)
- **list_templates**: List all available templates
- **retrieve_member**: Get details of a specific member
- **unsubscribe_member**: Unsubscribe a member from all mailings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyberimpact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all members in my Cyberimpact account."

**🤖 AI Agent:**
> I've fetched your member list. You currently have 4,502 subscribed members across all your lists.

---

**👤 You:**
> "Create a new group called 'April Newsletter'."

**🤖 AI Agent:**
> The group 'April Newsletter' has been successfully created with ID #8493.

---

**👤 You:**
> "Unsubscribe member 'MEMBER_ID' from all mailings."

**🤖 AI Agent:**
> Member 'MEMBER_ID' has been fully unsubscribed and removed from active mailing lists.


## ❓ FAQ

**Q: Which plan is required for API access?**
The API is available for Plus and Pro plans in Cyberimpact.

**Q: How long is an API token valid?**
API tokens are valid for 10 years unless manually deleted.

**Q: Can I manage groups via the API?**
Yes, you can create, retrieve, edit, or delete groups and manage memberships.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cyberimpact-alternative](https://vinkius.com/mcp/cyberimpact-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cyberimpact** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cyberimpact-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cyberimpact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cyberimpact-alternative": {
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
