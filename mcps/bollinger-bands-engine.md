# Bollinger Bands Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bollinger-bands-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate moving standard deviation and Bollinger Bands for financial time-series deterministically.

## Description
Bollinger Bands are crucial for measuring market volatility. They require computing a moving average, then a moving standard deviation, and then adding/subtracting it to form Upper and Lower bands. LLMs fail completely at calculating rolling standard deviations. This engine handles the complex math locally, returning exact arrays for the Upper, Middle, and Lower bands.


## Available Tools (1)
- **calculate_bollinger_bands**: Provide an array of numbers and optional period/stdDev.

Calculates precise Bollinger Bands (Upper, Middle, Lower)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bollinger Bands Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standard 20-period, 2-std-dev Bollinger Bands for this BTC price history."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Compute the Bollinger Bands, then list all the dates where the closing price was strictly greater than the Upper Band."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Calculate the width between the Upper and Lower bands. If the width shrinks by 50%, flag it as a 'Bollinger Squeeze'."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: What are the default parameters?**
The default is a 20-period moving average with a 2.0 standard deviation multiplier, which is the industry standard set by John Bollinger.

**Q: How do I spot breakouts?**
When prices break above the Upper Band, it signals strong momentum (or overbought conditions). Breaking below the Lower Band signals a sell-off (or oversold conditions).

**Q: Can it be used for non-financial data?**
Absolutely. Bollinger Bands are just rolling standard deviations. You can use them to detect statistical anomalies in server latency or sensor temperatures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bollinger-bands-engine](https://vinkius.com/mcp/bollinger-bands-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bollinger Bands Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bollinger-bands-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bollinger Bands Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bollinger-bands-engine": {
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
