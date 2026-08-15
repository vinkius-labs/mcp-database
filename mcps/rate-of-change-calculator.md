# Rate of Change Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rate-of-change-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate deterministic Rate of Change (ROC) and Momentum to identify market trends and divergences.

## Description
This MCP server provides deterministic financial analysis tools for calculating Rate of Change (ROC) and Momentum. It allows AI agents to analyze price velocity and identify market trends through specific indicators. Use `calculate_basic_indicators` to get fundamental ROC and Momentum values, `analyze_roc_trend` to detect zero-line crossings and moving average trends, or `detect_extremes_and_divergence` to identify overbought/oversold conditions and price-momentum divergences.


## Available Tools (3)
- **analyze_roc_trend**: Evaluate ROC trend using a moving average and identify zero-line crossings
- **detect_extremes_and_divergence**: Identify overbought/oversold conditions and price-momentum divergences
- **calculate_basic_indicators**: Calculate fundamental ROC and Momentum values for a price series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rate of Change Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the basic ROC and Momentum for these closing prices: [100, 102, 101, 105, 107, 110]."

**🤖 AI Agent:**
> The calculated ROC is 10.0% and the Momentum is 10.0.

---

**👤 You:**
> "Check if there is a bearish divergence in this price series: [150, 155, 152, 158, 156]."

**🤖 AI Agent:**
> A bearish divergence was detected as the price reached a higher high but the momentum indicator showed a lower high.

---

**👤 You:**
> "Is the current ROC trend showing a zero-line cross up?"

**🤖 AI Agent:**
> Yes, the current ROC has crossed above the zero line, indicating accelerating upward momentum.


## ❓ FAQ

**Q: What is the difference between ROC and Momentum?**
ROC measures the percentage change in price over a period, representing velocity, while Momentum measures the absolute price change.

**Q: How can I detect market reversals?**
You can use `detect_extremes_and_divergence` to find overbought/oversold zones or identify bullish and bearish divergences between price and momentum.

**Q: How do I identify trend changes?**
Use `analyze_roc_trend` to monitor zero-line crosses and the ROC moving average to confirm trend direction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rate-of-change-calculator](https://vinkius.com/mcp/rate-of-change-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rate of Change Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rate-of-change-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rate of Change Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rate-of-change-calculator": {
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
