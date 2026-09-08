# infra-revenue-per-asset MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infra-revenue-per-asset)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculates revenue productivity per asset to identify performance trends and underperforming infrastructure.

## Description
This MCP server provides tools to analyze the economic efficiency of infrastructure assets. It calculates revenue per asset, identifies performance trends, and flags underperforming assets based on type-specific benchmarks. Use `asset_productivity_tool` to find the core revenue metric, `productivity_trend_tool` to track performance direction, `identify_underperforming_assets_tool` to find assets failing efficiency targets, and `utilization_adjusted_efficiency_tool` to factor in asset age and usage rates.


## Available Tools (4)
- **asset_productivity_tool**: Calculates the core revenue per asset metric for a specific asset or asset group
- **identify_underperforming_assets_tool**: Flags assets that are failing to meet efficiency benchmarks
- **utilization_adjusted_efficiency_tool**: Adjusts the productivity metric to account for how much an asset is being used versus its age
- **productivity_trend_tool**: Determines if the economic performance of an asset group is improving, declining, or stable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **infra-revenue-per-asset** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the revenue per asset for an energy asset with $500,000 revenue and a $2,000,000 value?"

**🤖 AI Agent:**
> The revenue per asset is $0.25.

---

**👤 You:**
> "Is the productivity of this asset group improving? The historical values are [10, 12, 15, 14, 18]."

**🤖 AI Agent:**
> The trend is improving with a positive rate of change.

---

**👤 You:**
> "Calculate the adjusted efficiency for an asset with $50 revenue per asset, 80% utilization, and 5 years of age."

**🤖 AI Agent:**
> The adjusted efficiency score is 40.0 with an optimal rating.


## ❓ FAQ

**Q: How is revenue per asset calculated?**
The `asset_productivity_tool` calculates this by dividing the total revenue attributed to an asset or group by its total capital value.

**Q: Can I identify assets that are not meeting their targets?**
Yes, you can use the `identify_underperforming_assets_tool` by providing a list of assets and their corresponding type-specific benchmarks.

**Q: How does asset age affect the efficiency score?**
The `utilization_adjusted_efficiency_tool` adjusts the productivity score by considering both the utilization rate and the age of the asset to provide a more accurate efficiency rating.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infra-revenue-per-asset](https://vinkius.com/ai-agent-connect/infra-revenue-per-asset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **infra-revenue-per-asset** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-revenue-per-asset` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **infra-revenue-per-asset** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-revenue-per-asset": {
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
