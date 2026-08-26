# True Strength Index (TSI) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/true-strength-index-tsi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic technical analysis engine for calculating TSI values, signal lines, and momentum signals.

## Description
This MCP server provides a deterministic technical analysis engine for the True Strength Index (TSI). It uses double exponential smoothing to calculate momentum-based indicators, helping identify trend direction and strength. Use `calculate_tsi_metrics` to generate TSI values and signal line crossovers, `detect_tsi_divergence` to find potential trend reversals, and `get_tsi_summary` for a high-level snapshot of current market momentum.


## Available Tools (3)
- **calculate_tsi_metrics**: Calculates the base TSI values, the signal line, and detects primary trend signals
- **get_tsi_summary**: Provides a high-level snapshot of the current market state based on the most recent TSI data
- **detect_tsi_divergence**: Identifies potential trend reversals by comparing price action against TSI movement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **True Strength Index (TSI) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the TSI metrics for these closing prices: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.8]."

**🤖 AI Agent:**
> The calculated TSI values and signal line have been generated, showing a bullish trend with a recent zero-line cross.

---

**👤 You:**
> "Are there any divergences in this data? Prices: [100, 105, 102, 108, 106] and TSI: [0.5, 0.8, 0.4, 0.9, 0.7]."

**🤖 AI Agent:**
> No significant divergences were detected in the provided data.

---

**👤 You:**
> "Give me a summary of the current market state using these TSI values: [0.1, 0.2, 0.5] and signal line: [0.0, 0.1, 0.3]."

**🤖 AI Agent:**
> The current trend state is Bullish with a Bullish Crossover detected.


## ❓ FAQ

**Q: What is the True Strength Index (TSI)?**
The TSI is a momentum indicator that uses double exponential smoothing to reduce lag and filter noise, helping traders identify trend strength.

**Q: How do I detect trend reversals?**
You can use the `detect_tsi_divergence` tool to identify bullish or bearish divergences between price action and the TSI indicator.

**Q: Can I get a quick summary of the current trend?**
Yes, the `get_tsi_summary` tool provides a snapshot of the current trend state and crossover status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/true-strength-index-tsi-calculator](https://vinkius.com/ai-agent-connect/true-strength-index-tsi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **True Strength Index (TSI) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `true-strength-index-tsi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **True Strength Index (TSI) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "true-strength-index-tsi-calculator": {
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
