# Soil Amendment Purchase Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/soil-amendment-purchase-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculates amendment mass, net purchase needs, and optimized package selections.

## Description
This MCP server provides a complete logistical workflow for soil amendment planning. It converts spatial measurements into physical mass requirements using `calculate_mass_requirement`, determines the actual amount to buy via `calculate_net_purchase_needs` by accounting for existing stock, and optimizes logistics with `optimize_package_selection` to find the most efficient package combinations. Finally, it ensures orders meet supplier constraints using `validate_delivery_eligibility`.


## Available Tools (4)
- **calculate_mass_requirement**: Determines the total mass of amendment needed for a specific plot
- **calculate_net_purchase_needs**: Calculates how much more amendment must be bought after accounting for current inventory
- **optimize_package_selection**: Translates a mass requirement into specific numbers of commercial packages
- **validate_delivery_eligibility**: Checks if the planned purchase meets the logistical constraints of the supplier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil Amendment Purchase Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 500 square meter plot and need 0.5 kg of amendment per square meter. The bulk density is 1.2 kg/L. How much mass and volume do I need?"

**🤖 AI Agent:**
> You need a total mass of 250 kg, which corresponds to a volume of 208.33 liters.

---

**👤 You:**
> "I need 100 kg of amendment. I already have 30 kg in my shed. How much more do I need to buy?"

**🤖 AI Agent:**
> You need to purchase an additional 70 kg of amendment.

---

**👤 You:**
> "I need to buy 45 kg of amendment. Available bag sizes are 5kg, 10kg, and 25kg. What is the best package combination?"

**🤖 AI Agent:**
> The optimal selection is one 25kg bag and two 10kg bags, totaling 45kg using 3 packages.


## ❓ FAQ

**Q: How does the tool calculate the total mass needed?**
The `calculate_mass_requirement` tool calculates mass by multiplying the plot area by the application rate, then derives volume using the provided bulk density.

**Q: Can I account for the soil amendments I already have in stock?**
Yes, use `calculate_net_purchase_needs` to subtract your current stock mass from the total requirement to find the net amount to purchase.

**Q: How does the system handle different bag sizes?**
The `optimize_package_selection` tool uses a greedy approach to select the combination of available package sizes that satisfies your needs using the fewest total packages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/soil-amendment-purchase-planner](https://vinkius.com/en/ai-agent-connect/soil-amendment-purchase-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil Amendment Purchase Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-amendment-purchase-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil Amendment Purchase Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-amendment-purchase-planner": {
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
