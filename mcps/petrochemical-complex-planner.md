# Petrochemical Complex Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petrochemical-complex-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimize product slates, unit capacities, and feedstock mixes for integrated petrochemical complexes.

## Description
This MCP server provides specialized tools for modeling integrated petrochemical value chains. It allows AI agents to calculate the most profitable product mix using `plan_product_slate`, verify if production targets are physically possible with `validate_unit_capacities`, and quantify the economic gains of byproduct reuse via `calculate_integration_benefits`. Additionally, it helps minimize costs by identifying the ideal feedstock combination through `optimize_feedstock_mix`.


## Available Tools (4)
- **optimize_feedstock_mix**: Identifies the best combination of different feedstock types to minimize costs while meeting production targets
- **validate_unit_capacities**: Checks if a proposed product slate is physically achievable given the constraints of the plant equipment
- **calculate_integration_benefits**: Quantifies the economic advantage of using byproducts within the complex instead of selling them as standalone products
- **plan_product_slate**: Determines the most profitable mix of products based on current market conditions and feedstock constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petrochemical Complex Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the most profitable product mix for 1000 units of Naphtha given Ethylene is $800 and Propylene is $600?"

**🤖 AI Agent:**
> The optimal product slate consists of 600 units of Ethylene and 400 units of Propylene, yielding a total value of $680,000.

---

**👤 You:**
> "Is it possible to produce 500 units of Ethylene if my primary cracker has a capacity of 450 units?"

**🤖 AI Agent:**
> No, the production plan is infeasible because the required throughput exceeds the capacity of the primary cracker.

---

**👤 You:**
> "What is the benefit of using byproduct Ethane as feedstock instead of selling it?"

**🤖 AI Agent:**
> Integrating the byproduct Ethane as feedstock provides a net benefit of $50,000 compared to selling it at market price.


## ❓ FAQ

**Q: How can I determine the best product mix?**
You can use the `plan_product_slate` tool, which analyzes feedstock availability, market prices, and demand limits to find the most profitable combination of products.

**Q: Can I check if my production plan is feasible?**
Yes, the `validate_unit_capacities` tool checks your proposed product volumes against the physical limits of your plant equipment to identify potential bottlenecks.

**Q: How do I calculate the value of integrating byproducts?**
Use the `calculate_integration_benefits` tool to compare the value of selling byproducts as standalone items versus using them as feedstocks for other units.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petrochemical-complex-planner](https://vinkius.com/en/ai-agent-connect/petrochemical-complex-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petrochemical Complex Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petrochemical-complex-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petrochemical Complex Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petrochemical-complex-planner": {
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
