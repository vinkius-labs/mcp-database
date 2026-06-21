# Shipmondo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipmondo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Ship packages across Scandinavia and Europe with multi-carrier label printing, tracking, and return management from one platform.

## Description
Connect your **Shipmondo** account to any AI agent and take full control of your e-commerce logistics. This integration uses the Shipmondo v3 REST API to orchestrate multi-carrier shipments, manage sales orders, and query global pickpoints.

### Core Capabilities

- **Shipment Orchestration** — List, retrieve, and create shipments programmatically across hundreds of supported carriers.
- **Sales Order Management** — Monitor your fulfillment pipeline by retrieving detailed order metadata and statuses.
- **Pickpoint Intelligence** — Find the nearest delivery points by carrier code, country, and zip code to optimize customer delivery options.
- **Financial Visibility** — Access real-time account balances to ensure uninterrupted logistics operations.

### How it works

1. Subscribe to this server
2. Enter your Shipmondo API User and API Key
3. Start managing your logistics from Claude, Cursor, or any MCP client

No more manual carrier portal logins. Your AI acts as a dedicated logistics coordinator.


## Available Tools
- **create_shipment**: Pass data as a JSON string.

Create a new shipment
- **get_account_balance**: Check account balance
- **get_order**: Get sales order details
- **get_shipping_quote**: Get a shipping rate quote
- **get_shipment**: Get details for a specific shipment
- **list_carriers**: List all available shipping carriers
- **list_orders**: List all sales orders
- **list_pickpoints**: Find carrier pickpoints
- **list_returns**: List all return shipments
- **list_shipments**: List all shipments
- **list_warehouses**: List all configured warehouses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipmondo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find DHL pickpoints in Denmark for zip code 2100."

**🤖 AI Agent:**
> Searching for pickpoints... I found 3 DHL locations in zip code 2100: 'ServicePoint A', 'ServicePoint B', and 'Convenience Store C'. Which one would you like to select?

---

**👤 You:**
> "Show me all shipments from this week with carrier performance and delivery status breakdown."

**🤖 AI Agent:**
> 145 shipments this week. Delivered (98): 67.6% (avg delivery: 2.1 days). In transit (34): 23.4%. Processing (8): 5.5%. Exception (5): 3.4% (2 address issues, 2 customs holds, 1 damaged). By carrier: PostNord (67 shipments, 97% on-time), GLS (45, 94% on-time), UPS (23, 98% on-time), DHL (10, 100% on-time). Average shipping cost: €5.40. Total shipping spend: €783. International shipments: 23 (16%). Returns processed: 12.

---

**👤 You:**
> "Get shipping rate quotes for a 5kg package from Copenhagen to Berlin with all available carriers."

**🤖 AI Agent:**
> Shipping quotes for 5kg package (30x20x15cm), Copenhagen → Berlin. PostNord Economy: €4.20 (5-7 business days). GLS Standard: €6.80 (3-4 days). UPS Standard: €8.90 (2-3 days). DHL Express: €14.50 (1-2 days). UPS Express: €16.20 (next day). Best value: PostNord Economy at €4.20. Fastest: UPS Express at €16.20. Recommended: GLS Standard (best price-to-speed ratio). All include tracking. Insurance available: +€1.50 (up to €500 coverage).


## ❓ FAQ

**Q: Can my AI find pickpoints for a specific carrier like PostNord or DHL?**
Yes! Use the `list_pickpoints` tool with the carrier code (e.g., 'pnd' for PostNord, 'dhl' for DHL) and the zip code. Your agent will return a list of available locations instantly.

**Q: How do I check if I have enough balance to generate new labels?**
Simply ask the AI to run the `get_account_balance` action. It will retrieve your real-time balance directly from your Shipmondo account.

**Q: Where do I find my API credentials?**
Log in to your Shipmondo account, go to **Settings** > **API** > **Access**, and you will find your API User and API Key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipmondo](https://vinkius.com/mcp/shipmondo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipmondo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shipmondo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipmondo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipmondo": {
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
