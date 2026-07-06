# McLeod Software MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mcleod-software)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Transportation management via McLeod Software — manage orders, dispatches, and carriers.

## Description
Connect your **McLeod Software** LoadMaster or PowerBroker instance to any AI agent and take full control of your transportation management through natural conversation.

### What you can do

- **Order Management** — List all orders, search by term, and fetch detailed shipment metadata
- **Dispatch Orchestration** — Monitor active dispatches, movements, and driver assignments in real-time
- **Entity Management** — List and inspect master records for customers, carriers, and company drivers
- **Operational Visibility** — Access stop-level details for movements and detailed dispatch configurations

### How it works

1. Subscribe to this server
2. Enter your McLeod Base URL, Client ID, Client Secret, and Company ID
3. Start managing your logistics operations from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_order**: Get details for a specific order
- **list_carriers**: List master carrier records
- **list_customers**: List master customer records
- **list_dispatches**: List dispatch assignments
- **list_drivers**: List all drivers
- **list_movements**: List truckload movements
- **list_orders**: List all transportation orders
- **list_stops**: List stops for a movement
- **search_orders**: Search for orders by term
- **get_dispatch_details**: Get details for a specific dispatch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **McLeod Software** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 transportation orders."

**🤖 AI Agent:**
> Retrieving orders... I found several orders including ORD-98765 for TechCorp and ORD-98764 for GlobalLogistics.

---

**👤 You:**
> "Search for orders related to 'Chicago'."

**🤖 AI Agent:**
> Searching... I identified 3 orders with routes starting or ending in Chicago.

---

**👤 You:**
> "What is the status of dispatch assignment ID 555?"

**🤖 AI Agent:**
> Inspecting dispatch... Assignment 555 is currently 'In Transit', driven by John Smith.


## ❓ FAQ

**Q: How do I get my McLeod API credentials?**
You typically need to contact your internal McLeod admin or partner@mcleodsoftware.com to enable the API and receive your OAuth 2.0 Client ID and Secret.

**Q: What is the Company ID?**
The Company ID is a unique string used in the `X-com.mcleodsoftware.CompanyID` header to identify your specific TMS database/company.

**Q: Is my transportation data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mcleod-software](https://vinkius.com/mcp/mcleod-software)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **McLeod Software** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mcleod-software` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **McLeod Software** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mcleod-software": {
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
