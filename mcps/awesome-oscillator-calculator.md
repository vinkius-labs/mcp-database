# Awesome Oscillator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/awesome-oscillator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Bill Williams' Awesome Oscillator and detect momentum patterns.

## Description
This MCP server provides deterministic tools for calculating the Awesome Oscillator (AO) based on Bill Williams' methodology. It allows AI agents to process high and low price data to generate AO series, identify momentum shifts via `detect_patterns`, and classify market sentiment using `analyze_trend_signals`. Users can identify specific signatures like the Saucer pattern or Twin Peaks to better understand trend strength and direction.


## Available Tools (3)
- **analyze_trend_signals**: Classifies the specific type of zero-line cross to determine market sentiment
- **calculate_ao_series**: Generates the raw AO values and histogram colors for a provided set of price data
- **detect_patterns**: Identifies specific Bill Williams pattern signatures within the calculated AO series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Awesome Oscillator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the AO series for these prices: Highs [10, 12, 11, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43] and Lows [9, 11, 10, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42]."

**🤖 AI Agent:**
> The calculated AO values and histogram colors have been generated based on the provided median prices.

---

**👤 You:**
> "Detect patterns in these AO values: [1.5, 1.2, 1.4, 1.1, 1.3] and colors: ['green', 'red', 'green', 'red', 'green']."

**🤖 AI Agent:**
> No specific patterns like Saucers or Twin Peaks were detected in the provided sequence.

---

**👤 You:**
> "Identify the trend signal for AO values: [-0.5, -0.2, 0.1, 0.4]."

**🤖 AI Agent:**
> A Bullish Cross was detected as the AO value moved from negative to positive.


## ❓ FAQ

**Q: What data is required to use the AO tools?**
To use `calculate_ao_series`, you must provide arrays of high and low price points. Ensure both arrays have at least 34 elements to satisfy the SMA requirements.

**Q: How are patterns like Saucers detected?**
Patterns are identified using the `detect_patterns` tool, which analyzes the AO values and histogram colors for specific momentum signatures like Saucers or Twin Peaks.

**Q: Can I identify Bullish or Bearish crosses?**
Yes, the `analyze_trend_signals` tool classifies zero-line crosses as either Bullish or Bearish based on the direction of the AO movement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awesome-oscillator-calculator](https://vinkius.com/mcp/awesome-oscillator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Awesome Oscillator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `awesome-oscillator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Awesome Oscillator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "awesome-oscillator-calculator": {
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
