# Appliance Sale Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/appliance-sale-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare appliance total cost of ownership, energy costs, and rebates.

## Description
This MCP server provides tools to evaluate the true cost of household appliances. Instead of looking only at the sticker price, you can use `calculate_tco` to determine the total cost of ownership, including energy consumption and installation. You can also use `compare_appliances` to find the most cost-effective models, `get_appliance_details` for technical specs, and `get_rebate_eligibility` to find local incentives.


## Available Tools (4)
- **compare_appliances**: Performs a side-by-side comparison of multiple appliances to identify the most cost-effective option
- **get_appliance_details**: Retrieves core technical and pricing specifications for a specific appliance model
- **get_rebate_eligibility**: Checks which rebates apply to a specific appliance to determine the actual net purchase price
- **calculate_tco**: Calculates the total cost of ownership for a single appliance over its entire lifespan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appliance Sale Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost of ownership for appliance ID 'fridge-123' if energy costs $0.15 per kWh?"

**🤖 AI Agent:**
> The total cost of ownership for fridge-123 is $1,250.00, which includes a net purchase price of $800.00, $150.00 for installation, and $300.00 in energy costs over its lifespan.

---

**👤 You:**
> "Compare 'washer-99' and 'washer-100' with an energy rate of $0.20 per kWh."

**🤖 AI Agent:**
> The most cost-effective option is washer-100, with a total cost of ownership of $650.00 compared to $720.00 for washer-99.

---

**👤 You:**
> "Are there any rebates for 'dishwasher-55' in the USA?"

**🤖 AI Agent:**
> Yes, dishwasher-55 is eligible for the USA Federal Energy Rebate of $50.00.


## ❓ FAQ

**Q: How is the total cost calculated?**
The total cost is the sum of the sticker price (minus rebates), installation fees, and the cumulative cost of energy over the appliance's expected lifespan.

**Q: Can I compare multiple appliances at once?**
Yes, you can use the `compare_appliances` tool to perform a side-by-side comparison of several models to find the winner.

**Q: What regions are supported for rebates?**
Currently, `get_rebate_eligibility` supports the USA and Europe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/appliance-sale-comparator](https://vinkius.com/en/ai-agent-connect/appliance-sale-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appliance Sale Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appliance-sale-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appliance Sale Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appliance-sale-comparator": {
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
