# Pit Optimization (Lerchs-Grossmann) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pit-optimization-lerchs-grossmann)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal open-pit mine limits using the Lerchs-Grossmann algorithm.

## Description
This MCP server provides specialized tools for open-pit mine planning. It uses the Lerchs-Grossmann algorithm to determine the most profitable pit shell by analyzing 3D block models. Users can transform raw data into economic values using `calculate_block_values`, execute the core optimization with `run_lg_optimization`, and aggregate business results via `summarize_pit_metrics`. The server also includes `validate_geotechnical_safety` to ensure pit walls respect required slope constraints.


## Available Tools (4)
- **calculate_block_values**: Transforms raw block model data and economic parameters into net profit/loss values for every individual block
- **run_lg_optimization**: Executes the Lerchs-Grossmann algorithm to identify the set of blocks that form the most profitable pit shell
- **summarize_pit_metrics**: Aggregates the results of an optimization into high-level business metrics
- **validate_geotechnical_safety**: Checks if a proposed set of pit blocks adheres to the safety slope constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pit Optimization (Lerchs-Grossmann)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the net values for my block model with a metal price of 1500 and a base mining cost of 50."

**🤖 AI Agent:**
> The block values have been calculated. The net value for block ID 101 is 450.50 and for block ID 102 is -12.30.

---

**👤 You:**
> "Run the LG optimization for these block values with a 45 degree slope angle."

**🤖 AI Agent:**
> The optimization is complete. The ultimate pit limit contains 450 blocks with a total NPV of 12,450,000.

---

**👤 You:**
> "What is the total contained metal in the optimized pit?"

**🤖 AI Agent:**
> The total contained metal in the optimized pit is 85,200 units.


## ❓ FAQ

**Q: What is the Lerchs-Grossmann algorithm?**
It is a mathematical method used to find the ultimate pit limit by maximizing total profit while respecting geotechnical slope constraints.

**Q: How does the tool handle mining costs?**
The `calculate_block_values` tool accounts for depth-dependent costs by applying a multiplier to the base mining cost as the z-coordinate decreases.

**Q: Can I verify if my pit design is safe?**
Yes, you can use the `validate_geotechnical_safety` tool to check if your proposed pit blocks adhere to the specified slope angles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pit-optimization-lerchs-grossmann](https://vinkius.com/ai-agent-connect/pit-optimization-lerchs-grossmann)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pit Optimization (Lerchs-Grossmann)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pit-optimization-lerchs-grossmann` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pit Optimization (Lerchs-Grossmann)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pit-optimization-lerchs-grossmann": {
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
