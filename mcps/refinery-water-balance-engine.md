# Refinery Water Balance Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-water-balance-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Models water mass balances, consumption, and recycling efficiency for refinery operations.

## Description
This MCP server provides specialized computational tools for modeling water mass balances in industrial refinery environments. It allows AI agents to quantify water consumption, calculate recycle rates, and estimate wastewater treatment requirements. By using tools like `get_system_water_balance` and `estimate_treatment_load`, agents can accurately model the entire water cycle, including cooling water losses and boiler water requirements, to ensure operational efficiency and environmental compliance.


## Available Tools (4)
- **get_system_water_balance**: 
- **get_total_water_consumption**: 
- **calculate_recycle_efficiency**: 
- **estimate_treatment_load**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Water Balance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total water consumption if intake is 1000, cooling loss is 50, and boiler loss is 30?"

**🤖 AI Agent:**
> The total water consumption is 80 units, with a net water loss of 80 units.

---

**👤 You:**
> "Calculate the recycle efficiency for 500 intake, 200 wastewater generated, and 150 treated water return."

**🤖 AI Agent:**
> The recycle rate is 30% and the recovery efficiency is 0.75.

---

**👤 You:**
> "Estimate the treatment load for 500 process water use, 400 wastewater generated, and a sludge factor of 0.1."

**🤖 AI Agent:**
> The required daily treatment capacity is 400 and the expected sludge volume is 40.


## ❓ FAQ

**Q: How can I calculate the total water lost in the system?**
You can use the `get_total_water_consumption` tool, providing the total water intake, cooling water loss, and boiler water loss.

**Q: Can this tool help with wastewater planning?**
Yes, the `estimate_treatment_load` tool predicts the required capacity for wastewater treatment plants and expected sludge volume.

**Q: Does it support full system modeling?**
Yes, the `get_system_water_balance` tool provides a comprehensive overview of the entire water cycle, including intake, consumption, recycle rate, and discharge volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-water-balance-engine](https://vinkius.com/en/ai-agent-connect/refinery-water-balance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Water Balance Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-water-balance-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Water Balance Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-water-balance-engine": {
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
