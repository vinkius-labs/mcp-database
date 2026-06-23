# Cyberimpact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cyberimpact-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing lists and members — list subscribers, update profiles, and organize groups directly from any AI agent.

## Description
Connect your **Cyberimpact** account to any AI agent to streamline your email marketing workflows. Manage subscribers and groups through natural conversation.

### What you can do

- **Member Management** — List all members, fetch specific details by email, and create or update subscriber profiles using `upsert_member`.
- **Group Organization** — List all available groups and view members within specific segments using `list_group_members`.
- **Subscriber Actions** — Add members to specific groups for targeted campaigns or remove them from your account entirely.
- **Profile Customization** — Update names and language preferences (English/French) for your contacts to ensure personalized communication.

### How it works

1. Subscribe to this server
2. Enter your Cyberimpact API Key
3. Start managing your marketing lists from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — quickly update subscriber lists and check group memberships without logging into the dashboard
- **Sales Teams** — ensure leads are correctly categorized in the right marketing groups directly from their workflow
- **Support Teams** — verify member details or remove users upon request through a simple chat interface


## Available Tools (7)
- **add_group_member**: Add a member to a group
- **delete_member**: Delete a member
- **get_member**: Get details for a specific member
- **list_group_members**: List members in a group
- **list_groups**: List all groups
- **list_members**: List all members
- **upsert_member**: Create or update a member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyberimpact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the members currently in my Cyberimpact account."

**🤖 AI Agent:**
> I've retrieved your member list. You have several active subscribers, including 'john.doe@example.com' and 'jane.smith@test.com'. Would you like to see details for a specific member?

---

**👤 You:**
> "Add the email 'newlead@company.com' to group ID 502."

**🤖 AI Agent:**
> I have successfully added 'newlead@company.com' to group 502. The member is now part of that segment for your future campaigns.

---

**👤 You:**
> "Update the member 'contact@domain.com' with the first name 'Alice' and set language to French."

**🤖 AI Agent:**
> Processing the update... I've updated 'contact@domain.com' with the name Alice and set the language preference to 'fr_ca'.


## ❓ FAQ

**Q: How can I update a subscriber's language preference?**
Use the `upsert_member` tool and specify the `language` parameter with either 'en_ca' or 'fr_ca'. This will update the existing member's profile or create a new one with that preference.

**Q: Is it possible to see which members belong to a specific marketing group?**
Yes. By using the `list_group_members` tool with the specific group ID, the agent will retrieve the full list of subscribers associated with that segment.

**Q: Can I completely remove a contact from my Cyberimpact account via AI?**
Yes, the `delete_member` tool allows you to remove a member from your account using their email address as the identifier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cyberimpact-alternative-1](https://vinkius.com/mcp/cyberimpact-alternative-1)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `cyberimpact-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cyberimpact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cyberimpact-alternative-1": {
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
