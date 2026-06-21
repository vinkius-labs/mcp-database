# 17Track MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/17track)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Global package tracking platform — monitor shipments across 1500+ carriers via AI.

## Description
Equip your AI agent with the most comprehensive logistics intelligence available via **17Track**. This unified server provides your agent with instant access to real-time shipment status, event history, and carrier metadata for over 1,500 global logistics providers. Your agent can instantly register new tracking numbers, audit shipping progress, and retrieve detailed event logs without you ever checking a tracking page. Whether you are managing e-commerce fulfillment or tracking personal orders, your agent acts as a dedicated logistics coordinator through natural conversation.

### What you can do

- **Shipment Monitoring** — Register and track thousands of packages simultaneously with real-time status updates.
- **Event Auditing** — Fetch complete historical logs and specific milestone events for any tracking number.
- **Carrier Intelligence** — Automatically detect the carrier for a given number and list all supported global providers.
- **Metadata Management** — Add tags and names to your shipments to keep your logistics organized.
- **Inventory Control** — Stop or delete tracking for completed shipments to maintain a clean dashboard.

### How it works

1. Subscribe to this server
2. Enter your 17Track API Key
3. Start managing your logistics intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Business Owners** — instantly monitor fulfillment status and customer shipment progress.
- **Logistics Managers** — audit carrier performance and track supply chain milestones through simple natural language.
- **Frequent Online Shoppers** — keep all their personal orders organized and get status updates in one place.
- **IT & Operations Teams** — integrate shipment tracking workflows into internal tools via an AI-guided interface.
- **Customer Support Agents** — retrieve real-time tracking data to resolve delivery inquiries faster.


## Available Tools
- **delete_tracking**: Delete a tracking number
- **detect_carrier**: Detect carrier for a number
- **get_tracking_info**: Get status for a tracking number
- **list_carriers**: List all supported carriers
- **register_tracking**: Register a new tracking number
- **stop_tracking**: Stop tracking a number
- **update_tracking_tag**: Update tracking metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **17Track** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register tracking number '123456789' for my order."

**🤖 AI Agent:**
> I've successfully registered tracking number '123456789'. I'll now monitor this shipment for you. Would you like to add a custom tag to identify this order?

---

**👤 You:**
> "Get the latest status for my package '123456789'."

**🤖 AI Agent:**
> Retrieving tracking info... Your package is currently 'In Transit'. The latest event was 'Arrived at Sort Facility' in Chicago yesterday at 2 PM. Should I notify you of any further changes?

---

**👤 You:**
> "Detect which carrier is handling tracking number 'XY123456789Z'."

**🤖 AI Agent:**
> Analyzing tracking format... Based on the number, this shipment is most likely being handled by 'China Post' or 'EMS'. I can use these IDs to register and start tracking it for you now.


## ❓ FAQ

**Q: Can I track packages from different carriers like DHL and FedEx at once?**
Yes! 17Track supports over 1,500 carriers. You can register any tracking number, and the `detect_carrier` tool can help identify which provider is handling the shipment.

**Q: How do I add a friendly name to a tracking number?**
Use the `update_tracking_tag` tool and provide the tracking number along with your desired text in the `tag` parameter. This makes it easier to identify shipments later.

**Q: What happens if I don't know the carrier ID?**
No problem. You can use the `detect_carrier` tool with the tracking number first. It will return the most likely carrier IDs, which you can then use to register the shipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/17track](https://vinkius.com/mcp/17track)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **17Track** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `17track` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **17Track** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "17track": {
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
