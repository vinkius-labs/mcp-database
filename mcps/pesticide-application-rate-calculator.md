# Pesticide Application Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pesticide-application-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise pesticide dosages, sprayer settings, and tank mix compatibility.

## Description
This MCP server provides precision tools for agricultural spraying operations. It allows AI agents to calculate exact product dosages using `calculate_dosage`, determine sprayer equipment settings like tractor speed or nozzle flow with `calculate_equipment_settings`, verify chemical safety using `check_tank_mix_compatibility`, and plan logistics with `calculate_tank_mix_volume`.


## Available Tools (4)
- **calculate_dosage**: Determines the exact amount of a specific pesticide product needed to meet a target application rate
- **calculate_equipment_settings**: Calculates the required tractor speed or nozzle flow to achieve a specific spray volume
- **calculate_tank_mix_volume**: Determines the total volume of product and water needed for a specific tank size
- **check_tank_mix_compatibility**: Evaluates if a list of pesticide products can be safely mixed in a single tank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pesticide Application Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much product do I need if I want 50g of active ingredient per hectare, the product is 25% concentration, and I'm applying 200L/ha?"

**🤖 AI Agent:**
> You need 200 liters of product per hectare.

---

**👤 You:**
> "What speed should I drive if my boom is 15m wide, I have 5 nozzles at 0.5 L/min each, and I want to apply 300 L/ha?"

**🤖 AI Agent:**
> You should drive at 5.0 km/h.

---

**👤 You:**
> "Can I mix Product_A and Product_B in the same tank?"

**🤖 AI Agent:**
> No, Product_A and Product_B are incompatible and may cause precipitation if mixed.


## ❓ FAQ

**Q: How do I calculate the amount of product needed for my field?**
You can use the `calculate_dosage` tool by providing the target active ingredient rate, the product concentration, and the desired spray volume per hectare.

**Q: Can I check if two chemicals can be mixed together?**
Yes, use the `check_tank_mix_compatibility` tool with a list of product IDs to verify if they are safe to mix in a single tank.

**Q: How do I adjust my sprayer speed for a specific volume?**
The `calculate_equipment_settings` tool calculates the necessary tractor speed or nozzle flow rate based on your boom width and target spray volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pesticide-application-rate-calculator](https://vinkius.com/ai-agent-connect/pesticide-application-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pesticide Application Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pesticide-application-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pesticide Application Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pesticide-application-rate-calculator": {
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
