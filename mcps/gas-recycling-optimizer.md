# Gas Recycling Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-recycling-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize gas recycling rates and predict condensate recovery in gas condensate reservoirs.

## Description
This MCP server provides specialized tools for managing gas condensate reservoirs. It allows AI agents to calculate the `get_optimal_recycling_rate` to maintain reservoir pressure above the dew point, `predict_breakthrough_time` to avoid premature dry gas arrival at production wells, and `calculate_condensate_recovery` to estimate liquid yields. Users can also use `evaluate_recycling_strategy` to validate if a proposed injection rate is viable for specific reservoir conditions.


## Available Tools (4)
- **calculate_condensate_recovery**: Estimates the total volume of liquid condensate that can be recovered using a specific recycling strategy
- **evaluate_recycling_strategy**: Provides a comprehensive assessment of a proposed recycling design by combining rate, breakthrough, and recovery metrics
- **get_optimal_recycling_rate**: Determines the most efficient volume of gas to inject to maximize recovery without causing premature breakthrough
- **predict_breakthrough_time**: Estimates when the injected dry gas will reach the production well


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Recycling Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best injection rate for a reservoir at 4500 psi with a dew point of 4200 psi and a rich gas composition?"

**🤖 AI Agent:**
> The optimal injection rate is 12.5 MMSCF/D, providing a pressure buffer of 300 psi and an efficiency index of 0.85.

---

**👤 You:**
> "Will a recycling rate of 15 MMSCF/D cause early breakthrough if the wells are 500 meters apart?"

**🤖 AI Agent:**
> The estimated time until breakthrough is 4.2 years, with a breakthrough risk factor of 0.15.

---

**👤 You:**
> "Estimate the total condensate recovery for a rate of 10 MMSCF/D with a maintenance factor of 0.8."

**🤖 AI Agent:**
> The total recovered volume is estimated at 1,250,000 barrels with a recovery efficiency of 78%.


## ❓ FAQ

**Q: How do I prevent liquid dropout in my reservoir?**
You can use `get_optimal_recycling_rate` to determine the injection volume needed to keep the reservoir pressure above the dew point, preventing retrograde condensation.

**Q: Can I test different injection rates?**
Yes, the `evaluate_recycling_strategy` tool allows you to test if a proposed rate is viable based on pressure maintenance and breakthrough risks.

**Q: How is breakthrough time calculated?**
The `predict_breakthrough_time` tool estimates the timing of dry gas arrival by considering the recycling rate, reservoir pressure, gas composition, and well spacing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-recycling-optimizer](https://vinkius.com/en/ai-agent-connect/gas-recycling-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Recycling Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-recycling-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Recycling Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-recycling-optimizer": {
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
