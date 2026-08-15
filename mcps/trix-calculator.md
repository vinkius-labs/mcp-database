# TRIX-Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trix-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Triple EMA oscillator for trend and momentum analysis.

## Description
TRIX-Calculator provides a deterministic technical analysis engine for the Triple Exponential Average (TRIX) oscillator. It transforms price data into smoothed momentum indicators, allowing AI agents to identify trend shifts and momentum changes. By using `calculate_trix_metrics`, agents can generate the TRIX series, signal line, and histogram. The engine also includes `detect_trix_signals` to identify zero-line crosses, signal crossovers, and divergences, and `get_trix_summary` for a rapid snapshot of current market momentum.


## Available Tools (3)
- **calculate_trix_metrics**: 
- **detect_trix_signals**: 
- **get_trix_summary**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TRIX-Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the TRIX metrics for these closing prices: [150.2, 152.5, 151.8, 153.0, 155.2, 154.5, 156.0]."

**🤖 AI Agent:**
> The TRIX series has been calculated with a default EMA period of 15 and signal period of 9. The latest TRIX value is 0.12, the signal is 0.08, and the histogram is 0.04.

---

**👤 You:**
> "Are there any trend signals in this TRIX data: [{"trixValue": 0.1, "signalValue": 0.05}, {"trixValue": -0.1, "signalValue": 0.02}]?"

**🤖 AI Agent:**
> A bearish zero-line cross was detected at index 1.

---

**👤 You:**
> "Give me a summary of the current momentum for this TRIX series: [{"trixValue": 0.5, "signalValue": 0.4, "histogramValue": 0.1}, {"trixValue": 0.6, "signalValue": 0.45, "histogramValue": 0.15}]."

**🤖 AI Agent:**
> The current status shows a bullish trend with increasing momentum.


## ❓ FAQ

**Q: What is the TRIX oscillator?**
TRIX is a momentum oscillator that uses triple-smoothed exponential moving averages to filter out market noise and identify trend changes.

**Q: How do I detect trend reversals?**
You can use `detect_trix_signals` to find zero-line crosses and signal crossovers, which indicate potential trend reversals.

**Q: Can I customize the smoothing periods?**
Yes, the `calculate_trix_metrics` tool allows you to specify both the EMA period and the signal period to suit different trading styles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trix-calculator](https://vinkius.com/mcp/trix-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TRIX-Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trix-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TRIX-Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trix-calculator": {
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
