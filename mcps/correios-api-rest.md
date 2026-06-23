# Correios API (REST) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/correios-api-rest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Track Brazilian postal objects and calculate shipping prices and deadlines directly through the official Correios REST API.

## Description
Connect your AI agent to the **Correios** infrastructure to automate logistics queries in Brazil. This server provides direct access to the official REST API for real-time tracking and shipping simulations.

### What you can do

- **Object Tracking** — Get the full history of events and current status for any valid tracking code (e.g., AA123456789BR) using the `track_object` tool.
- **Shipping Calculation** — Simulate prices and delivery deadlines for various services like SEDEX and PAC based on weight, dimensions, and zip codes with `calculate_price_deadline`.
- **Logistics Automation** — Integrate shipping data into your e-commerce or support workflows without manual lookups.

### How it works

1. Subscribe to this server
2. Enter your Correios API credentials (User and Password)
3. Start querying logistics data from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly check delivery statuses for customers and provide proactive updates.
- **Logistics Managers** — automate shipping cost estimations for different regions in Brazil directly from the terminal or chat.
- **Support Teams** — provide instant tracking updates within AI-powered chat interfaces without leaving the conversation.


## Available Tools (2)
- **calculate_price_deadline**: Uses POST but acts as a query.

Calculate shipping price and deadline
- **track_object**: Track a postal object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Correios API (REST)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track the object with code NL123456789BR."

**🤖 AI Agent:**
> I've checked the status for NL123456789BR. It was posted on Oct 24th and is currently 'In Transit' to the distribution center in São Paulo.

---

**👤 You:**
> "Calculate SEDEX shipping from 01001-000 to 22041-001 for a 500g box (20x15x10cm)."

**🤖 AI Agent:**
> Using `calculate_price_deadline`, the estimated price for SEDEX is R$ 24.50 with a delivery deadline of 1 business day.

---

**👤 You:**
> "What is the current status of my package AA987654321BR?"

**🤖 AI Agent:**
> The package AA987654321BR was 'Delivered' today at 2:30 PM in Curitiba.


## ❓ FAQ

**Q: What information do I need to calculate a shipping price?**
You need to provide the origin and destination ZIP codes (CEP), the service code (e.g., 04014 for SEDEX), weight, package format, and dimensions (length, height, width) using the `calculate_price_deadline` tool.

**Q: Can I track multiple objects at once?**
The `track_object` tool currently processes one tracking code per request to ensure detailed event history for that specific item.

**Q: What is the 'idLote' field in the shipping calculation?**
The `idLote` (Batch ID) is a required identifier for the Correios API request. It can be any string or number used to identify your specific calculation request in their logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/correios-api-rest](https://vinkius.com/mcp/correios-api-rest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Correios API (REST)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `correios-api-rest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Correios API (REST)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "correios-api-rest": {
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
