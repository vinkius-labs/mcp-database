# Negative Volume Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/negative-volume-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate NVI and PVI to identify smart money activity and market sentiment.

## Description
This MCP server provides deterministic tools for calculating the Negative Volume Index (NVI) and Positive Volume Index (PVI). Use `calculate_volume_indices` to generate raw time-series data, `analyze_market_sentiment` to detect bull or bear regimes and smart money confirmation, and `calculate_divergence` to identify discrepancies between price and volume indices.


## Available Tools (3)
- **analyze_market_sentiment**: 
- **calculate_divergence**: 
- **calculate_volume_indices**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Negative Volume Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the volume indices for these prices: [100, 102, 101, 105] and volumes: [500, 450, 400, 600]."

**🤖 AI Agent:**
> The calculated NVI and PVI series have been generated based on the provided price and volume history.

---

**👤 You:**
> "Is there smart money confirmation in this data?"

**🤖 AI Agent:**
> Yes, the NVI is rising while the price is also rising, indicating smart money accumulation.

---

**👤 You:**
> "What is the current market sentiment?"

**🤖 AI Agent:**
> The current market regime is a Bull Market as the NVI is above its 255-day moving average.


## ❓ FAQ

**Q: What is the purpose of the NVI?**
The NVI is used to track 'smart money' activity by looking at price changes on days with lower than average volume.

**Q: How do I identify a bull market using these tools?**
A bull market is identified when the NVI is currently higher than its 255-day moving average, which can be determined via `analyze_market_sentiment`.

**Q: Can I calculate divergence between price and volume?**
Yes, use the `calculate_divergence` tool to find the relationship between price movement and the NVI or PVI indices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/negative-volume-index-calculator](https://vinkius.com/ai-agent-connect/negative-volume-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Negative Volume Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `negative-volume-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Negative Volume Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "negative-volume-index-calculator": {
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
