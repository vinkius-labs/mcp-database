# Wine Virtual Tasting Kit Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-virtual-tasting-kit-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate logistics, volume, and per-person pricing for virtual wine tasting kits.

## Description
This MCP server provides specialized tools for event planners and wine distributors to manage the logistics of virtual tasting events. It calculates total wine volume requirements using `calculate_wine_volume`, estimates packaging costs and weight with `estimate_packaging_needs`, determines shipping fees via `calculate_shipping_logistics`, and consolidates all data into a final per-person price using `generate_kit_pricing`. It helps balance the luxury of different tasting formats--from 50ml samples to full 750ml bottles--against shipping weights and costs.


## Available Tools (4)
- **estimate_packaging_needs**: Calculates the total cost and quantity of packaging materials required to secure the wine
- **generate_kit_pricing**: Consolidates all variables to provide the final per-person price for the virtual kit
- **calculate_wine_volume**: Determines the total amount of wine required for the entire group based on the chosen format
- **calculate_shipping_logistics**: Estimates the cost of transporting the kits to the event destination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Virtual Tasting Kit Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much wine do I need for 50 people if each person gets a 100ml pour?"

**🤖 AI Agent:**
> You will need a total of 5000ml of wine for 50 participants.

---

**👤 You:**
> "Calculate the total kit price for 20 people with a total wine cost of $400, packaging of $100, and shipping of $150."

**🤖 AI Agent:**
> The final price per kit is $32.50, and the total event cost is $650.00.

---

**👤 You:**
> "What is the total weight of packaging for 100 kits if each unit costs $2.50 to package?"

**🤖 AI Agent:**
> The total packaging cost is $250.00.


## ❓ FAQ

**Q: What volume options are supported for the tasting kits?**
The system supports three formats: 50ml (Micro Tier), 100ml (Standard Tier), and 750ml (Premium Tier).

**Q: How does the tool calculate the final price per person?**
The `generate_kit_pricing` tool sums the total wine cost, packaging cost, and shipping cost, then divides that total by the number of participants.

**Q: Can I estimate shipping costs for different regions?**
Yes, you can use `calculate_shipping_logistics` to estimate costs for the USA and Europe based on the total weight of the shipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-virtual-tasting-kit-sizing](https://vinkius.com/en/ai-agent-connect/wine-virtual-tasting-kit-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Virtual Tasting Kit Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-virtual-tasting-kit-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Virtual Tasting Kit Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-virtual-tasting-kit-sizing": {
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
