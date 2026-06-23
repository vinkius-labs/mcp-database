# Metrc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metrc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Cannabis track-and-trace via Metrc — track facilities, items, plants, and harvests.

## Description
Connect your **Metrc** account to any AI agent and take full control of your cannabis track-and-trace compliance through natural conversation.

### What you can do

- **Facility Oversight** — List all licensed facilities and fetch detailed metadata for your operations
- **Inventory Tracking** — Retrieve active items, strains, and inventory packages with real-time status visibility
- **Supply Chain Management** — Monitor plant life cycles, harvest batches, and incoming inventory transfers securely
- **Compliance Auditing** — List active sales receipts and verify unit of measure configurations
- **Detailed Inspection** — Fetch comprehensive metadata for individual packages and state-specific license configurations

### How it works

1. Subscribe to this server
2. Enter your state-specific Metrc Base URL, Integrator Key, and User Key
3. Start managing your compliance data from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_package_details**: Get details for a specific package
- **get_unit_of_measures**: g. Grams, Ounces).

List all units of measure
- **list_facilities**: List all licensed facilities
- **list_active_harvests**: List active harvests for a facility
- **list_active_items**: List active items for a facility
- **list_active_packages**: List active packages for a facility
- **list_tracked_plants**: List tracked plants for a facility
- **list_active_sales**: List active sales receipts
- **list_active_strains**: List active strains for a facility
- **list_incoming_transfers**: List incoming inventory transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metrc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active facilities associated with my Metrc account."

**🤖 AI Agent:**
> Retrieving facilities... I found 2 licensed facilities: 'Green Valley Cultivation' and 'Downtown Distribution Center'.

---

**👤 You:**
> "Show active inventory packages for license 'LIC-12345'."

**🤖 AI Agent:**
> Querying inventory... I identified 15 active packages, including 10 units of 'Blue Dream' flower and 5 units of 'OG Kush' concentrates.

---

**👤 You:**
> "Get details for package label 'ABCDEFG1234567'."

**🤖 AI Agent:**
> Inspecting package... Label 'ABCDEFG1234567' contains 500g of bulk flower, currently in 'Active' status at your primary facility.


## ❓ FAQ

**Q: How do I find my Metrc API Keys?**
Your Integrator Key is provided by your software vendor. Your User Key is found in your Metrc User Profile under the 'API Keys' section.

**Q: Which Base URL should I use?**
You must use the API URL corresponding to your state (e.g., https://api-ca.metrc.com for California).

**Q: Is my regulatory data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metrc](https://vinkius.com/mcp/metrc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metrc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metrc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metrc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metrc": {
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
