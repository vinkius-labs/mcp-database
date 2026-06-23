# Walmart Drop Ship Vendor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/walmart-drop-ship-vendor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Exclusive 1P Supplier logistics server. Map DSV operations like Lag Times and physical supply nodes securely.

## Description
### What you can do

Take complete proxy logistics control explicitly handling 1P Walmart Supplier structures:

- **Process 1P DSV Orders:** Efficiently poll orders required to be shipped on behalf of Walmart as Seller of Record.
- **Update Fulfillment Lag Times:** Seamlessly track node latency dynamically updating transit delay variables.
- **Manage Node Inventories:** Actuate precise stock counts representing your supply chain warehouse locations.
- **Print Packing Slips:** Extract packing directives needed explicitly for handling supplier boxes.

### How it works

1. **Define Security Scope:** The server acts solely through the `/v3/dsv` endpoints directly linking to 1P Walmart internal catalogs.
2. **Submit Advance Notices:** The system provides built-in ASN generators notifying distribution immediately.
3. **Map Carrier Logistics:** Manage preferred logistics partners with accuracy.

### Who is this for?

Specifically built for **1P Suppliers**, **Drop Ship Vendors**, and large scalable **Fulfillment Nodes**.


## Available Tools (8)
- **dsv_cancel_lines**: Cancel DSV explicitly parsing unfulfilled constraints isolating cleanly 1P seller structures natively
- **dsv_check_node_status**: Poll safely logical Node arrays checking completely if the 1P distribution centers bounds are running efficiently
- **dsv_get_orders**: Extract actively explicitly created Drop Ship Vendor orders resolving native structured logs inherently cleanly
- **dsv_get_packing_slips**: Extract packing arrays compiling explicit 1P documents cleanly generating accurate warehouse tracking constraints
- **dsv_manage_inventory**: Allocate physical 1P logistic stock actively pushing exact constraints explicitly
- **dsv_route_shipments**: Verify explicitly local transport carriers ensuring correctly routed bounds targeting accurate node paths natively
- **dsv_submit_asn**: Execute advance shipping notices mapping the physical tracking updates tracing supplier shipments natively
- **dsv_update_lag_time**: Execute tracking updates bounding fulfillment lag days parsing supplier node latency accurately explicitly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Walmart Drop Ship Vendor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check active and unfulfilled DSV sales orders."

**🤖 AI Agent:**
> Query completed. Exported currently unfulfilled packaging arrays efficiently.

---

**👤 You:**
> "Summarize the current Lag Times for facility ID 'WH-EAST'."

**🤖 AI Agent:**
> Based on your query, the current default Lag Time for physical node 'WH-EAST' is configured to 2 days before mandatory shipment.

---

**👤 You:**
> "Prepare an Advanced Shipping Notice (ASN) for package PLT-444 containing 5 units of SKU-10."

**🤖 AI Agent:**
> ASN Generated successfully. Package PLT-444 is registered in transit and the DSV dashboard has been updated.


## ❓ FAQ

**Q: Does this MCP server work for standard 3P Marketplace Sellers?**
No. This server natively accesses ONLY the Drop Ship Vendor `/v3/dsv` endpoints explicitly. If you are 3P, use `walmart-orders-mcp`.

**Q: What does updating the Lag Time mean for my DSV account?**
Lag Time defines the number of days between an order being placed and shipped. This agent allows you to adjust it dynamically to prevent late shipment penalties during high volume.

**Q: Can I generate advanced shipping notices (ASNs) with this tool?**
Yes, you can properly inform Walmart's fulfillment network by creating standard DSV ASN payloads seamlessly via this interface before trucks leave the warehouse.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/walmart-drop-ship-vendor](https://vinkius.com/mcp/walmart-drop-ship-vendor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Walmart Drop Ship Vendor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `walmart-drop-ship-vendor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Walmart Drop Ship Vendor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "walmart-drop-ship-vendor": {
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
