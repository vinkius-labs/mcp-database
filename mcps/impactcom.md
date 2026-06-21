# Impact.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/impactcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage partnership campaigns, ads, and affiliate payouts via Impact.com API.

## Description
Empower your AI agents to manage your partnership ecosystem with Impact.com (formerly Impact Radius). This MCP server allows you to list campaigns, retrieve ad details, track actions and conversions, manage invoices, and view affiliate payouts directly through the Impact API. Ideal for automating partnership marketing and performance monitoring.


## Available Tools (10)
- **list_actions**: Lists all actions (conversions, clicks)
- **list_ads**: Lists all ads in your account
- **list_campaigns**: Lists all partnership campaigns
- **list_contracts**: Lists all partnership contracts
- **list_invoices**: Lists all invoices
- **list_media_partners**: Lists all media partners (affiliates)
- **list_payouts**: Lists all payouts to partners
- **list_queued_notifications**: Lists all queued action notifications
- **list_transactions**: Lists all financial transactions
- **list_webhooks**: Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Impact.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active partnership campaigns in my Impact.com account."

**🤖 AI Agent:**
> I'll fetch the list of your partnership campaigns for you.

---

**👤 You:**
> "Show me recent conversions and actions from today."

**🤖 AI Agent:**
> I'll retrieve the latest actions and conversions recorded in your account.

---

**👤 You:**
> "Check for any pending invoices or payouts."

**🤖 AI Agent:**
> I'll look up your invoices and payouts to check for any pending items.


## ❓ FAQ

**Q: How do I get Impact.com API credentials?**
Log in to your Impact account. Brands can find credentials in Settings > Technical > API. Partners can find them by clicking the Cloud icon > API. You need both Account SID and Auth Token.

**Q: Which version of the API is used?**
This MCP uses the latest Impact.com REST API endpoints for comprehensive account and partnership management.

**Q: Can I see real-time conversions?**
Yes, the list_actions tool provides access to tracked actions, including clicks and conversions, recorded in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/impactcom](https://vinkius.com/mcp/impactcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Impact.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `impactcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Impact.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "impactcom": {
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
