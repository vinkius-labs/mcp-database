# Put/Call Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/putcall-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate deterministic PCR metrics, sentiment scores, and statistical extremes.

## Description
This MCP server provides precise tools for analyzing market sentiment through Put/Call Ratios (PCR). It allows AI agents to calculate Volume PCR and Open Interest PCR, determine sentiment classifications (Bullish, Bearish, or Neutral), and identify statistical outliers using percentile ranks and z-scores. Use `calculate_pcr_metrics` to get core ratios, `analyze_sentiment_and_extremes` to evaluate sentiment against historical data, and `calculate_moving_averages` to identify trends via smoothed PCR series.


## Available Tools (3)
- **calculate_moving_averages**: Smooth PCR data to identify sentiment trends using a moving average
- **calculate_pcr_metrics**: Calculate primary volume and open interest PCR values
- **analyze_sentiment_and_extremes**: Determine sentiment classification, statistical percentile, and z-score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Put/Call Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the PCR metrics for 5000 puts and 4000 calls, with 10000 put OI and 8000 call OI."

**🤖 AI Agent:**
> The Volume PCR is 1.25 and the Open Interest PCR is 1.25.

---

**👤 You:**
> "Analyze the sentiment for a current PCR of 1.2 given a historical series of [0.8, 0.9, 1.1, 1.0, 1.2]."

**🤖 AI Agent:**
> The sentiment is Bearish, with a percentile rank of 1.0 and a z-score of 0.74.

---

**👤 You:**
> "What is the 21-day moving average for this PCR series: [0.7, 0.8, 0.75, 0.82, 0.78, 0.8, 0.79, 0.81, 0.8, 0.77, 0.76, 0.75, 0.74, 0.73, 0.72, 0.71, 0.7, 0.69, 0.68, 0.67, 0.66]?"

**🤖 AI Agent:**
> The 21-day moving average is 0.74.


## ❓ FAQ

**Q: What is the difference between Volume PCR and OI PCR?**
Volume PCR measures immediate market activity by comparing put and call volumes, while OI PCR (Open Interest) reflects long-term positioning and total outstanding contracts.

**Q: How is sentiment classified?**
Sentiment is classified as Bearish if the PCR is greater than 1.0 and Bullish if the PCR is less than 0.7. Values in between are considered Neutral.

**Q: Can I use this to find contrarian signals?**
Yes. Extreme sentiment values, identified via `analyze_sentiment_and_extremes` through high percentile ranks or z-scores, often serve as contrarian indicators for market tops or bottoms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/putcall-ratio-calculator](https://vinkius.com/ai-agent-connect/putcall-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Put/Call Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `putcall-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Put/Call Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "putcall-ratio-calculator": {
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
