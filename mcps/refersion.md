# Refersion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/refersion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your affiliate marketing program via Refersion — list affiliates, track conversions, and manage webhooks directly from any AI agent.

## Description
Connect your **Refersion** account to any AI agent to streamline your affiliate marketing operations through natural conversation.

### What you can do

- **Affiliate Management** — List all registered affiliates, fetch detailed profiles using unique IDs, and register new affiliate accounts instantly.
- **Conversion Tracking** — Query all recorded conversions and create new conversion records to credit your partners accurately for sales.
- **Real-time Updates** — List existing webhook configurations and register new listeners to receive real-time updates on program activities.
- **Deep Inspection** — Fetch complete metadata for specific affiliates and conversions to resolve disputes or analyze performance.

### How it works

1. Subscribe to this server
2. Enter your Refersion Public Key and Secret Key
3. Start managing your affiliate network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Affiliate Managers** — quickly check affiliate details and approve conversions without digging through the dashboard
- **Marketing Teams** — automate the retrieval of performance data and affiliate lists for reporting
- **Developers** — test and manage webhooks and conversion logic directly from the coding environment


## Available Tools (8)
- **create_affiliate**: Create a new affiliate
- **create_conversion**: Create a new conversion
- **create_webhook**: Registers a new webhook listener
- **get_affiliate**: Get details for a specific affiliate
- **get_conversion**: Get details for a specific conversion
- **list_affiliates**: List affiliates for your account
- **list_conversions**: List conversions
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refersion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current affiliates in Refersion."

**🤖 AI Agent:**
> I've retrieved your affiliate list. You have 12 active affiliates, including 'Sarah Jenkins' (ID: aff_882) and 'Tech Reviews Inc' (ID: aff_901). Would you like details on a specific one?

---

**👤 You:**
> "Create a new conversion of 75.00 USD for affiliate ID aff_882."

**🤖 AI Agent:**
> The conversion has been successfully recorded. A new entry for $75.00 USD has been credited to affiliate aff_882 (Sarah Jenkins).

---

**👤 You:**
> "Show me all configured webhooks."

**🤖 AI Agent:**
> You currently have 2 webhooks configured: one for 'New Affiliate' events pointing to your production server and another for 'New Conversion' events.


## ❓ FAQ

**Q: Can I register a new affiliate directly through the AI?**
Yes! Use the `create_affiliate` tool by providing the first name, last name, and email address. The agent will register them in your Refersion account immediately.

**Q: How do I check the details of a specific conversion?**
Simply provide the conversion ID to the `get_conversion` tool. The agent will return the amount, currency, and the associated affiliate information.

**Q: Is it possible to manage webhooks using this server?**
Yes, you can use `list_webhooks` to see your current configuration and `create_webhook` to register new endpoints for real-time notifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/refersion](https://vinkius.com/mcp/refersion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refersion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refersion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refersion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refersion": {
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
