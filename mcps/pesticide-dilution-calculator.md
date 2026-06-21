# Pesticide Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pesticide-dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise pesticide dilution, tank loads, and safety intervals.

## Description
This MCP server provides specialized tools for agricultural precision. Use `calculate_mixing_ratio` to determine the exact amount of product and water needed per tank, `calculate_total_deployment` to plan logistics like total tanks and cost per hectare, and `lookup_safety_warnings` to retrieve critical pre-harvest interval (PHI) data based on active ingredients.


## Available Tools
- **calculate_mixing_ratio**: Determines the precise composition of a single spray tank load
- **lookup_safety_warnings**: Retrieves essential safety and compliance information based on the chemical used
- **calculate_total_deployment**: Calculates the total logistics required for treating a large-scale area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pesticide Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much product should I add to a 500L tank if the dose is 200ml/ha and spray volume is 200L/ha?"

**🤖 AI Agent:**
> You should add 500ml of product to the tank, with 499.5L of water.

---

**👤 You:**
> "Calculate total tanks and cost for 50 hectares at 200L/ha dose 200ml/ha with unit price 0.05."

**🤖 AI Agent:**
> You will need 50 tanks, a total volume of 10,000L, and the cost per hectare is 10.0.

---

**👤 You:**
> "What is the safety interval for atrazine?"

**🤖 AI Agent:**
> The pre-harvest interval for atrazine is 30 days.


## ❓ FAQ

**Q: How do I calculate the amount of product per tank?**
Use the `calculate_mixing_ratio` tool by providing the recommended dose, spray volume per hectare, and your tank capacity.

**Q: Can I calculate total costs for a large area?**
Yes, the `calculate_total_deployment` tool calculates the number of tanks required and the cost per hectare based on your total area.

**Q: How do I find safety intervals for specific chemicals?**
Use the `lookup_safety_warnings` tool with the name of the active ingredient to find the required pre-harvest interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pesticide-dilution-calculator](https://vinkius.com/mcp/pesticide-dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pesticide Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pesticide-dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pesticide Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pesticide-dilution-calculator": {
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
