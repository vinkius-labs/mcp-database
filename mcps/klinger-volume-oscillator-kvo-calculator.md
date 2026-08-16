# Klinger Volume Oscillator (KVO) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/klinger-volume-oscillator-kvo-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise Klinger Volume Oscillator values, signal crossovers, and price divergence.

## Description
This MCP server provides deterministic tools for technical analysis using the Klinger Volume Oscillator (KVO). It allows AI agents to calculate core KVO metrics, detect momentum shifts through signal crossovers, and identify potential trend reversals via price divergence analysis. Use `calculate_kvo_metrics` to generate the oscillator and signal line, `analyze_kvo_signals` to find bullish or bearish crossovers, and `detect_kvo_divergence` to spot discrepancies between price action and volume momentum.


## Available Tools (3)
- **analyze_kvo_signals**: Detect momentum signals including crossovers and trend confirmations
- **calculate_kvo_metrics**: Optional periods for short, long, and signal EMAs can be provided.

Calculate core Klinger Volume Oscillator (KVO) values and the signal line
- **detect_kvo_divergence**: Identify potential trend reversals by finding discrepancies between price movement and KVO movement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klinger Volume Oscillator (KVO) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the KVO metrics for these prices: highs [150, 155], lows [145, 148], closes [148, 152], and volumes [1000, 1200]."

**🤖 AI Agent:**
> The calculated KVO values and signal line for the provided dataset are ready for analysis.

---

**👤 You:**
> "Analyze these KVO and signal values for crossovers: kvoValues [1.5, 2.0, 0.5], signalValues [1.0, 1.2, 1.8]."

**🤖 AI Agent:**
> A bearish crossover was detected at index 2.

---

**👤 You:**
> "Check for divergence between these closing prices [100, 110, 105] and KVO values [1, 2, 1.5]."

**🤖 AI Agent:**
> A bearish divergence was identified.


## ❓ FAQ

**Q: What is the Klinger Volume Oscillator?**
The Klinger Volume Oscillator (KVO) is a volume-based momentum indicator that identifies trend changes by combining price action with volume intensity.

**Q: How do I detect a trend reversal?**
You can use `detect_kvo_divergence` to find instances where price movement and KVO movement conflict, which often signals a reversal.

**Q: Can I customize the EMA periods?**
Yes, the `calculate_kvo_metrics` tool allows you to specify custom short, long, and signal EMA periods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/klinger-volume-oscillator-kvo-calculator](https://vinkius.com/ai-agent-connect/klinger-volume-oscillator-kvo-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Klinger Volume Oscillator (KVO) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klinger-volume-oscillator-kvo-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Klinger Volume Oscillator (KVO) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klinger-volume-oscillator-kvo-calculator": {
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
