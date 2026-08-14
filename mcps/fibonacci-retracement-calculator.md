# Fibonacci Retracement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fibonacci-retracement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise Fibonacci retracement levels, price extensions, and time zones.

## Description
This MCP server provides deterministic technical analysis tools for traders. It calculates key Fibonacci retracement levels to identify support and resistance, projects price extension targets for profit taking, and identifies future time zones for potential market turns. Use `calculate_retracement_levels` to find support/resistance, `calculate_extension_targets` for price targets, `identify_current_testing_level` to see if price is near a level, and `calculate_time_zones` for temporal analysis.


## Available Tools (4)
- **calculate_extension_targets**: Projects future price targets for traders looking to take profit or enter trades after a retracement
- **calculate_retracement_levels**: Determines the specific price points where a market might find support or resistance during a retracement
- **calculate_time_zones**: Identifies the future time intervals (measured in bars/periods) where significant market turns might occur
- **identify_current_testing_level**: Identifies which specific Fibonacci retracement level the current market price is currently interacting with


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fibonacci Retracement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the Fibonacci retracement levels for a swing high of 150 and a swing low of 100?"

**🤖 AI Agent:**
> The retracement levels are: 23.6% at 140.2, 38.2% at 130.9, 50.0% at 125.0, 61.8% at 119.1, and 78.6% at 110.7.

---

**👤 You:**
> "Is the current price of 125.2 testing a level if the swing high was 150 and low was 100?"

**🤖 AI Agent:**
> Yes, the price is testing the 50.0% level (125.0).

---

**👤 You:**
> "What are the price extension targets for a swing high of 150 and low of 100?"

**🤖 AI Agent:**
> The extension targets are: 127.2% at 163.6, 161.8% at 180.9, 200.0% at 200.0, and 261.8% at 230.9.


## ❓ FAQ

**Q: How do I find support and resistance levels?**
You can use the `calculate_retracement_levels` tool by providing the swing high and swing low prices.

**Q: Can I see if the current price is at a Fibonacci level?**
Yes, the `identify_current_testing_level` tool checks if the current price is within a 0.5% tolerance of a calculated level.

**Q: How are extension targets calculated?**
Extension targets are projected using the `calculate_extension_targets` tool based on the provided swing high and low.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fibonacci-retracement-calculator](https://vinkius.com/mcp/fibonacci-retracement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fibonacci Retracement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fibonacci-retracement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fibonacci Retracement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fibonacci-retracement-calculator": {
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
