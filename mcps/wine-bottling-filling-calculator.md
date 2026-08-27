# Wine Bottling & Filling Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-bottling-filling-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate production timelines, material needs, and unit costs for wine bottling lines.

## Description
This MCP server provides specialized logistics and capacity planning for wine production. It connects AI agents to precise calculation tools for bottling operations. Use `get_production_timeline` to determine how long a run will take based on line speed and efficiency. Use `estimate_material_needs` to calculate required closures and inert gas for headspace displacement. Finally, use `calculate_operational_cost` and `get_case_metrics` to derive total production costs and cost per case.


## Available Tools (4)
- **calculate_operational_cost**: Estimates the total cost of a production run based on time and consumables
- **estimate_material_needs**: Calculates the quantity of closures and inert gas required for a production run
- **get_case_metrics**: Converts bottle-level production data into standard case-level logistics
- **get_production_timeline**: Determines how long it will take to meet a specific production target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Bottling & Filling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take to produce 5000 bottles if the line speed is 50 bottles per minute and efficiency is 85%?"

**🤖 AI Agent:**
> At an efficiency of 85%, your hourly output is 2550 bottles per hour. To produce 5000 bottles, it will take approximately 1.96 hours.

---

**👤 You:**
> "Calculate the material needs for 1000 bottles of 0.75L wine with a 0.7L fill height and a gas factor of 1.2."

**🤖 AI Agent:**
> For 1000 bottles, you will need 1000 closures (plus buffer) and 90 liters of inert gas.

---

**👤 You:**
> "What is the cost per case for 1200 bottles packed in cases of 12?"

**🤖 AI Agent:**
> With 1200 bottles packed 12 to a case, you will produce 100 cases. The cost per case is the total production cost divided by 100.


## ❓ FAQ

**Q: How do I calculate the time needed for a production run?**
You can use the `get_production_timeline` tool. Provide the target volume, the theoretical line speed, and the efficiency decimal to get the total hours required.

**Q: How is inert gas consumption calculated?**
The `estimate_material_needs` tool calculates gas requirements by determining the headspace volume (bottle size minus fill height) and applying a gas usage factor across the target volume.

**Q: Can I estimate the cost per case?**
Yes. Use `calculate_operational_cost` to find the total cost, then use `get_case_metrics` to convert that into the cost per case based on your bottles per case configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-bottling-filling-calculator](https://vinkius.com/ai-agent-connect/wine-bottling-filling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Bottling & Filling Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-bottling-filling-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Bottling & Filling Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-bottling-filling-calculator": {
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
