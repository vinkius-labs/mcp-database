# Minutemailer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/minutemailer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Email and SMS marketing — manage contacts, lists, and templates via Minutemailer.

## Description
Connect your **Minutemailer** account to automate your email and SMS marketing workflows. This server allows your AI agents to manage your audience and monitor campaigns directly.

### What you can do

- **Audience Management** — List, create, and remove contacts seamlessly
- **Segment Organization** — Access your contact lists and smart lists for targeted outreach
- **Template Visibility** — Browse available email templates for your campaigns
- **Activity Monitoring** — Track account events and historical data in real-time

### How it works

1. Subscribe to this server
2. Enter your **Minutemailer API Token**
3. Start managing your marketing engine from Claude, Cursor, or any MCP client


## Available Tools
- **create_contact**: Create a new contact
- **delete_contact**: Delete a contact
- **get_account_info**: Get account metadata
- **list_contacts**: List all contacts
- **list_events**: List account events
- **list_contact_lists**: List all contact lists
- **list_smart_lists**: List smart lists
- **list_templates**: List email templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Minutemailer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Minutemailer contacts."

**🤖 AI Agent:**
> Fetching contacts... I've found 1,200 contacts in your account. Here are the most recent ones...

---

**👤 You:**
> "Add 'jane.doe@example.com' to my contact list."

**🤖 AI Agent:**
> Adding contact... Success! Jane Doe has been added to your Minutemailer audience.


## ❓ FAQ

**Q: Where do I find my API Token?**
Log in to Minutemailer, go to your account settings, and look for the 'API Settings' section to generate a token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/minutemailer](https://vinkius.com/mcp/minutemailer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Minutemailer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `minutemailer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Minutemailer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "minutemailer": {
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
