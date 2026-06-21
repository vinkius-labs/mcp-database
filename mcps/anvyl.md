# Anvyl MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anvyl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Streamline your supply chain with Anvyl — manage purchase orders, track shipments, and coordinate with suppliers via AI.

## Description
The **Anvyl MCP Server** brings visibility and automation to your supply chain operations. By connecting your Anvyl account to your AI agent, you can seamlessly track production progress, manage parts and suppliers, and update critical milestones using natural language.

### What you can do

- **Order Visibility** — List all purchase orders and drill down into specific order details to check status and quantities.
- **Milestone Management** — Track production and shipping milestones. Confirm completions or record delays directly from your chat.
- **Supplier Coordination** — Quickly retrieve supplier information and part specifications stored in Anvyl.
- **Logistics Tracking** — Access tracking records and logistics data for any purchase order to keep your team informed on delivery timelines.

### How it works

1. Subscribe to this server
2. Provide your Anvyl API Key and Team ID
3. Start managing your supply chain workflow through your AI chat interface.

### Who is this for?

- **Supply Chain Managers** — Automate the tracking of multiple POs and receive instant updates on milestone statuses.
- **Procurement Teams** — Efficiently look up part details and supplier contact information during planning.
- **Operations Leads** — Keep a high-level view of production health and logistics without manually navigating through dashboards.


## Available Tools
- **confirm_milestone**: Confirm a milestone for a purchase order
- **delay_milestone**: Delay a milestone for a purchase order
- **get_part**: Get details for a specific part
- **get_purchase_order**: Get details for a specific purchase order
- **get_supplier**: Get details for a specific supplier
- **list_logistics**: List tracking records for a purchase order
- **list_milestones**: List milestones for a purchase order
- **list_parts**: List parts in the Anvyl account
- **list_purchase_orders**: List Anvyl purchase orders for the team
- **list_suppliers**: List suppliers in the Anvyl account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anvyl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active purchase orders."

**🤖 AI Agent:**
> I've retrieved 12 active purchase orders. The most recent one is PO #8821 for 'Aluminum Housings' with an expected delivery date of April 15th.

---

**👤 You:**
> "Check the milestones for order PO-123."

**🤖 AI Agent:**
> Order PO-123 has 5 milestones. 'Material Sourcing' and 'Production Start' are completed. 'Quality Inspection' is currently in progress and expected by tomorrow.

---

**👤 You:**
> "Delay milestone 'm_456' for order PO-789 by 1 week because of raw material shortage."

**🤖 AI Agent:**
> I've updated the milestone 'm_456' for order PO-789. The new expected date is now set to May 22nd, and the reason 'raw material shortage' has been recorded.


## ❓ FAQ

**Q: Where do I find my Anvyl Team ID?**
You can find your Team ID in the URL when you are logged into the Anvyl dashboard (e.g., `app.anvyl.com/teams/{TEAM_ID}/...`) or in your workspace settings.

**Q: Can I update the status of a production milestone via AI?**
Yes, you can use the `confirm_milestone` tool to mark a milestone as complete or `delay_milestone` if production is behind schedule, providing a reason and a new expected date.

**Q: How do I track the shipping status of my orders?**
Use the `list_logistics` tool with your Purchase Order ID. It will return all tracking records and shipping updates associated with that specific order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anvyl](https://vinkius.com/mcp/anvyl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anvyl** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `anvyl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anvyl** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anvyl": {
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
