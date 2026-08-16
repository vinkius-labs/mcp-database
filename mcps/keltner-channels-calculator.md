# Keltner Channels Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/keltner-channels-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis for Keltner Channels, volatility squeezes, and breakouts.

## Description
This MCP server provides a deterministic engine for technical analysis using Keltner Channels. It allows AI agents to compute volatility envelopes, identify market squeezes, and detect price breakouts. Use `calculate_keltner_channels` to derive middle lines, upper/lower boundaries, and channel width. Use `detect_volatility_squeeze` to identify low-volatility periods when Bollinger Bands contract within the Keltner Channels. Finally, use `analyze_breakouts` to find specific price movements that exit the volatility envelope.


## Available Tools (3)
- **analyze_breakouts**: Identifies indices where the price has broken out of the volatility envelope
- **calculate_keltner_channels**: Computes the core Keltner Channel boundaries and volatility metrics
- **detect_volatility_squeeze**: Determines if the market is in a low-volatility squeeze


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keltner Channels Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Keltner Channels for these prices: High [10, 12, 11], Low [8, 9, 10], Close [9, 11, 10.5]."

**🤖 AI Agent:**
> The middle line is 10.17, the upper channel is 12.34, and the lower channel is 7.99.

---

**👤 You:**
> "Is there a volatility squeeze happening right now?"

**🤖 AI Agent:**
> No, the Bollinger Bands are currently wider than the Keltner Channels, so no squeeze is detected.

---

**👤 You:**
> "Did the price break out of the channel?"

**🤖 AI Agent:**
> Yes, an UPPER_BREAKOUT was detected at index 5.


## ❓ FAQ

**Q: How do I calculate the Keltner Channel boundaries?**
You can use the `calculate_keltner_channels` tool by providing arrays of high, low, and close prices along with the desired EMA and ATR periods.

**Q: What is a volatility squeeze?**
A squeeze occurs when market volatility is low, specifically when Bollinger Bands fall inside the Keltner Channels. You can detect this using `detect_volatility_squeeze`.

**Q: How can I identify price breakouts?**
Use the `analyze_breakouts` tool with your closing prices and the previously calculated channel boundaries to identify UPPER_BREAKOUT or LOWER_BREAKOUT signals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/keltner-channels-calculator](https://vinkius.com/ai-agent-connect/keltner-channels-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keltner Channels Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keltner-channels-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keltner Channels Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keltner-channels-calculator": {
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
