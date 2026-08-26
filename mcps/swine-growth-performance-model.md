# Swine Growth Performance Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/swine-growth-performance-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict swine growth metrics, production costs, and optimal market weight using NRC equations.

## Description
This MCP server provides advanced biological and economic modeling for swine production. By applying National Research Council (NRC) standards, it allows AI agents to calculate critical performance indicators such as average daily gain and feed conversion ratio using `predict_growth_metrics`. Users can estimate financial requirements with `estimate_production_costs`, identify the most profitable selling point via `find_optimal_market_weight`, and evaluate how heat stress affects development through `simulate_environmental_impact`. It is designed to optimize market timing and maximize profitability in swine operations.


## Available Tools (4)
- **estimate_production_costs**: Calculates the financial cost associated with reaching a specific target weight
- **find_optimal_market_weight**: Determines the most profitable weight to sell the animal based on economic variables
- **predict_growth_metrics**: Calculates primary physiological performance indicators for a specific growth window
- **simulate_environmental_impact**: Evaluates how different thermal conditions will shift the performance timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swine Growth Performance Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the growth metrics for a 20kg barrow with a target weight of 100kg, using a high-performance genotype and a diet with 3.2 energy density and 0.8 lysine."

**🤖 AI Agent:**
> The predicted average daily gain is 0.85 kg/day, the feed conversion ratio is 2.4, and it will take 94 days to reach the target weight.

---

**👤 You:**
> "What is the optimal market weight for a gilt starting at 25kg, assuming a feed cost of $0.40/kg and a market price of $2.10/kg?"

**🤖 AI Agent:**
> The optimal market weight is 112 kg, with an expected profit of $145.50.

---

**👤 You:**
> "How will an ambient temperature of 35 degrees Celsius affect the growth of a 50kg boar?"

**🤖 AI Agent:**
> The high temperature triggers thermal stress, resulting in a 15% reduction in growth speed.


## ❓ FAQ

**Q: How does the model account for heat stress?**
The `simulate_environmental_impact` tool evaluates thermal conditions. If temperatures exceed the thermoneutral zone, the model applies a reduction factor to growth rates and increases the feed conversion ratio.

**Q: Can I find the most profitable weight to sell my swine?**
Yes, you can use `find_optimal_market_weight` to determine the specific weight that maximizes profit by balancing weight value against feed costs and efficiency.

**Q: What biological models are used for growth?**
The model utilizes non-linear Gompertz and Bridging growth curves based on NRC standards to accurately represent biological development.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/swine-growth-performance-model](https://vinkius.com/ai-agent-connect/swine-growth-performance-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swine Growth Performance Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swine-growth-performance-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swine Growth Performance Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swine-growth-performance-model": {
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
