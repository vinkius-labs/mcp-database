# OBV Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/obv-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic On-Balance Volume (OBV) analysis engine.

## Description
This MCP server provides a deterministic technical analysis engine for On-Balance Volume (OBV). It connects AI agents to precise volume flow calculations, including OBV series generation, moving averages, slope analysis, and divergence detection. Use `calculate_obv_series` to generate the core volume series, `analyze_obv_trends` for smoothing and momentum, `detect_divergences` to find price-volume discrepancies, and `classify_volume_flow` to identify Accumulation or Distribution states.


## Available Tools (4)
- **analyze_obv_trends**: Provides smoothing and momentum metrics based on the calculated OBV
- **detect_divergences**: Identifies discrepancies between price movement and volume movement
- **calculate_obv_series**: Computes the complete series of On-Balance Volume values from price and volume data
- **classify_volume_flow**: Categorizes the current market state as Accumulation or Distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OBV Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the OBV series for these closing prices: [150, 152, 151, 153] and volumes: [1000, 1200, 800, 1500]."

**🤖 AI Agent:**
> The OBV series is: [1000, 2200, 1400, 2900].

---

**👤 You:**
> "Is the current market state accumulation or distribution based on these OBV values and slopes: [100, 110, 120] and [10, 10]?"

**🤖 AI Agent:**
> The current market state is Accumulation.

---

**👤 You:**
> "Check for divergences in these prices [10, 12, 11, 13] and OBV values [100, 105, 102, 103]."

**🤖 AI Agent:**
> A bearish divergence was detected at index 3.


## ❓ FAQ

**Q: What is On-Balance Volume (OBV)?**
OBV is a momentum indicator that uses volume flow to predict changes in stock price by analyzing whether volume is flowing into or out of a security.

**Q: How do I detect market accumulation?**
You can use the `classify_volume_flow` tool to identify Accumulation, which is characterized by rising OBV or bullish divergence.

**Q: Can I detect price-volume divergences?**
Yes, the `detect_divergences` tool identifies discrepancies where price movement and OBV movement do not align.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/obv-calculator](https://vinkius.com/ai-agent-connect/obv-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OBV Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `obv-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OBV Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "obv-calculator": {
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
