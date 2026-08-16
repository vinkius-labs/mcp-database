# High-Low Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/high-low-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate market breadth, cumulative summation, and detect momentum divergence.

## Description
This MCP server provides deterministic tools to analyze market breadth using the High-Low Index. It allows AI agents to calculate the core `calculate_breadth_metrics` to determine bullish or bearish sentiment, track long-term trends via `calculate_cumulative_summation`, smooth data with `analyze_moving_average`, and identify potential trend reversals using `detect_divergence`.


## Available Tools (4)
- **analyze_moving_average**: 
- **calculate_breadth_metrics**: 
- **calculate_cumulative_summation**: 
- **detect_divergence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **High-Low Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the market breadth sentiment for 60 new highs and 40 new lows."

**🤖 AI Agent:**
> The High-Low Index is 60.0, which indicates bullish breadth.

---

**👤 You:**
> "What is the cumulative summation if the current index is 55 and the previous sum was 10?"

**🤖 AI Agent:**
> The updated cumulative summation is 15.0.

---

**👤 You:**
> "Check for divergence with price highs [150, 155, 160] and index highs [45, 48, 47]."

**🤖 AI Agent:**
> A bearish_divergence was detected because the price reached a new high while the High-Low Index did not.


## ❓ FAQ

**Q: What is the High-Low Index?**
The High-Low Index is a momentum indicator that compares the number of stocks reaching new highs against those reaching new lows to quantify market breadth.

**Q: How do I detect market divergence?**
You can use the `detect_divergence` tool to compare recent price peaks against High-Low Index peaks to identify potential trend reversals.

**Q: Can I calculate moving averages for the index?**
Yes, the `analyze_moving_average` tool allows you to smooth the High-Low Index over a specified period to identify the underlying trend.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/high-low-index-calculator](https://vinkius.com/ai-agent-connect/high-low-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **High-Low Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `high-low-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **High-Low Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "high-low-index-calculator": {
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
