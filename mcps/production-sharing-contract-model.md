# Production Sharing Contract Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/production-sharing-contract-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Models the economic distribution of resources within a Production Sharing Contract (PSC).

## Description
This MCP server provides tools to model the economic distribution of resources in a Production Sharing Contract (PSC). It allows AI agents to calculate the breakdown of production between a state entity and a contractor. Key capabilities include using `calculate_period_economics` to determine cost oil and profit oil, `simulate_sliding_scale` to adjust splits based on production tiers, `apply_investment_credits` for depreciation and incentives, and `get_contractor_entitlement` to find the final volume claims.


## Available Tools (4)
- **apply_investment_credits**: Applies depreciation and specific investment incentives to recoverable costs
- **calculate_period_economics**: Calculates the economic breakdown of production for a specific period
- **get_contractor_entitlement**: Calculates the specific volume the contractor is allowed to claim
- **simulate_sliding_scale**: Simulates how the profit split changes as production progresses through different tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Production Sharing Contract Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the economics for a period with 1000 units of production, a 60% cost recovery limit, and a 50/50 profit split."

**🤖 AI Agent:**
> The cost oil is 600 units and the profit oil is 400 units. With a 50/50 split, the government receives 200 units and the contractor receives 200 units of profit oil.

---

**👤 You:**
> "What is the contractor's entitlement if cost oil is 500, profit oil is 500, and the contractor's profit split is 0.6?"

**🤖 AI Agent:**
> The contractor's total entitlement is 800 units (500 from cost oil and 300 from profit oil).

---

**👤 You:**
> "Apply a 5% investment credit to a base expenditure of 1000."

**🤖 AI Agent:**
> The total credit value is 50.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It models the economic distribution of resources in a Production Sharing Contract, calculating cost oil, profit oil, and entitlements.

**Q: How does the sliding scale work?**
You can use `simulate_sliding_scale` to determine how the profit split changes as production volume reaches different predefined thresholds.

**Q: Can I calculate the contractor's final share?**
Yes, the `get_contractor_entitlement` tool calculates the total volume the contractor is allowed to claim from both cost oil and profit oil.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/production-sharing-contract-model](https://vinkius.com/ai-agent-connect/production-sharing-contract-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Production Sharing Contract Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `production-sharing-contract-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Production Sharing Contract Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "production-sharing-contract-model": {
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
