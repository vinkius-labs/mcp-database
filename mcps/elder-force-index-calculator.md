# Elder Force Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/elder-force-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Elder Force Index, detect trend signals, and identify price-momentum divergences.

## Description
This MCP server provides deterministic tools for calculating the Elder Force Index (EFI), a momentum indicator that combines price movement and volume. Use `calculate_force_index` to generate smoothed index values, `detect_trend_signals` to identify zero-line crosses and pullback zones, and `analyze_divergence` to find discrepancies between price action and momentum strength.


## Available Tools (3)
- **analyze_divergence**: Detect discrepancies between price movement and momentum strength
- **calculate_force_index**: The period defaults to 2.

Compute the raw Elder Force Index values for a provided series of price and volume data
- **detect_trend_signals**: Identify zero-line crosses and extreme pullback zones within the calculated Force Index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elder Force Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Force Index for these close prices: [150, 152, 151, 153] and volumes: [1000, 1100, 950, 1200]."

**🤖 AI Agent:**
> The calculated Force Index values are [0, 200, -100, 300].

---

**👤 You:**
> "Are there any trend signals in these index values: [0.5, -0.2, 0.8] with a period of 2?"

**🤖 AI Agent:**
> A Zero-Line Cross was detected at index 1.

---

**👤 You:**
> "Check for divergence with prices [10, 12, 11, 13] and index values [1, 2, 1.5, 1.8]."

**🤖 AI Agent:**
> Bearish Divergence detected at index 3.


## ❓ FAQ

**Q: What is the Elder Force Index?**
The Elder Force Index is a momentum indicator that measures the ability of a market to move in a specific direction by combining price changes and volume.

**Q: How do I detect a trend reversal?**
You can use `detect_trend_signals` to identify zero-line crosses, which indicate changes in momentum direction.

**Q: Can I detect divergences between price and momentum?**
Yes, the `analyze_divergence` tool detects when price makes new highs or lows that are not supported by the Force Index momentum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/elder-force-index-calculator](https://vinkius.com/ai-agent-connect/elder-force-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elder Force Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elder-force-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elder Force Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elder-force-index-calculator": {
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
