# Dada Now Delivery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dada-now-delivery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Bring Dada Now's Instant Local Delivery API to your LLM. Schedule swift deliveries, manage your stores, and calculate routing fees.

## Description
Integrate **Dada Now (达达快送)**, one of the leading on-demand delivery platforms, tightly into your AI. With 10 full-scale fleet administration and logistics tools embedded, your AI model can function as an autonomous fleet coordinator for P2P deliveries.

### What you can do

- **Create Deliveries on the Fly** — Simply tell the AI where to send the goods and it will evaluate the `query_order_fee` alongside `add_order` instantly
- **Interactive Routing** — Add rider 'tips' during peak rush-hour dynamically, or complain against delays on the dashboard automatically
- **Store Management** — Create new delivery pickup hubs (Shop registration) directly via conversational prompts

### How it works

1. Sign up on the Dada Now Developer Program to receive an **App Key**, **App Secret**, and Merchant **Source ID**
2. Add them safely into Vurb
3. The backend encapsulates the required `MD5 Signature` rules alongside timestamps so your LLM doesn't have to navigate cryptography.

### Who is this for?

- **E-commerce Chatbots** — Directly dispatch local couriers from customer conversations without hitting backend servers
- **Operations Teams** — Give non-technical logistics staff the ability to control Dada dashboards via natural language


## Available Tools
- **add_complaint**: Submit a complaint about a driver
- **add_order**: Create a new Dada delivery order
- **add_shop**: Register a new Store/Shop to pick up from
- **add_tip**: Add a monetary tip to a specific delivery order
- **cancel_order**: Cancel a delivery dispatch
- **get_city_code**: Retrieve Dada City Codes
- **query_order_fee**: Estimate the delivery fee before ordering
- **query_order_status**: Get live tracking status of an order
- **readd_order**: Re-add an expired or failed delivery order
- **update_shop**: Update existing Station details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dada Now Delivery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the cost to deliver order JSON object `...` using Dada."

**🤖 AI Agent:**
> I requested the quote from the `query_order_fee` API. The estimated delivery toll is ¥ 12.00. Are we proceeding to dispatch?

---

**👤 You:**
> "Add a new store pickup point named 'Central Hub' at origin 'Shop1'."

**🤖 AI Agent:**
> The shop information has been effectively updated on the Dada Network API.


## ❓ FAQ

**Q: Is the MD5 signature abstracted?**
Yes! The parameters like `timestamp`, `app_key`, `v`, and `format` are automatically concatenated. The backend performs the `MD5` check and injects the `signature` transparently to the LLM context, yielding flawless delivery logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dada-now-delivery](https://vinkius.com/mcp/dada-now-delivery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dada Now Delivery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dada-now-delivery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dada Now Delivery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dada-now-delivery": {
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
