# Shippo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shippo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Get the best shipping rates from top carriers, print labels, and track deliveries with an API that simplifies e-commerce shipping.

## Description
Connect your **Shippo** account to any AI agent and take full control of your global shipping and logistics orchestration through natural conversation. Shippo provides a powerful API for comparing shipping rates across multiple carriers, generating labels, and tracking packages directly from your chat interface.

### What you can do

- **Rate & Shipment Orchestration** — Compare real-time shipping rates from various carriers and create shipments programmatically.
- **Label Lifecycle Management** — Generate shipping labels and manage transactions directly from the AI interface to streamline your fulfillment.
- **Tracking Intelligence** — Retrieve real-time tracking information for any package by carrier and tracking number via natural language.
- **Address Validation Control** — Create and validate sender and recipient addresses to ensure your deliveries are always accurate.
- **Operational Oversight** — Access carrier accounts, manage customs declarations, and monitor manifest metadata to maintain a clear overview of your logistics.

### How it works

1. Subscribe to this server
2. Enter your Shippo API Token from your dashboard
3. Start managing your shipping operations from Claude, Cursor, or any MCP-compatible client

No more manual address checking or rate hunting. Your AI acts as a dedicated shipping clerk or logistics manager.

### Who is this for?

- **E-commerce Business Owners** — quickly compare shipping costs and generate labels without switching between carrier sites.
- **Fulfillment Teams** — automate the retrieval of tracking statuses and monitor customs documents via natural conversation.
- **Developers** — integrate multi-carrier shipping capabilities into custom AI-driven business workflows.


## Available Tools (12)
- **check_api_health**: Verify Shippo API connectivity
- **create_and_validate_address**: Required for shipments.

Add a new shipping address
- **create_shipment_get_rates**: Get real-time shipping rates
- **purchase_shipping_label**: Purchase and generate a label
- **track_package_status**: Track a shipment in real-time
- **list_saved_addresses**: List saved shipping addresses
- **list_connected_carriers**: ) linked to your Shippo profile.

List active carrier accounts
- **list_customs_declarations**: List customs declarations
- **list_customs_items**: List international customs items
- **list_carrier_manifests**: List daily carrier manifests
- **list_recent_shipments**: List recent shipping requests
- **list_purchased_labels**: List all shipping transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shippo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the tracking status for USPS package 1234567890."

**🤖 AI Agent:**
> I've retrieved the tracking info. Your USPS package is currently 'In Transit' and is expected to be delivered by tomorrow, June 15th. Would you like to see the full milestone history?

---

**👤 You:**
> "List all my active carrier accounts in Shippo."

**🤖 AI Agent:**
> Retrieving carrier accounts... You have 4 active accounts configured: FedEx, UPS, DHL, and USPS. Would you like to check the settings for any of them?

---

**👤 You:**
> "Validate this address: 123 Main St, San Francisco, CA 94105."

**🤖 AI Agent:**
> Processing address validation... The address is valid and identified as a commercial location. Should I use it to get shipping rates for your next package?


## ❓ FAQ

**Q: Can my AI automatically find the tracking status for a package using only the carrier and tracking number?**
Yes! Use the `get_tracking` tool. Provide the carrier name (e.g., 'usps', 'fedex') and the tracking number, and your agent will return the real-time status and estimated delivery date.

**Q: How do I compare shipping rates for a new shipment?**
Simply ask the agent to run the `create_shipment` action with the package details and addresses. It will retrieve and compare pricing from all configured carrier accounts.

**Q: How do I find my Shippo API Token?**
Log in to your Shippo account, navigate to **Settings** > **API**, and you will find your unique Live or Test API Token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shippo](https://vinkius.com/mcp/shippo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shippo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shippo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shippo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shippo": {
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
