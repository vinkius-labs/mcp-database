# Flexport MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flexport)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage global freight shipments, purchase orders, and logistics documents via AI agents with Flexport.

## Description
Connect your **Flexport** account to any AI agent and automate your global trade and freight operations through the Model Context Protocol (MCP). Flexport is the modern freight forwarder that provides full visibility and control over your supply chain. Now, you can track shipments, manage purchase orders, and retrieve essential logistics documentation directly through natural conversation.

### What you can do

- **Shipment Tracking** — List all your ocean and air shipments, fetch detailed tracking metadata, and monitor transit statuses in real-time.
- **PO Management** — Automate your purchase order lifecycle by listing, retrieving, and creating POs directly from the agent.
- **Document Retrieval** — List and fetch essential logistics documents such as Bills of Lading, Commercial Invoices, and Packing Lists.
- **Billing & Invoices** — Access freight and commercial invoices associated with your account or specific shipments for better financial oversight.
- **Customs Documentation** — Retrieve commercial invoice data required for customs clearance and compliance reporting.
- **Global Visibility** — Get a high-level overview of your entire global supply chain operations without switching tabs.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flexport API Key (found in your Flexport Developer Portal)
3. Start managing your global freight operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Managers** — quickly check shipment statuses and cargo ready dates while coordinating with carriers.
- **Supply Chain Analysts** — get a real-time overview of purchase orders and invoices through simple AI commands.
- **Finance Operations** — automate the retrieval of freight billing data and documents for audit and reconciliation.


## Available Tools (12)
- **list_commercial_invoices**: List commercial invoices
- **list_documents**: List logistics documents
- **list_invoices**: List freight invoices
- **list_purchase_orders**: List purchase orders
- **list_shipment_invoices**: List invoices for shipment
- **list_shipments**: List freight shipments
- **create_purchase_order**: Create a new purchase order
- **download_document**: Get document download link
- **get_document**: Get document metadata
- **get_invoice**: Get invoice details
- **get_purchase_order**: Get purchase order details
- **get_shipment**: Get shipment details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flexport** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent freight shipments and their status."

**🤖 AI Agent:**
> Fetching shipments... I found 5 recent shipments, including 'SHIP-123' (In Transit - Ocean) and 'SHIP-456' (Arrival - Air). Would you like the tracking details or associated documents for any of these?

---

**👤 You:**
> "Show me all purchase orders pending for this quarter."

**🤖 AI Agent:**
> Retrieving purchase orders... You have 8 active POs, with 3 marked as 'Pending Vendor Confirmation'. Would you like me to drill down into the line items for these pending orders?

---

**👤 You:**
> "Get the download link for the Bill of Lading for shipment 'SHIP-789'."

**🤖 AI Agent:**
> Generating document link... I've retrieved a secure temporary link for the Bill of Lading associated with SHIP-789. You can download the file here: https://api.flexport.com/documents/doc_abc/download.


## ❓ FAQ

**Q: How do I track a specific shipment using its ID?**
You can use the 'get_shipment' tool and provide the Flexport Shipment ID. The agent will return the most recent status, location, and estimated arrival dates for that shipment.

**Q: Can I retrieve commercial invoices for customs purposes?**
Yes! The 'list_commercial_invoices' and 'list_documents' tools allow you to access the necessary paperwork for customs clearance. You can even use 'download_document' to get a temporary link to the actual file.

**Q: Is it possible to filter invoices by shipment?**
Absolutely. Use the 'list_shipment_invoices' tool and provide the Shipment ID. The agent will retrieve all freight billing documents associated with that specific cargo movement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flexport](https://vinkius.com/mcp/flexport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flexport** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flexport` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flexport** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flexport": {
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
