# CPSC (Consumer Product Safety Commission) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cpsc-consumer-product-safety-commission)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Access official consumer product recall data — search by product, hazard, manufacturer, or date to ensure safety and compliance.

## Description
Connect to the **Consumer Product Safety Commission (CPSC)** database to monitor product safety and recalls through natural conversation.

### What you can do

- **Recall Search** — Search the entire database using keywords, product names, or specific recall numbers.
- **Hazard Filtering** — Identify products recalled for specific risks like fire, choking, or lead exposure.
- **Manufacturer Tracking** — Query recalls associated with specific brands or manufacturers.
- **UPC & Model Verification** — Check if a specific product model or UPC is under an active recall notice.
- **Date Range Queries** — Filter results to see the most recent safety alerts or historical data.

### How it works

1. Subscribe to this server
2. No authentication is required for this public government API
3. Start querying safety data from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — verify product safety against official government records.
- **Retailers & E-commerce** — ensure inventory does not contain recalled items.
- **Concerned Parents & Consumers** — quickly check household items for safety hazards.


## Available Tools
- **search_recalls**: The API is public and requires no authentication.

Search for CPSC consumer product recalls


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CPSC (Consumer Product Safety Commission)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recalls involving 'fire' hazards from the last year."

**🤖 AI Agent:**
> I've searched the CPSC database for fire-related recalls in 2023-2024. I found 12 active notices, including portable heaters and certain lithium-ion battery packs. Would you like the details for a specific product?

---

**👤 You:**
> "Are there any active recalls for 'Fisher-Price' products?"

**🤖 AI Agent:**
> Querying CPSC for 'Fisher-Price'... I found several historical and recent recalls. The most recent involves certain baby gliders and sleepers. I can provide the specific recall numbers and remedies for these items.

---

**👤 You:**
> "Check if there are any recalls for product model 'XYZ123'."

**🤖 AI Agent:**
> I am checking the database for model 'XYZ123'. No active recalls were found for this specific model number in the CPSC records. Would you like me to search by the manufacturer name instead?


## ❓ FAQ

**Q: Can I filter recalls by a specific hazard type like 'Fire' or 'Choking'?**
Yes! Use the `search_recalls` tool and provide the hazard keyword in the `Hazard` parameter. The agent will return all matching products associated with that specific risk.

**Q: Is it possible to search for recalls from a specific manufacturer or brand?**
Absolutely. You can use the `Manufacturer` parameter in the `search_recalls` tool to list all safety notices issued for products from a particular company.

**Q: Can I search for a recall using a specific Product UPC?**
Yes, the `search_recalls` tool includes a `ProductUPC` field. This allows for precise identification of specific items that may be subject to safety recalls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cpsc-consumer-product-safety-commission](https://vinkius.com/mcp/cpsc-consumer-product-safety-commission)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CPSC (Consumer Product Safety Commission)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cpsc-consumer-product-safety-commission` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CPSC (Consumer Product Safety Commission)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cpsc-consumer-product-safety-commission": {
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
