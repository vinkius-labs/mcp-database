# Basis Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basis-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and analyze commodity basis by comparing local physical prices against exchange futures.

## Description
The Basis Calculator MCP server provides AI agents with specialized tools to determine market parity for commodities. Using `calculate_current_basis`, agents can compute the absolute basis value and identify if a market is Above or Below Parity. The server also includes `get_historical_averages` to benchmark current prices against historical regional data, and `get_seasonality_trend` to predict basis movements during Harvest or Off-season periods.


## Available Tools (3)
- **calculate_current_basis**: Positive is Above Parity, negative is Below Parity.

Determine the absolute basis value and its market classification based on current pricing
- **get_historical_averages**: Retrieve hardcoded historical basis averages for specific regions and commodities
- **get_seasonality_trend**: Identify the expected basis movement pattern for a specific period in the agricultural cycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basis Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the basis if the physical price is 120 and the future price is 115."

**🤖 AI Agent:**
> The absolute basis value is 5, which indicates a market position of Above Parity.

---

**👤 You:**
> "What is the historical average basis for Mato Grosso - Soy?"

**🤖 AI Agent:**
> The historical average basis for Mato Grosso - Soy is retrieved from the registry to provide context.

---

**👤 You:**
> "What is the expected trend during the Harvest season?"

**🤖 AI Agent:**
> During the Harvest season, the basis movement direction is typically identified as part of the seasonal behavior profile.


## ❓ FAQ

**Q: How can I calculate the current market parity?**
Use the `calculate_current_basis` tool by providing the local physical price and the futures contract price for the same maturity.

**Q: Can I check historical basis values for specific regions?**
Yes. By using `get_historical_averages`, an agent can retrieve hardcoded historical mean basis values for a given location and commodity.

**Q: Does the server provide information on seasonal trends?**
Yes, the `get_seasonality_trend` tool identifies expected basis movements (Increasing, Decreasing, or Stable) based on whether it is currently Harvest or Off-season.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basis-calculator](https://vinkius.com/mcp/basis-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basis Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basis-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basis Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basis-calculator": {
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
