# Accessory Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessory-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Track and audit accessory quantities within shipments.

## Description
A specialized system for logistics and inventory management. Use `get_accessory_inventory` to monitor current stock levels, `log_accessory_arrival` to record new items, `get_shipment_summary` to view expected contents, and `verify_shipment_count` to perform audits and detect discrepancies in shipments.


## Available Tools (4)
- **get_accessory_inventory**: Retrieve the total count of all accessories currently recorded in the system
- **get_shipment_summary**: Retrieve a detailed breakdown of all accessories expected within a specific shipment
- **log_accessory_arrival**: Record the arrival of new accessories into the inventory
- **verify_shipment_count**: Compare the expected quantity of accessories for a specific shipment against the physically counted quantity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessory Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many cables are currently in the inventory?"

**🤖 AI Agent:**
> There are currently 150 cables in the inventory.

---

**👤 You:**
> "I just received 50 mounting brackets for shipment SHP-992. Please record this."

**🤖 AI Agent:**
> The arrival of 50 mounting brackets for shipment SHP-992 has been recorded. The inventory has been updated.

---

**👤 You:**
> "Verify shipment SHP-101. I counted 12 items physically."

**🤖 AI Agent:**
> The audit for shipment SHP-101 is complete. A discrepancy was detected: the expected count was 15, but only 12 were found.


## ❓ FAQ

**Q: How do I check the current stock of a specific accessory type?**
You can use the `get_accessory_inventory` tool and provide the specific accessory type as a filter.

**Q: What happens if the physical count doesn't match the shipment record?**
When you run `verify_shipment_count`, the system will return a discrepancy value and flag the audit status as 'Discrepancy Detected'.

**Q: Can I see what items are supposed to be in a shipment before counting them?**
Yes, use the `get_shipment_summary` tool with the relevant shipment ID to see the expected items and quantities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessory-count](https://vinkius.com/en/ai-agent-connect/accessory-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessory Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessory-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessory Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessory-count": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
