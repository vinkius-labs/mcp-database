# Portfolio Weight Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/portfolio-weight-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate asset weights, concentration risk, and rebalancing needs.

## Description
This MCP server provides precise financial calculation tools for managing investment portfolios. It allows AI agents to determine the exact weight of an asset using `get_asset_weight`, identify concentration risks with `get_portfolio_concentration`, verify the mathematical consistency of a portfolio via `validate_portfolio_composition`, and calculate necessary trades using `calculate_rebalancing_requirement`.


## Available Tools (4)
- **get_portfolio_concentration**: Identifies if an asset's weight exceeds predefined risk thresholds
- **calculate_rebalancing_requirement**: Determines how much value must be added or removed from an asset to reach a target weight
- **get_asset_weight**: Calculates the specific percentage weight of a single asset within a portfolio
- **validate_portfolio_composition**: Checks if the sum of all asset weights in a portfolio is mathematically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Weight Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the weight of a $25,000 asset in a $100,000 portfolio?"

**🤖 AI Agent:**
> The asset weight is 25%.

---

**👤 You:**
> "Is an asset worth $40,000 in a $100,000 portfolio concentrated if my threshold is 0.35?"

**🤖 AI Agent:**
> Yes, the asset is concentrated. The current weight is 40%, which exceeds the 35% threshold by 5%.

---

**👤 You:**
> "How much should I add to an asset worth $10,000 in a $100,000 portfolio to make it 20% of the total?"

**🤖 AI Agent:**
> You need to add $10,000 to the asset to reach the target weight of 20%.


## ❓ FAQ

**Q: How do I check if my portfolio is too concentrated?**
You can use the `get_portfolio_concentration` tool to check if an asset's weight exceeds your specified risk threshold.

**Q: Can I calculate how much to buy to reach a target weight?**
Yes, the `calculate_rebalancing_requirement` tool determines the exact monetary amount needed to reach your target weight.

**Q: How is the asset weight calculated?**
The `get_asset_weight` tool calculates the weight by dividing the individual asset value by the total portfolio value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/portfolio-weight-engine](https://vinkius.com/en/ai-agent-connect/portfolio-weight-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Weight Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-weight-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Weight Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-weight-engine": {
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
