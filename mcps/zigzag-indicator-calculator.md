# ZigZag Indicator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/zigzag-indicator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect price swing points and analyze market structure using deterministic ZigZag logic.

## Description
This MCP server provides precise tools for technical analysis of price action. It uses a state-machine-based ZigZag algorithm to identify significant market turning points. Use `detect_swing_pivots` to find confirmed swing highs and lows based on a custom deviation percentage. Once pivots are identified, use `analyze_swing_metrics` to calculate the amplitude and duration of each move, or `interpret_market_structure` to receive hints about Elliott Wave patterns like impulse or corrective waves.


## Available Tools (3)
- **analyze_swing_metrics**: Calculates the intensity and duration of the movements between the detected pivots
- **detect_swing_pivots**: Identifies all confirmed high and low pivot points within a price series based on a deviation threshold
- **interpret_market_structure**: Provides high-level hints regarding whether the sequence of pivots resembles an impulse or corrective wave pattern


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZigZag Indicator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the swing pivots for these high prices [100, 105, 102, 110, 108] and low prices [95, 98, 97, 105, 103] with a 5% deviation."

**🤖 AI Agent:**
> The confirmed pivots are: High at index 1 (price 105), Low at index 2 (price 97), and High at index 3 (price 110).

---

**👤 You:**
> "Analyze the market structure for these pivots: [{'barIndex': 0, 'price': 10, 'type': 'low'}, {'barIndex': 5, 'price': 20, 'type': 'high'}, {'barIndex': 10, 'price': 15, 'type': 'low'}, {'barIndex': 15, 'price': 25, 'type': 'high'}, {'barIndex': 20, 'price': 20, 'type': 'low'}]"

**🤖 AI Agent:**
> The current sequence suggests an impulse wave pattern with a confidence of 0.8.

---

**👤 You:**
> "Calculate the amplitude and duration for the following pivots: [{'barIndex': 10, 'price': 100, 'type': 'low'}, {'barIndex': 15, 'price': 110, 'type': 'high'}]"

**🤖 AI Agent:**
> The movement between these pivots has an amplitude of 10.0% and a duration of 5 bars.


## ❓ FAQ

**Q: How does the deviation percentage work?**
The deviation percentage is the minimum price movement required to confirm a change in direction. A new pivot is only confirmed when the price reverses by this percentage from the previous pivot.

**Q: Can I identify Elliott Wave patterns?**
Yes, by using the `interpret_market_structure` tool, you can receive hints on whether the current sequence of pivots resembles an impulse or a corrective wave.

**Q: What information is included in the swing metrics?**
The `analyze_swing_metrics` tool provides the amplitude (percentage change) and the bar duration (time elapsed) between consecutive confirmed pivots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/zigzag-indicator-calculator](https://vinkius.com/ai-agent-connect/zigzag-indicator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZigZag Indicator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zigzag-indicator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZigZag Indicator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zigzag-indicator-calculator": {
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
