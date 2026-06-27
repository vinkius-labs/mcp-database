# folk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/folk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage relationships across sales, recruiting, and partnerships with a lightweight CRM that syncs contacts from everywhere.

## Description
Connect your **folk** CRM account to any AI agent and simplify how you manage your professional relationships, coordinate contact groups, and track interactions through natural conversation.

### What you can do

- **Contact Oversight** — List all contacts and retrieve detailed profile metadata, including custom fields and status.
- **Group Management** — Coordinate your contact lists by querying and managing specific groups in your folk workspace.
- **Interaction Tracking** — Retrieve a complete history of emails, meetings, and calls for any contact to maintain context.
- **Relationship CRM** — Create new contact records and update profile data programmatically via AI.
- **Notes & Insights** — List and query all notes and comments associated with your contacts to capture important details.
- **Operational Visibility** — Verify account configurations and monitor your professional ecosystem directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your folk API Key (found in your account settings)
3. Start managing your professional network from Claude, Cursor, or any MCP client

### Who is this for?

- **Founders & Entrepreneurs** — quickly retrieve investor details and track recent interactions via simple AI commands.
- **Sales & BD Teams** — manage lead groups and verify contact history directly from the workspace.
- **Recruiters** — track candidate pipelines and monitor interview notes via the AI assistant.


## Available Tools (6)
- **list_contact_notes**: List notes for a contact
- **create_contact**: Create a new contact
- **get_contact_details**: Get details for a specific contact
- **list_contacts**: Optionally filter by group ID.

List folk contacts
- **list_groups**: List folk groups
- **list_interactions**: List interactions for a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **folk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in my folk account."

**🤖 AI Agent:**
> I've retrieved your contacts. You have access to 150 profiles including 'John Doe', 'Sarah Miller', and 'Mike Ross'. Which one would you like to see the details or interaction history for?

---

**👤 You:**
> "Show me the recent interactions for 'John Miller' (ID: 10293)."

**🤖 AI Agent:**
> Fetching interactions... For John Miller, there are 3 recent events: an email sent yesterday, a Zoom meeting from last week, and a call log. Would you like the details of the latest email?

---

**👤 You:**
> "Add a new contact: 'Anna White' (anna@example.com)."

**🤖 AI Agent:**
> Success! Anna White (anna@example.com) has been added to your folk CRM with ID cont_88231. She is currently in your main directory. Would you like me to assign her to a group?


## ❓ FAQ

**Q: Can I see all contacts in a specific folk group via AI?**
Yes! Use the `list_contacts` tool and provide the Group ID. Your agent will retrieve all profiles and metadata for the contacts in that specific group.

**Q: How do I add a new person to my folk directory?**
Use the `create_contact` action. Provide the first name, last name, and email address to register the new contact in your folk account instantly.

**Q: Is it possible to see the interaction history for a contact via AI?**
Absolutely. Run the `list_interactions` query with the Contact ID. The agent will retrieve a history of emails, meetings, and calls associated with that profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/folk](https://vinkius.com/mcp/folk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **folk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `folk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **folk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "folk": {
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
