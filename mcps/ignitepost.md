# IgnitePOST MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ignitepost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage hand-written note orders and outreach campaigns via IgnitePOST API.

## Description
Empower your AI agents to send personalized, hand-written notes with IgnitePOST. This MCP server allows you to list and retrieve orders, manage templates, view available fonts and stationery, and track outreach campaigns directly through the IgnitePOST API. Ideal for automating relationship marketing and high-touch customer outreach.


## Available Tools
- **get_order**: Retrieves details for a specific order
- **list_campaigns**: Lists all outreach campaigns
- **list_contacts**: Lists all contacts
- **list_envelopes**: Lists all available envelopes
- **list_fonts**: Lists all available hand-written fonts
- **list_orders**: Lists all hand-written note orders
- **list_products**: Lists all available products
- **list_stationeries**: Lists all available stationery types
- **list_templates**: Lists all letter templates
- **verify_auth**: Verifies if the API token is valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IgnitePOST** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent hand-written note orders in IgnitePOST."

**🤖 AI Agent:**
> I'll fetch your recent order list for you.

---

**👤 You:**
> "Show me available fonts for my hand-written cards."

**🤖 AI Agent:**
> I'll retrieve the list of hand-written fonts supported by IgnitePOST.

---

**👤 You:**
> "Check the status of order ID '789'."

**🤖 AI Agent:**
> I'll look up the details and current status for that specific order.


## ❓ FAQ

**Q: How do I get IgnitePOST API credentials?**
Log in to your IgnitePOST dashboard, navigate to Profile > API Keys, and generate your Secret Token.

**Q: Can I test without sending real mail?**
Yes, you can use a test API key or include the X-TESTING: true header in your requests to test the integration without incurring costs.

**Q: What fonts are available?**
You can use the list_fonts tool to see all available hand-written fonts supported by IgnitePOST.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ignitepost](https://vinkius.com/mcp/ignitepost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IgnitePOST** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ignitepost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IgnitePOST** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ignitepost": {
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
