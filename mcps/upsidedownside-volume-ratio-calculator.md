# Upside/Downside Volume Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/upsidedownside-volume-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate market pressure using UDVR, Tick Index, and exhaustion signals.

## Description
This MCP server provides deterministic financial analysis tools to measure market sentiment. Use `calculate_market_pressure` to determine buying or selling intensity via the Upside/Downside Volume Ratio (UDVR). Use `analyze_tick_index` to identify market exhaustion when the Tick Index reaches extreme levels. You can also use `get_udvr_percentile` to compare current UDVR against historical annual ranges.


## Available Tools (3)
- **analyze_tick_index**: Evaluate Tick Index for exhaustion
- **calculate_market_pressure**: Calculate UDVR and pressure class
- **get_udvr_percentile**: Get UDVR percentile rank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upside/Downside Volume Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the market pressure for an upside volume of 1500 and downside volume of 500."

**🤖 AI Agent:**
> The UDVR is 3.0, which indicates Strong Buying Pressure.

---

**👤 You:**
> "Check if the current Tick Index of 1200 indicates exhaustion given a history of [900, 850, 1000, 950, 800, 700, 600, 500, 400, 300]."

**🤖 AI Agent:**
> The 10-day moving average is 630, and the current reading indicates Positive Exhaustion.

---

**👤 You:**
> "What is the percentile rank for a UDVR of 1.2 if the annual history is [0.5, 0.8, 1.0, 1.1, 1.3, 1.5]?"

**🤖 AI Agent:**
> The percentile rank is 66.67.


## ❓ FAQ

**Q: What is UDVR?**
The Upside/Downside Volume Ratio (UDVR) is a metric representing the relative strength of buying versus selling volume.

**Q: How is market exhaustion identified?**
Exhaustion is identified via `analyze_tick_index` when the Tick Index exceeds 1000 or falls below -1000.

**Q: What constitutes strong buying pressure?**
Strong buying pressure is triggered when the UDVR calculated by `calculate_market_pressure` is greater than 1.5.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/upsidedownside-volume-ratio-calculator](https://vinkius.com/ai-agent-connect/upsidedownside-volume-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upside/Downside Volume Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upsidedownside-volume-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upside/Downside Volume Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upsidedownside-volume-ratio-calculator": {
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
