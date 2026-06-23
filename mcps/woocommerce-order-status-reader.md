# WooCommerce Order Status Reader MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-order-status-reader)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

This MCP gives your AI agent the ability to check the real-time status and tracking information of any WooCommerce order using an Order ID or a Customer Email. Perfect for automating "where is my order?" (WISMO) support queries.

## Description
Empower your AI customer support bots to instantly answer the most common e-commerce question: "Where is my order?". This MCP provides a highly restricted, read-only bridge to your WooCommerce store.

### The Superpowers

- **Instant WISMO Resolution:** The AI can look up an order by its exact ID, or search for the most recent orders using just the customer's email address.
- **Zero-Trust Safety:** This is a strictly read-only tool. The agent cannot modify the order, cannot issue refunds, and cannot read orders belonging to other customers unless explicitly asked for that email.
- **Tracking Extraction:** It automatically parses WooCommerce's `_tracking_number` meta data so the AI can provide tracking links and shipping method details directly to the customer.


## Available Tools (1)
- **read_woocommerce_order**: You must provide either the specific orderId or the customer's email address to search for recent orders.

Reads the real-time status of a WooCommerce order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WooCommerce Order Status Reader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A customer is asking for the status of order #10452. Can you check it for them?"

**🤖 AI Agent:**
> I've checked the status of Order #10452. It is currently **COMPLETED** and was shipped via FedEx. The tracking number is 1Z9999999999999999.


## ❓ FAQ

**Q: Can the AI issue refunds with this tool?**
No. This MCP only calls the `GET` endpoint for orders. It is physically impossible for the AI to alter an order status or issue a refund using this server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-order-status-reader](https://vinkius.com/mcp/woocommerce-order-status-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WooCommerce Order Status Reader** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `woocommerce-order-status-reader` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WooCommerce Order Status Reader** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woocommerce-order-status-reader": {
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
