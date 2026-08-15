# Williams Fractals Indicator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/williams-fractals-indicator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [technical-analysis](../categories/technical-analysis.md)

Detect Williams Fractal patterns, structural levels, and breakout signals.

## Description
This MCP server provides deterministic technical analysis for identifying Williams Fractal patterns in price action. It identifies confirmed up-fractals and down-fractals using a 5-bar pattern, allowing for the calculation of key structural levels. Use `get_fractal_patterns` to find peaks and valleys, `get_fractal_metrics` to determine resistance, support, and fractal density, or `check_breakout_signal` to detect when price breaches recent structural levels. It is designed to bridge AI agents with precise market structure data.


## Available Tools (3)
- **check_breakout_signal**: Determines if the current price action has breached the most recent structural fractal levels
- **get_fractal_metrics**: Calculates structural levels and market activity based on recent fractal occurrences
- **get_fractal_patterns**: Identifies all confirmed up-fractals and down-fractals within a provided price series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Williams Fractals Indicator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify all confirmed fractal patterns in this price data: highs [10, 12, 15, 13, 11, 10] and lows [5, 6, 4, 5, 6, 7]."

**🤖 AI Agent:**
> The detected patterns are: Up-Fractal at price 15 (index 2) and Down-Fractal at price 4 (index 2).

---

**👤 You:**
> "Calculate the resistance and support levels for these fractals: upFractals '[{"price": 150, "index": 10}]' and downFractals '[{"price": 140, "index": 12}]'."

**🤖 AI Agent:**
> The resistance level is 150 and the support level is 140.

---

**👤 You:**
> "Check if a price of 155 is a breakout given an up-fractal at 150 and a down-fractal at 140."

**🤖 AI Agent:**
> Yes, there is an Up-Breakout because the price 155 is greater than the most recent Up-Fractal at 150.


## ❓ FAQ

**Q: What is a Williams Fractal?**
A Williams Fractal is a five-bar price pattern where the middle bar's high (for up-fractals) or low (for down-fractals) is the highest or lowest among the surrounding four bars.

**Q: How is the breakout signal calculated?**
The `check_breakout_signal` tool determines a breakout when the current price closes strictly above the most recent confirmed Up-Fractal or strictly below the most recent confirmed Down-Fractal.

**Q: Is there a delay in fractal detection?**
Yes, because a fractal requires two subsequent bars to confirm the pattern, there is a 2-bar confirmation lag before a fractal is considered valid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/williams-fractals-indicator](https://vinkius.com/mcp/williams-fractals-indicator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Williams Fractals Indicator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `williams-fractals-indicator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Williams Fractals Indicator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "williams-fractals-indicator": {
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
