# MACD Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/macd-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis engine for MACD indicators and signals.

## Description
This MCP server provides a deterministic engine for calculating Moving Average Convergence Divergence (MACD) indicators. It allows AI agents to perform precise technical analysis by generating MACD lines, signal lines, and histograms. Use `calculate_macd_indicators` to generate the full indicator suite, `analyze_crossovers` to detect bullish or bearish momentum shifts, `detect_zero_crossings` to identify trend direction changes, and `detect_histogram_divergence` to find potential trend reversals through price and momentum discrepancies.


## Available Tools (4)
- **calculate_macd_indicators**: Generates the full suite of MACD values (Line, Signal, and Histogram) for a given price series
- **analyze_crossovers**: Identifies momentum shifts by detecting crossovers between the MACD line and the Signal line
- **detect_histogram_divergence**: Detects potential trend reversals by finding discrepancies between price movement and histogram momentum
- **detect_zero_crossings**: Identifies when the MACD line crosses the zero threshold, signaling a change in trend direction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MACD Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the MACD indicators for this price series: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.1, 157.5, 158.0, 157.2]"

**🤖 AI Agent:**
> The MACD line is 1.25, the signal line is 0.85, and the histogram is 0.40.

---

**👤 You:**
> "Check if there was a bullish crossover in this MACD data: [{'macdLine': 1.5, 'signalLine': 1.2}, {'macdLine': 1.8, 'signalLine': 1.4}]"

**🤖 AI Agent:**
> A bullish crossover was detected at index 1.

---

**👤 You:**
> "Did the MACD line cross the zero line in this data: [{'macdLine': -0.5}, {'macdLine': 0.2}]"

**🤖 AI Agent:**
> An upward zero-line crossing was detected at index 1.


## ❓ FAQ

**Q: How are the EMA values initialized?**
To ensure deterministic results, the first EMA value in a series is calculated as the Simple Moving Average (SMA) of the first N periods.

**Q: What tools are available in this server?**
The server provides `calculate_macd_indicators` for data generation, `analyze_crossovers` for momentum shifts, `detect_zero_crossings` for trend changes, and `detect_histogram_divergence` for trend reversals.

**Q: Can I use custom periods for the MACD calculation?**
Yes, you can specify custom values for the fast, slow, and signal periods when calling `calculate_macd_indicators`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/macd-calculator](https://vinkius.com/ai-agent-connect/macd-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MACD Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `macd-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MACD Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "macd-calculator": {
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
