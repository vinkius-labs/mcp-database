# Candlestick Pattern Recognizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/candlestick-pattern-recognizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify single, two, and three-bar candlestick patterns from price data.

## Description
This MCP server provides a deterministic engine for identifying candlestick patterns in financial markets. It analyzes price action through single-bar shapes, two-bar relationships, and complex three-bar sequences. Use `single_bar_patterns` to detect immediate sentiment shifts like Dojis or Hammers, `two_bar_patterns` for reversal patterns like Engulfing, and `three_bar_patterns` for complex sequences like Morning Stars. It returns the pattern name, market direction, and a reliability score.


## Available Tools (3)
- **single_bar_patterns**: Identify single-candle candlestick patterns
- **three_bar_patterns**: Identify complex three-bar candlestick patterns
- **two_bar_patterns**: Identify two-bar candlestick reversal patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Candlestick Pattern Recognizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify any single-bar patterns for a candle with open 100, high 105, low 95, and close 100."

**🤖 AI Agent:**
> The identified pattern is Doji.

---

**👤 You:**
> "Check for two-bar patterns where the current bar is open 110, high 115, low 105, close 112 and the previous bar was open 100, high 102, low 98, close 101."

**🤖 AI Agent:**
> The identified pattern is Bullish Engulfing.

---

**👤 You:**
> "What three-bar patterns are present for these three bars: bar1={open:10, high:12, low:9, close:11}, bar2={open:11, high:11.5, low:10.5, close:11}, bar3={open:11, high:14, low:11, close:13.5}?"

**🤖 AI Agent:**
> The identified pattern is Morning Star.


## ❓ FAQ

**Q: What patterns can the engine identify?**
The engine identifies single-bar patterns (Doji, Hammer, etc.), two-bar patterns (Engulfing, Piercing Line, etc.), and three-bar patterns (Morning Star, Three White Soldiers, etc.) using `single_bar_patterns`, `two_bar_patterns`, and `three_bar_patterns` tools.

**Q: How is the reliability score determined?**
The reliability score is a deterministic value calculated by the engine based on the mathematical precision of the price relationships defined in the pattern logic.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP server to Claude Desktop, Cursor, VS Code, or any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/candlestick-pattern-recognizer](https://vinkius.com/mcp/candlestick-pattern-recognizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Candlestick Pattern Recognizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `candlestick-pattern-recognizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Candlestick Pattern Recognizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "candlestick-pattern-recognizer": {
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
